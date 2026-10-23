---
id: pqart-pqart与pqcam安装流程
title: PQArt 与 PQCAM 安装流程
status: active
tags: [PQArt, 安装, 升级, PQCAM]
source: pq-skill/references/PQArt与PQCAM安装流程.md
updatedAt: 2026-09-22T04:18:47.255Z
---
# PQArt 与 PQCAM 安装流程

适用于远程 Windows 桌面安装同一构建号的 PQArt 和 PQCAM。

## 准备

1. 取同一构建号的 `PQArt_Ent_V11.2_x64_Setup_<构建号>.exe` 和 `pqCAM_x64_<构建号>.exe`；两个安装包必须来自同一构建号。需要最新构建时用 DailyBuild 源，见下节。
2. 复制到目标机本地临时目录并校验 SHA-256；安装器要在这个本地副本上运行，不要在共享路径上直接启动。
3. 关闭正在运行的 PQArt，在目标用户的交互桌面以高权限直接启动本地安装包，保持窗口可见。

### 安装包来源

DailyBuild 每个构建号一个目录，同时含 PQArt 与 PQCAM，实测可直接枚举读取：

```
\\192.168.99.185\RA-Files\RobotArt-DailyBuild\V11.2\<构建号>_<日期>\x64\Setup\PQArt_Ent_V11.2_x64_Setup_<构建号>.exe
\\192.168.99.185\RA-Files\RobotArt-DailyBuild\V11.2\<构建号>_<日期>\x64\Setup\patch\pqCAM_x64_<构建号>.exe
```

以 2026-09-22 的 11.2.0.8243 为例，两个包分别是 `...\11.2.0.8243_2026-09-22\x64\Setup\PQArt_Ent_V11.2_x64_Setup_8243.exe`（343 MB）和 `...\x64\Setup\patch\pqCAM_x64_8243.exe`（143 MB）。

- 目录名把构建号和日期拼在一起，例如 `11.2.0.8243_2026-09-22`；按名称排序取最后一个即最新，同一天可能有多个构建号。取最新目录：

```powershell
Get-ChildItem -LiteralPath '\\192.168.99.185\RA-Files\RobotArt-DailyBuild\V11.2' -Directory |
  Sort-Object Name | Select-Object -Last 1
```

- `x64\Setup` 根目录同时放着 Cpt、Edu、Sim 三种版本的安装包，Ent 版必须认准 `PQArt_Ent_V11.2_x64_Setup_<构建号>.exe`，不要误取 `PQArt_Cpt_x64_Setup_<构建号>.exe`、`PQArt_Edu_x64_Setup_<构建号>.exe` 或 `PQFactory_Sim_x64_Setup_<构建号>.exe`。
- CAM 包不在 `Setup` 根目录，而在 `Setup\patch\` 下。该子目录还有 `pqCAM_Exchange_x64_<构建号>.exe`、`pqExchange_x64_<构建号>.exe`、`RobotArt_Ent_ResLib_x64_<构建号>.exe`、`RobotArt_Edu_*` 等补丁包，按需取用。
- 另一来源是内网共享 `\\DESKTOP-IDCKPK1\share\pqart_setup\<日期>`，早期 8113、8221 从该处取得。两个来源都可用，按目标构建号选择。

2026-09-22 实测 8243 两个包：文件为 PE，内含 `Nullsoft`/`NSIS` 标记，属 NSIS 打包；`FileVersion` 与 `ProductVersion` 均为 `11.2.0.8243`，产品名分别是 `PQArt V11.2(64)` 和 `PQCAM_Package`。

## 静默安装（NSIS，已验证 11.2.0.8221）

两个安装包都是 NSIS 打包，支持 `/S` 静默安装，无需 GUI 或 computer use。安装顺序不能颠倒：先 PQArt，后 PQCAM。

DailyBuild 的最新构建走同一条静默路径：把 `Setup\PQArt_Ent_V11.2_x64_Setup_<构建号>.exe` 和 `Setup\patch\pqCAM_x64_<构建号>.exe` 复制到本地临时目录后，按下面的顺序执行即可。8243 的静默安装可用性由用户确认，本技能只在 share 包的 8221 上实测过完整流程。

1. 关闭所有 PQArt/`Unreal`/`RobotArt`/`pqCAM` 进程，并记下升级前基线：注册表版本、安装目录文件数与体积、C 盘剩余空间。
2. 把同一构建号的两个安装包复制到本地临时目录，并 `Unblock-File`。
3. 在管理员会话依次执行，轮询到安装进程退出：

```powershell
Start-Process -FilePath 'PQArt_Ent_V11.2_x64_Setup_8221.exe' -ArgumentList '/S'
Start-Process -FilePath 'pqCAM_x64_8221.exe' -ArgumentList '/S'
```

4. 校验三处版本都等于目标构建号：注册表 `DisplayVersion`、`bin\RobotArt\bin\RobotArt.exe` 的 `ProductVersion`、`bin\RobotArt\bin\apCam.dll` 的 `FileVersion`。
5. 启动冒烟：安装版 `RobotArt.exe` 应拉起 `Unreal`、`pqBridge`、`RobotArtHelper`，且进程状态为 `Responding`。

要点：PQArt 升级会先清空安装目录，把已装的 CAM 文件一并删除，所以**每次升级 PQArt 后都必须重装 PQCAM**。安装目录体积会先降后回升（2092 MB → 1025 MB → 2013 MB），可据此判断 CAM 是否漏装。PQCAM 没有独立卸载注册项，版本只能按 `apCam.dll` 等文件版本判断。

## 安装 PQArt

1. 启动 PQArt 安装包，核对安装版本和当前版本，点击“快速安装”。

   ![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/pqart-install.png)

2. 出现“安装完成”后立即点击右侧“完成安装”。
3. 核验卸载注册表中的 `DisplayVersion` 和 `bin\RobotArt\bin\RobotArt.exe` 文件版本等于目标版本。

## 安装 PQCAM

1. PQArt 安装完成后启动同构建号 PQCAM 安装包，保持目标为 `PQArt V11.2(64)`，点击“快速安装”。

   ![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/pqcam-install.png)

2. 出现“安装完成”后立即点击“完成安装”。

   ![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/pqcam-done.png)

3. 确认安装器退出，并核验 `apCam.dll`、`bmCamApi*.dll` 等 CAM 文件版本等于目标版本。

## 已验证版本

- `11.2.0.8113`：PQArt SHA-256 `D04D3B8F6C713611074827EF79C08E9BA5DA8331CA6D517ABC445B696F2EA185`；PQCAM SHA-256 `3FB11D1C07AF7F5E1E6AEDFAA94E12081BEB91D49DC7730A71C9EE193F2066A0`。
- `11.2.0.8243`（DailyBuild `11.2.0.8243_2026-09-22`）：打包类型、版本号、文件清单已在本机核实；静默安装尚未在本机复测。
