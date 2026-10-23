---
id: pqart-官方文档-使用说明书v2024
title: PQArt 工业机器人离线编程软件使用说明书（V2024）
status: active
tags: [PQArt, 使用手册, 官方文档, 操作, 入门]
source: D:\doc\pq\官方文档\1.PQArt工业机器人离线编程软件---使用说明书.docx
updatedAt: 2026-10-23T00:00:00.000Z
---

# PQArt

工业机器人离线编程软件

V2024

使用手册
## 软件应用环境
### 运行环境

推荐硬件：

CPU：intel i5 或同类性能以上 CPU；

内存：16G 以上内存；

显卡：4G 以上 NVIDIA 独显卡；

显示器：23寸及以上显示器；

推荐软件：

操作系统：Win10/Win11 (64 位) ；

分辨率：1920 ×1080（推荐）；

※ 网络要求：联网，可访问 Internet；
### 安装与登录

1、打开盘中文件，双击“PQArt_Ent_2024_x64_Setup.exe”应用程序。

2、有些操作系统会自动弹出 【用户账户控制】对话框，单击对话框中的【是】按钮，即可开始安装PQArt软件，如图 1.1所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image3.jpeg)
图 1.1 用户账户控制

3、首先弹出的是下图所示的对话框。直接点击“快速安装”按钮，等待完成安装，如图 1.2所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image4.png)
图 1.2 快速安装

点击“自定义安装”可自行设置软件安装路径。如图 1.3所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image5.png)
图 1.3 自定义安装

*只有勾选了“同意 PQArt 的用户许可协议”后，才能安装软件。

4、安装完成后即可登陆，如图1.4所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image6.png)
图1.4：登录页面

*试用用户：推荐使用微信直接扫描二维码，直接快速登录使用。

*正式用户：插入加密锁后，无需登录，可直接使用。
### 软件界面

PQArt采用Ribbon风格界面，一种以面板及标签页为架构的用户界面，丰富的命令布局可以帮助用户更容易地找到重要的、常用的功能。界面主要分为八大部分：标题栏、绘图区、机器人加工管理面板、菜单栏、机器人控制面板、调试面板、输出面板、状态栏等。如图1.5所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image7.png)
图1.5 功能界面

- 标题栏：用于显示软件的名称、账号角色和剩余时间等；功能面板涵盖了PQArt的基本功能，包括编程仿真、定义组件、校准、自由设计、程序编辑、显示、多机协同、二次开发、帮助，是软件中较为常用的功能栏；

- 菜单栏：涵盖了PQArt的基本功能，如场景搭建、设备状态、轨迹添加等，是最常用的功能栏；

- 绘图区：用于场景搭建、模型定义、轨迹添加和编辑等操作的显示和编辑界面；

- 机器人加工管理面板：共含有十个元素节点，包括场景、零件、坐标系、外部工具、快换工具、法兰工具、底座、状态机、机器人以及工作单元，通过面板中的树形结构可以轻松查看并管理机器人、工具和零件等场景元素；

- 调试面板：主要用于显示调整机器人各个轴的关节角信息，编辑轨迹点信息以及查看轨迹点当前状态；

- 机器人控制面板：可快速控制机器人轴关节的运动，读取机器人当前姿态，切换三维球参考坐标系以及控制机器人回到机械零点等；

- 输出面板：用于显示机器人执行的动作、指令、事件和轨迹点的状态；

- 状态栏：包括显示/隐藏某组件、显示全图、局部放大、选中物体显示居中、模型绘制样式、视向等功能。
## 编程仿真
### 文件

（1）新建：用于创建一个新的工程文件；

（2）打开：从电脑磁盘中打开一个存在的工程文件；

（3）保存：保存当前工程文件到电脑磁盘指定位置，若是已有保存记录的文件，默认保存到原位置；

（4）另存为：将当前工程文件另存到电脑磁盘指定位置；

（5）轻量化：用于将当前工程文件进行轻量保存到电脑磁盘指定位置，默认状态轻量化时只对场景节点下的模型进行轻量化处理，对其他定义过的模型不做轻量化处理。勾选“深度轻量化”功能后，将对该工程文件中的所有场景元素全部进行轻量化处理如图2.1所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image8.png)
图2.1：深度轻量化
### 场景搭建
##### 三维球

位置: 编程仿真-场景搭建-三维球 / 定义组件-场景-三维球

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image9.png)
图2.2：三维球位置

功能说明：三维球是一个非常简单实用的三维空间定位工具，它可以通过鼠标平移、旋转和原点定位的方式精确定位任何一个三维空间中的物体，同时还可以完成对轨迹旋转平移、轨迹点位姿调整以及产线设备坐标系定义等操作，在场景搭建、自定义、轨迹编辑等过程中发挥着至关重要的作用。

三维球功能默认状态为灰色不可选中状态，用户通过在绘图区或机器人加工管理面板中选中场景、零件、坐标系、机器人等三维空间中的对象后，三维球功能便会亮显可用，此时在功能栏点击三维球功能图标或快捷键F10可激活三维球；在设备定义、轨迹编辑或轨迹点编辑等操作中，无需手动激活三维球，选中相应功能后三维球便可自动弹出激活。

结构和颜色

在结构上，三维球由中心点（原点）、平移轴以及旋转轴三部分组成，如图2.3所示。中心点（原点）主要是用来点到点的移动，右击三维球中心点（原点）可以弹出对应的右键菜单，可以根据需求选择相应的功能，将三维球以中心点（原点）为基准，进行相应的操作。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image10.png)
图2.3：三维球工具

平移轴：有两种使用方法，方法一：拖动法，将三维球的其中一个轴用鼠标左键按住拖动，沿着平移方向拖动过程中出现的空白数值框内输入需要移动的距离数值后回车，默认单位为mm（输入数值的正负决定平移的正负方向），完成后物体将在该方向上平移相应的距离，如图2.4所示。方法二：右击平移轴菜单，右击三维球的平移轴弹出右键菜单，根据需求选取对应的功能。

旋转轴：有两种使用方法，方法一：拖动法，将三维球的一个旋转轴用鼠标左键按住拖动，在旋转过程中出现空白数值框输入需要旋转的角度数值后回车，默认单位为°（输入数值的正负决定旋转的正负方向），完成后物体将沿着该方向旋转相应的角度，如图2.5所示。方法二：右键旋转轴菜单，右击三维球的旋转轴弹出右键菜单，根据需求选取对应的功能。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image11.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image12.png)
图2.4：平移轴拖动                    图2.5：旋转轴拖动

三维球有三种不同的颜色，分别为：默认颜色（XYZ三个轴对应的颜色分别是红绿蓝）、白色、黄色，如图2.6所示，每种颜色都对应着不同的状态。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image13.png)
图2.6：三维球颜色

◎默认颜色：表示三维球和场景模型具有绑定关系，移动或旋转三维球后，模型也会随之移动和旋转。

◎白色：表示三维球和场景模型不具有绑定关系，移动和旋转三维球后，模型不会随着三维球的变化而变化。

◎黄色：此种颜色只有单条平移轴会出现，表示其余两轴方向已经被固定（约束），三维球只能在该条轴的方向上移动。

注：三维球被激活后，三维球和场景模型的绑定关系可以通过键盘上的空格键切换，在默认颜色时按一下空格键，三维球就会变成白色，此时三维球和场景模型解除绑定；同理在三维球为白色时，按一下空格键就会变成默认颜色，此时三维球和场景模型重新绑定。

点定位方式

点定位方式主要指的是基于三维球中心点的基本操作，在三维球被激活后，鼠标右键点击三维球中心点，即可弹出三维球右键菜单，如图2.7所示，点定位方式主要包括：编辑位置、到点、到中心点、点到点、到边的中点、Z向垂直到点以及到面中点共七种不同的编辑方式。

1. 编辑位置

编辑位置功能用来对场景中模型位置通过数值的方式进行精确快速的定位。

选中模型之后激活三维球，鼠标右键点击三维球中心点，在弹出的右键菜单中选择编辑位置功能，之后将弹出带文本输入框的编辑位置对话框，如图2.8所示。通过在X、Y、Z三个文本输入框中输入相应的数值，即可将三维球中心点快速移动相应的位置上。

注：输入的X、Y、Z数值是基于世界坐标系X、Y、Z方向上的数值偏移量，点击确定之后即可改变三维球中心点在世界坐标系中的绝对位置。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image14.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image15.png)
图2.7：点控制菜单                        图2.8：编辑位置示例

1. 到点

到点功能可以使和三维球绑定的模型移动到另一个模型上指定点的位置处。

选中模型之后激活三维球，鼠标右键点击三维球中心点，在弹出的右键菜单中选择到点功能，再选中另一个模型上某个点，三维球中心点便可快速移动至另一模型的指定点位置处，如图2.9所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image16.png)
图2.9：到点示例

1. 到中心点

到中心点可以使和三维球绑定的模型移动至另一个回转体中心的位置。

选中模型之后激活三维球，鼠标右键点击三维球中心点，在弹出的右键菜单中选择到中心点功能，通过拾取回转体的边或面实现以回转体轴线为基准或参考的装配关系，如图2.10所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image17.png)
图2.10：到中心点示例

1. 点到点

点到点可以使和三维球绑定的模型移动至另一个模型上指定两点（非重合点）连线的中心位置处。

选中模型之后激活三维球，鼠标右键点击三维球中心点，在弹出的右键菜单中选择点到点功能，再拾取另一个模型上的两个非重合点使两个模型实现装配，如图2.11所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image18.png)
图2.11：点到点示例

1. 到边的中点

到边的中点功能可以使和三维球绑定的模型移动至另一个模型选定边的中心位置。

选中模型之后激活三维球，鼠标右键点击三维球中心点，在弹出的右键菜单中选择到边的中点功能，之后于指定模型上一条可拾取的边，从而实现两个模型的装配，如图2.12所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image19.png)
图2.12：到边的中点示例

1. Z向垂直到点

Z向垂直到点可以使和三维球绑定的模型快速移动至另一个模型的指定点所在平面上，且保证模型三维球的Z向垂直于指定点所在平面（指定点只能拾取平面内的某个点，不能拾取平面边线上的点位）。

选中模型之后激活三维球，鼠标右键点击三维球中心点，在弹出的右键菜单中选择Z向垂直到点功能，拾取另一个模型相应平面上的一个点，使模型快速移动并垂直于拾取的平面，如图2.13所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image20.png)
图2.13：Z向垂直到点示例

1. 到面中点

到面中点可以使和三维球绑定的模型移动至另一个模型所选面的中心位置上。

选中模型之后激活三维球，鼠标右键点击三维球中心点，在弹出的右键菜单中选择到面中点功能，拾取另一个模型的一个面即可使三维球中心点移动至所选面的中心位置，如图2.14所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image21.png)
图2.14：到面的中点示例

轴控制方式

三维球的轴控制包含了平移轴和旋转轴两种不同的方式，但一般情况下，我们只要对平移轴进行编辑处理即可，无需对旋转轴进行编辑操作，轴控制主要是用于调整三维球的姿态，鼠标右键点击其中一个轴，即可弹出右键菜单，如图2.15所示，轴控制方式主要包括编辑位置、到点、到中心点、与边平行、与面垂直、与轴平行、反向、点到点、到边的中点、平移和旋转总计十一种不同的编辑方式，选择其中相应的功能实现对三维球不同的姿态控制。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image22.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image23.png)
图2.15：轴控制菜单               图2.16：编辑位置示例

1. 编辑位置

编辑位置功能可以通过数值控制的方式快速调整三维球的姿态。

选中模型之后激活三维球，鼠标右键点击三维球其中一坐标轴，在弹出的菜单中选择编辑位置功能，在弹出的带文本输入框的编辑位置对话框中输入X、Y、Z相应的数值即可使三维球选定的轴快速指向对应的确定的方向。如图2.16所示。

注：输入的X、Y、Z数值表示的是每个轴基于世界坐标系XYZ的向量，输入数值确定后可以改变轴在世界坐标系下的朝向。

1. 到点

到点功能可以使三维球中被选择的轴指向场景中某一模型上选定的点。

选中模型之后激活三维球，通过鼠标右键点击三维球其中一坐标轴，在弹出的菜单中选择到点功能，再选中另一模型上的某个点，三维球该轴便可指向模型的选定点方向，如图2.17所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image24.png)
图2.17：到点示例

1. 到中心点

到中心点可以使三维球中被选择的轴指向场景中某一回转体模型的中心点，既可以捕捉回转体模型的边，也可以捕捉模型的面。

选中模型之后激活三维球，通过鼠标右键点击三维球某一轴，在弹出的菜单中选择到中心点功能，通过拾取回转体的边或面来实现。如图2.18所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image25.png)
图2.18：到中心点示例

1. 与边平行

与边平行可以使三维球中被选择的轴与场景中某一模型的某条边平行。

选中模型之后激活三维球，通过鼠标右键点击三维球某一轴，在弹出的菜单中选择与边平行，通过拾取模型的某条边来实现。如图2.19所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image26.png)
图2.19：与边平行示例

1. 与面垂直

与面垂直可以使三维球中被选择的轴与场景中某一模型的某个面垂直。

选中模型之后激活三维球，通过鼠标右键点击三维球某一轴，在弹出的菜单中选择与面垂直，通过拾取回转体的面来实现。如图2.20所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image27.png)
图2.20：与面垂直示例

1. 与轴平行

与轴平行可以使三维球中被选择的轴与场景中某一模型的某根轴平行。

选中模型之后激活三维球，通过鼠标右键点击三维球某一轴，在弹出的菜单中选择与轴平行，通过拾取回转体的轴来实现。如图2.21所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image28.png)
图2.21：与轴平行示例

1. 反向

反向可以使三维球中被选择的轴指向方向反转。

选中模型之后激活三维球，通过鼠标右键点击三维球某一轴，在弹出的菜单中选择反向功能，则该轴方向翻转。如图2.22所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image29.png)
图2.22：反向示例

1. 点到点

点到点可以使得三维球中被选择的轴指向场景中某一模型上指定两非重合点连线的中心位置处。

选中模型之后激活三维球，通过鼠标右键点击三维球某一轴，在弹出的菜单中选择点到点功能，再拾取另一个模型上的两个非重合点，则实现模型位置的调整，如图2.23所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image30.png)
图2.23：点到点示例

1. 到边的中点

到边的中点可以使得三维球中被选择的轴指向场景中某一模型上某条边的中点。

选中模型之后激活三维球，通过鼠标右键点击三维球某一轴，在弹出的菜单中选择到边的中点，通过拾取回转体的边来实现。如图2.24所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image31.png)
图2.24：到边的中点示例

1. 平移

平移可以使得三维球中被选择的轴在场景中按轴方向平移指定距离。

选中模型之后激活三维球，通过鼠标右键点击三维球某一轴，在弹出的菜单中选择平移，在文本框中输入数值，则三维球平移相应数值距离。如图2.25所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image32.png)
图2.25：平移示例

注：当输入的数值为正时，三维球将朝该轴指向的方向平移，当输入的数值为负时，三维球将朝该轴指向方向的反向平移。

1. 旋转

旋转可以使得三维球绕被选择的轴在场景中翻转指定角度。

选择旋转后在文本框中输入角度值，则三维球旋转相应角度。选中模型之后激活三维球，通过鼠标右键点击三维球某一轴，在弹出的菜单中选择旋转，在文本框中输入角度值，则三维球旋转相应角度。如图2.26所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image33.png)
图2.26：旋转示例

注：当输入的数值为正时，三维球将朝箭头指向的方向旋转，当输入的数值为负时，三维球将朝箭头指向方向的反向旋转。
##### 应用案例

为方便用户对案例的查看熟悉，PQArt为用户提供了“应用案例”云端库，案例库中包含大量仿真案例，用户可通过点击案例库中不同仿真案例的下载按钮，将案例工作站导入绘图区进行仿真查看， 如图2.27所示。

同样应用案例库支持通过应用场景和关键字进行搜索，还可按综合、使用量的方式进行排序。同时，库中的应用案例也可以进行缓存，当其被下载过一次之后便可被缓存到本地，之后，下载按钮也会变为插入按钮，点击工作站图片可打开详情页查看工作站参数。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image34.png)
图2.27：应用案例
##### 机器人库

位置：编程仿真-场景搭建-机器人库，如图2.28所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image35.png)
图2.28：功能位置

功能说明：如图2.29所示，用于导入官方提供的工业机器人、导轨以及变位机。机器人库提供了大量不同品牌不同信号的机器人，包含ABB、KUKA、Fanuc、YASKAWA等，可通过点击【下载\插入】按钮将机器人导入到绘图区当中使用。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image36.png)
图2.29：“选择机器人”界面
#### *列表中涵盖了众多市场上流行的机器人品牌，如ABB，KUKA等。
#### 插入官方机器人模型：单击“下载/插入”按钮即可插入机器人模型；单击机器人图片，可查看机器人的具体参数，包括轴数、负载、工作区域等，同时“看了又看”中推荐出相似参数的机器人型号
#### 本界面采用网页形式，支持机器人品牌、型号的筛选、搜索和排序。
##### 工具库

位置：编程仿真-场景搭建-工具库，如图2.30所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image35.png)
图2.30：功能位置

用于导入官方提供的工具，如图2.31所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image37.png)
图2.31：“选择工具库”界面

功能说明：用于导入软件提供的非标工具，也支持按照一定方式进行排序和搜索，如图2.31所示。在PQArt软件中将所有的工具分为了三大类，包括法兰工具、快换工具以及外部工具，其中法兰工具表示直接安装在机器人法兰末端的工具，快换工具一般为安装在法兰工具上的需要频繁更换的工具，外部工具是无需安装在机器人本体上的工具。工具可通过不同分类和关键字的方式来进行搜索，可通过综合以及使用量来进行排序。
##### 设备库

位置：编程仿真-场景搭建-设备库，如图2.32所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image35.png)
图2.32：功能位置

功能说明：如图2.33所示，为方便用户快速进行场景搭建，设备库提供了大量的场景设备，用户可根据需求自由导入设备库中的零件、传感器、PLC、触摸屏、状态机、底座等设备，其中，零件包括场景零件和加工零件。场景零件用来搭建工作环境，加工零件是机器人加工的对象。设备库同样支持按照分类和关键字来进行搜索，以及按照综合和使用量来进行排序。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image38.png)
图2.33：“选择设备库”界面
##### 输入

位置：定义组件-场景-输入/编程仿真-场景搭建-输入，如图2.34所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image35.png)
图2.34：功能位置

功能说明：输入功能是将本地模型导入PQArt，通过这个功能，用户可以方便地将自己已有的模型文件导入到软件中，以便后续的处理与使用。PQArt支持多种不同的三维模型中间格式，包含*.obj、*.brep、*.bms、*.igs、*.jt、*.off、*.pq3d、*.ply、*.stp、*.stl等三维格式，支持多种格式的文件导入到PQArt环境中。如图2.35所示目前支持的格式包括：

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image39.png)
图2.35：PQArt支持的模型格式

*列表中涵盖了众多市场上流行的3D绘图软件所制作的模型格式，如CATIA，Solidworks等。
##### 贴图

位置：编程仿真-场景搭建-贴图，如图2.36所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image40.png)
图2.36：功能位置

功能说明：用于给三维模型贴图，可将图片贴到模型的表面，使模型看起来更加美观真实，支持bmp、jpg、tif、jpeg格式的图片，并可通过旋转角度和镜像来修改图片的方向。

点击贴图，可以在软件左边看到贴图面板。贴图面板分为“元素”和“属性”两部分。在“元素”部分选择进行贴图的模型表面，以及用于贴图的图像文件。在“属性”部分对图像进行微调。如图2.37所示。

选择模型表面：勾选“添加/修改”后可以在绘图区中选择想要贴图的面，勾选“删除”可以剔除错选的面。

选择图像文件：点击按钮，在电脑磁盘中选择用于贴图的图像文件。文件格式可为bmp、jpg、tif、jpeg。

更改图像属性：贴图时，图像可旋转任意角度或镜像。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image43.png)
图2.37：贴图面板
##### 测量

位置：编程仿真-场景搭建-测量，如图2.38所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image35.png)
图2.38：功能位置

功能说明：对场景内模型的点、线、面进行有关间距、口径和角度等的测量，测出的结果可以在绘图区和从“测量结果”栏中查看。
##### 新建坐标系

位置：编程仿真-场景搭建-新建坐标系，如图2.39所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image35.png)
图2.39：功能位置

功能说明：可根据输入的参数或获取的特征点生成用户自定义的坐标系，并且支持坐标系预览功能查看预览效果，如图2.40所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image44.png)
图2.40：新建坐标系

生成的坐标系支持编辑功能，通过鼠标右键点击用户坐标系节点下的坐标系名称，在“编辑”功能框可基于其他的坐标系修改参数，在“属性”功能框中可选择绑定的模型，绑定之后移动其中一个元素，另一个也会随之移动。
##### 网格平滑

位置：编程仿真-场景搭建-网格平滑，如图2.41所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image35.png)
图2.41：功能位置

导入文件，如图2.42，在左侧菜单栏中，勾选仅选择，点击添加，在工件正面圈出需要平滑的区域，被选中的区域变红，点击确定，完成平滑处理，如图2.43所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image45.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image46.png)
图2.42：选择添加                        图2.43：待处理区域
##### 裁剪网格

位置：编程仿真-场景搭建-裁剪网络，如图2.44所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image35.png)
图2.44：功能位置

如图2.45及2.46所示，导入文件，选中文件后出现“小剪刀”图标，在模型上根据需求裁剪相应的部分，右键选择切割形式，点击确定，完成裁剪。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image47.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image48.png)
图2.45：切割选取示例                       图2.46：切割形式
### 轨迹规划
##### 生成轨迹
#### 位置：位于【编程仿真】下的【生成轨迹】中，如图2.47所示。。
#### 图2.47: 功能位置

用于生成机器人工作的轨迹，即机器人运动的路径。

“类型”用于指定机器人生成轨迹的方式，通过拾取模型中的点、线、面特征，输入相关的参数生成所需的加工轨迹。为了应对不同的应用场景，如图2.48所示，十种生成轨迹的方式：沿着一个面的一条边；面的一个环；面的环；曲线特征；边；点云打孔；打孔；截面线；面夹边；沿着零件边界的一条边。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image50.png)
图2.48：10种生成轨迹方式

（1）沿着一个面的一条边

1.功能说明：通过一条边，加上其轨迹方向（箭头），再加上轨迹Z轴指向的平面来确定轨迹。即拾取一条边和这条边相邻的面，沿着这条边进一步搜索其他的边来生成轨迹，如图2.49，2.50，2.51所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image51.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image52.png)
图2.49：沿着一个面的一条边（上）       图2.50：沿着一个面的一条边（中）

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image53.png)
图2.51：沿着一个面的一条边（下）

2.选择工具与TCP:

a.使用的工具，选择时要注意是机器人手持工具还是手持工件，机器人手持工件时，就需要用到外部工具。生成轨迹时要注意到底是需要哪个TCP来进行工作。

b.关联TCP，一个工具上有时会含有多个TCP，生成轨迹时要注意需要用到哪个TCP来生成，要选择生成轨迹时相对应的TCP，如图2.52所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image54.png)
图2.52：多TCP工具

3.拾取元素:

a.线和面需要相邻，即选择的线必须在选择的面上，如果线不在面上就会报错。

b.必经边的含义就是必须要经过所选择的边，前提是这条边必须在所选择的面上，否则是不会有反应的，如图2.53，54所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image55.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image56.png)
图2.53：未选必经边                         图2.54：选取必经边

4.搜索终止条件：

终止点是指轨迹终止于此点的位置，如图2.55所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image57.png)
图2.55：选取终止条件

5.设置：

a.反转是指选取的边的方向反转，从而使轨迹生成的方向沿着这条边往另一个方向搜索其他的边。

b.Z向与侧面平行就是让生成轨迹后，轨迹点的Z轴与轨迹侧面是平行的，如图2.56所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image58.png)
图2.56：Z向与侧面平行

c.垂直于面：生成轨迹后，轨迹点z轴的方向与所选中的面垂直

d.平行于面：生成轨迹后，轨迹点z轴的方向与所选中的面平行

e.侧面的角平分线：生成轨迹后，轨迹点z轴为所选中的面与侧面夹角的角平分线上。

6.轨迹参数：

a.点步长是指两个轨迹点之间的长度，同一条轨迹点步长的数值越小，轨迹点的数量就会越多。

b.仅为直线生成首末点是指当一条边为直线时，生成轨迹时只会在直线的首点和末点生成两个轨迹点，如图2.57所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image60.png)
图2.57：仅为直线生成首末点

c.不考虑连接点是指在两条边的连接处的位置只考虑步长，不用必须在连接位置生成轨迹点；连接处生成一个点是指在两条边连接的位置需要生成一个轨迹点；连接处生成两个点是指在两条边连接的位置需要生成两个轨迹点。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image61.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image62.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image63.png)
图2.58：不考虑连接点   图2.59:连接处生成一个点  图2.60：连接处生成两个点

d.仅为圆弧生成三个点是指当选中的边是圆弧的时候，生成轨迹时只会在圆弧上生成三个轨迹点。（用这种方法会生成MoveC指令）

e.为样条线生成圆弧点是指将样条线强行整合成圆弧，并且生成圆弧的三个点。圆周角阈值是控制圆弧的弧度的值，其默认值为150，如图2.61所示。

整合圆周角阈值整合圆周角阈值

图2.61：为样条生成圆弧点

f.Y轴与切向一致是指生成轨迹后轨迹点的y轴与轨迹的切线方向一致。

7.轨迹后处理：

操作可以选择无和z轴旋转最小，Z轴旋转最小是指在Z轴不变的前提下，使x、y轴的变化是最小的，这种变化都是基于第一个加工的点来说的，从图中可以看出，x、y轴的指向基本上是不变的。这是为了尽可能使6轴的旋转最小，从而防止轴超限的现象发生。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image64.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image65.png)
图2.62：z轴旋转最小（前）  图2.63：z轴旋转最小（后）

1. 面的一个环

1.功能说明：拾取一个面和这个面上的一条边，生成一个封闭环的轨迹。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image66.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image67.png)
图2.64：面的一个环（上）          图2.65：面的一个环（下）

2.选择工具和TCP：

a.使用的工具，选择时要注意是机器人手持工具还是手持工件，机器人手持工件时，就需要用到外部工具。生成轨迹时要注意到底是需要哪个TCP来进行工作。

b.关联TCP，一个工具上有时会含有多个TCP，生成轨迹时要注意需要用到哪个TCP来生成，要选择生成轨迹时相对应的TCP，如图2.66所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image54.png)
图2.66：多TCP工具

3.拾取元素：

拾取的线必须在拾取的面上，否则就会出现提示。

4.设置：

a.反转是指选取的边的方向反转，从而使轨迹生成的方向沿着这条边往另一个方向搜索其他的边。

b.Z向与侧面平行就是让生成轨迹后，轨迹点的Z轴与轨迹侧面是平行的。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image58.png)
图2.67：Z向与侧面平行

c.垂直于面：生成轨迹后，轨迹点z轴的方向与所选中的面垂直

d.平行于面：生成轨迹后，轨迹点z轴的方向与所选中的面平行

e.侧面的角平分线：生成轨迹后，轨迹点z轴为所选中的面与侧面夹角的角平分线上。

5.轨迹参数：

a.点步长是指两个轨迹点之间的长度，同一条轨迹点步长的数值越小，轨迹点的数量就会越多。

b.仅为直线生成首末点是指当一条边为直线时，生成轨迹时只会在直线的首点和末点生成两个轨迹点。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image60.png)
图2.68：仅为直线生成首末点

c.不考虑连接点是指在两条边的连接处的位置只考虑步长，不用必须在连接位置生成轨迹点；连接处生成一个点是指在两条边连接的位置需要生成一个轨迹点；连接处生成两个点是指在两条边连接的位置需要生成两个轨迹点。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image61.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image62.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image63.png)
图2.69：不考虑连接点   图2.70:连接处生成一个点  图2.71：连接处生成两个点

d.仅为圆弧生成三个点是指当选中的边是圆弧的时候，生成轨迹时只会在圆弧上生成三个轨迹点。（用这种方法会生成MoveC指令）

e.为样条线生成圆弧点是指将样条线强行整合成圆弧，并且生成圆弧的三个点。圆周角阈值是控制圆弧的弧度的值，其默认值为150，如图2.72所示。

整合圆周角阈值整合圆周角阈值

图2.72：为样条生成圆弧点

f.Y轴与切向一致是指生成轨迹后轨迹点的y轴与轨迹的切线方向一致。

6.轨迹后处理：

操作可以选择无和z轴旋转最小，Z轴旋转最小是指在Z轴不变的前提下，使x、y轴的变化是最小的，这种变化都是基于第一个加工的点来说的，从图中可以看出，x、y轴的指向基本上是不变的。这是为了尽可能使6轴的旋转最小，从而防止轴超限的现象发生。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image64.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image65.png)
图2.73：z轴旋转最小（前）  图2.74：z轴旋转最小（后）

1. 面的环

1.功能说明：

选择一个面，在这个面的外环上生成轨迹。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image68.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image69.png)
图2.75：面的一个环（上）             图2.76：面的一个环（中）

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image70.png)
图2.77 ：面的一个环（下）

2.选择工具和TCP：

a.使用的工具，选择时要注意是机器人手持工具还是手持工件，机器人手持工件时，就需要用到外部工具。生成轨迹时要注意到底是需要哪个TCP来进行工作。

b.关联TCP，一个工具上有时会含有多个TCP，生成轨迹时要注意需要用到哪个TCP来生成，要选择生成轨迹时相对应的TCP，如图2.78所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image54.png)
图2.78：多TCP工具

3.拾取元素

面可以多选，但必须在一个机器人上。

拾取面的元素包括面的内环，外环，所有环，面的内环需设置相关参数，如图2.79所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image71.png)
图2.79：内环的参数设置

4.设置

a.反转是指选取的边的方向反转，从而使轨迹生成的方向沿着这条边往另一个方向搜索其他的边。

b.Z向与侧面平行就是让生成轨迹后，轨迹点的Z轴与轨迹侧面是平行的。

c.垂直于面：生成轨迹后，轨迹点z轴的方向与所选中的面垂直

d.平行于面：生成轨迹后，轨迹点z轴的方向与所选中的面平行

e.侧面的角平分线：生成轨迹后，轨迹点z轴为所选中的面与侧面夹角的角平分线上。

5.轨迹参数

起点/终点内偏

a.点步长是指两个轨迹点之间的长度，同一条轨迹点步长的数值越小，轨迹点的数量就会越多。

b.仅为直线生成首末点是指当一条边为直线时，生成轨迹时只会在直线的首点和末点生成两个轨迹点，如图2.80所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image60.png)
图2.80：仅为直线生成首末点

c.不考虑连接点是指在两条边的连接处的位置只考虑步长，不用必须在连接位置生成轨迹点；连接处生成一个点是指在两条边连接的位置需要生成一个轨迹点；连接处生成两个点是指在两条边连接的位置需要生成两个轨迹点。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image61.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image62.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image63.png)
图2.81：不考虑连接点     图2.82:连接处生成一个点    图2.83：连接处生成两个点

d.仅为圆弧生成三个点是指当选中的边是圆弧的时候，生成轨迹时只会在圆弧上生成三个轨迹点。（用这种方法会生成MoveC指令）

e.为样条线生成圆弧点是指将样条线强行整合成圆弧，并且生成圆弧的三个点。圆周角阈值是控制圆弧的弧度的值，其默认值为150，如图2.84所示。                                  整合圆周角阈值整合圆周角阈值

图2.84：为样条生成圆弧点

f.Y轴与切向一致是指生成轨迹后轨迹点的y轴与轨迹的切线方向是一致的。

轨迹后处理：

操作可以选择无和z轴旋转最小，Z轴旋转最小是指在Z轴不变的前提下，使x、y轴的变化是最小的，这种变化都是基于第一个加工的点来说的，从图中可以看出，x、y轴的指向基本上是不变的。这是为了尽可能使6轴的旋转最小，从而防止轴超限的现象发生。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image64.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image65.png)
图2.85：z轴旋转最小（前）          图2.86：z轴旋转最小（后）

1. 曲线特征

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image72.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image73.png)
图2.87：曲线特征（上）               图2.88：曲线特征（下）

1.功能说明：拾取上面的曲线，拾取一个面或者一个零件/装配。

*这种曲线是3D曲线，和前面拾取的零件上的边有所不同。

2.选择工具和TCP：

a.使用的工具，选择时要注意是机器人手持工具还是手持工件，机器人手持工件时，就需要用到外部工具。生成轨迹时要注意到底是需要哪个TCP来进行工作。

b.关联TCP，一个工具上有时会含有多个TCP，生成轨迹时要注意需要用到哪个TCP来生成，要选择生成轨迹时相对应的TCP，如图2.89所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image54.png)
图2.89：多TCP工具

3.拾取元素：

拾取的曲线需要在面或者零件/装配上，可以单独拾取面和零件/装配，也可以同时拾取面和零件/装配。

4.设置：

a.反转是指选取的边的方向反转，从而使轨迹生成的方向沿着这条边往另一个方向搜索其他的边。

b.合并轨迹是将生成的所有轨迹合并成一条轨迹，如果不勾选的话有时候曲线不连续，会生成好几条轨迹。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image74.png)
图2.90：合并轨迹（前）

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image75.png)
图2.91：合并轨迹（后）

5.轨迹参数：

a.点步长是指两个轨迹点之间的长度，同一条轨迹点步长的数值越小，轨迹点的数量就会越多。

b.仅为直线生成首末点是指当一条边为直线时，生成轨迹时只会在直线的首点和末点生成两个轨迹点，如图2.92所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image60.png)
图2.92：仅为直线生成首末点

c.不考虑连接点是指在两条边的连接处的位置只考虑步长，不用必须在连接位置生成轨迹点；连接处生成一个点是指在两条边连接的位置需要生成一个轨迹点；连接处生成两个点是指在两条边连接的位置需要生成两个轨迹点。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image61.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image62.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image63.png)
图2.93：不考虑连接点     图2.94:连接处生成一个点    图2.95：连接处生成两个点

d.仅为圆弧生成三个点是指当选中的边是圆弧的时候，生成轨迹时只会在圆弧上生成三个轨迹点。（用这种方法会生成MoveC指令）

e.为样条线生成圆弧点是指将样条线强行整合成圆弧，并且生成圆弧的三个点。圆周角阈值是控制圆弧的弧度的值，其默认值为150，如图2.96所示。                                  整合圆周角阈值整合圆周角阈值

图2.96：为样条生成圆弧点

f.Y轴与切向一致是指生成轨迹后轨迹点的y轴与轨迹的切线方向是一致的。

6.轨迹后处理：

操作可以选择无和z轴旋转最小，Z轴旋转最小是指在Z轴不变的前提下，使x、y轴的变化是最小的，这种变化都是基于第一个加工的点来说的，从图中可以看出，x、y轴的指向基本上是不变的。这是为了尽可能使6轴的旋转最小，从而防止轴超限的现象发生。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image64.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image65.png)
图2.97：z轴旋转最小（前）            图2.98：z轴旋转最小（后）

1. 边

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image76.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image77.png)
图2.99：边（上）                     图2.100：边（下）

1.功能说明：拾取零件或装配上的一条边，再拾取一个面，拾取的面可以和边相邻也可以不相邻，但是必须在同一个零件上。

2.选择工具和TCP：

a.使用的工具，选择时要注意是机器人手持工具还是手持工件，机器人手持工件时，就需要用到外部工具。生成轨迹时要注意到底是需要哪个TCP来进行工作。

b.关联TCP，一个工具上有时会含有多个TCP，生成轨迹时要注意需要用到哪个TCP来生成，要选择生成轨迹时相对应的TCP，如图2.101所示。。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image54.png)
图2.101：多TCP工具

3.拾取元素：

拾取的边可以个选择的面相邻也可以不相邻，但是必须是同一个零件上的，否则就会出现提示。

4.设置：

a.反转是指选取的边的方向反转，从而使轨迹生成的方向沿着这条边往另一个方向搜索其他的边。

b.Z向与侧面平行就是让生成轨迹后，轨迹点的Z轴与轨迹侧面是平行的，如图2.102所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image58.png)
图2.102：Z向与侧面平行

c.垂直于面：生成轨迹后，轨迹点z轴的方向与所选中的面垂直

d.平行于面：生成轨迹后，轨迹点z轴的方向与所选中的面平行

e.侧面的角平分线：生成轨迹后，轨迹点z轴为所选中的面与侧面夹角的角平分线上。

5.轨迹参数：

a.点步长是指两个轨迹点之间的长度，同一条轨迹点步长的数值越小，轨迹点的数量就会越多。

b.仅为直线生成首末点是指当一条边为直线时，生成轨迹时只会在直线的首点和末点生成两个轨迹点，如图2.103所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image60.png)
图2.103：仅为直线生成首末点

c.不考虑连接点是指在两条边的连接处的位置只考虑步长，不用必须在连接位置生成轨迹点；连接处生成一个点是指在两条边连接的位置需要生成一个轨迹点；连接处生成两个点是指在两条边连接的位置需要生成两个轨迹点。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image61.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image62.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image63.png)
图2.104：不考虑连接点    图2.105:连接处生成一个点   图2.106：连接处生成两个点

d.仅为圆弧生成三个点是指当选中的边是圆弧的时候，生成轨迹时只会在圆弧上生成三个轨迹点。（用这种方法会生成MoveC指令）

e.为样条线生成圆弧点是指将样条线强行整合成圆弧，并且生成圆弧的三个点。圆周角阈值是控制圆弧的弧度的值，其默认值为150，如图2.107所示。                                  整合圆周角阈值整合圆周角阈值

图2.107：为样条生成圆弧点

f.Y轴与切向一致是指生成轨迹后轨迹点的y轴与轨迹的切线方向是一致的。

6.轨迹后处理：

操作可以选择无和z轴旋转最小，Z轴旋转最小是指在Z轴不变的前提下，使x、y轴的变化是最小的，这种变化都是基于第一个加工的点来说的，从图中可以看出，x、y轴的指向基本上是不变的。这是为了尽可能使6轴的旋转最小，从而防止轴超限的现象发生。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image64.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image65.png)
图2.108：z轴旋转最小（前）             图2.109：z轴旋转最小（后）

1. 点云打孔

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image78.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image79.png)
图2.110：点云打孔（上）                     图2.111：点云打孔（下）

1.功能说明：

通过拾取点云数据、参照面等，生成轨迹的一种打孔方式。

2.选择工具和TCP：

a.使用的工具，选择时要注意是机器人手持工具还是手持工件，机器人手持工件时，就需要用到外部工具。生成轨迹时要注意到底是需要哪个TCP来进行工作。

b.关联TCP，一个工具上有时会含有多个TCP，生成轨迹时要注意需要用到哪个TCP来生成，要选择生成轨迹时相对应的TCP，如图2.112所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image54.png)
图2.112：多TCP工具

3.拾取元素：

拾取点云、面、零件/装配，并设置相应的孔深，按照需求选择是否添加一组点。

是否添加一组点：选中其中一个点，勾选后，即可自动选中模型内所有点。

4.设置：

在机器人直接打孔的方式中，设置工具的出入刀偏移量为生成的往复路径值，并根据打孔需求设置相应的孔深。

5.轨迹后处理：

操作可以选择无和z轴旋转最小，Z轴旋转最小是指在Z轴不变的前提下，使x、y轴的变化是最小的，这种变化都是基于第一个加工的点来说的，从图中可以看出，x、y轴的指向基本上是不变的。这是为了尽可能使6轴的旋转最小，从而防止轴超限的现象发生。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image64.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image65.png)
图2.113：z轴旋转最小（前）              图2.114：z轴旋转最小（后）

1. 打孔

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image80.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image81.png)
图2.115：打孔（上）                         图2.116：打孔（下）

1.功能说明：拾取孔边，生成带工具偏移和孔深信息的打孔轨迹。

2.选择工具和TCP：

a.使用的工具，选择时要注意是机器人手持工具还是手持工件，机器人手持工件时，就需要用到外部工具。生成轨迹时要注意到底是需要哪个TCP来进行工作。

b.关联TCP，一个工具上有时会含有多个TCP，生成轨迹时要注意需要用到哪个TCP来生成，要选择生成轨迹时相对应的TCP，如图2.117所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image54.png)
图2.117：多TCP工具

3.拾取元素：

选择边或面，拾取孔边，并设置拟合圆弧容差和孔深的参数。

拾取面时，可支持一次性拾取多个，同时完成多个孔的轨迹生成。

反转：z轴反向，工具从下向上进行打孔。

孔深：根据需求设置打孔的深度。

4.设置：

在机器人直接打孔的方式中，设置工具的出入刀偏移量为生成的往复路径值，并根据打孔需求设置相应的孔深。

5.轨迹后处理：

操作可以选择无和z轴旋转最小，Z轴旋转最小是指在Z轴不变的前提下，使x、y轴的变化是最小的，这种变化都是基于第一个加工的点来说的，从图中可以看出，x、y轴的指向基本上是不变的。这是为了尽可能使6轴的旋转最小，从而防止轴超限的现象发生。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image64.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image65.png)
图2.118：z轴旋转最小（前）             图2.119：z轴旋转最小（后）

1. 截面线

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image82.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image83.png)
图2.120：截面线（上）                图2.121：截面线（中）

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image84.png)
图2.122 ：截面线（下）

1.功能说明：选取一条引导线或者引导面，再选取需要的实体或者表面，通过生成的虚拟截面与实际表面相交形成的交线来生成轨迹。

2.选择工具和TCP：

a.使用的工具，选择时要注意是机器人手持工具还是手持工件，机器人手持工件时，就需要用到外部工具。生成轨迹时要注意到底是需要哪个TCP来进行工作。

b.关联TCP，一个工具上有时会含有多个TCP，生成轨迹时要注意需要用到哪个TCP来生成，要选择生成轨迹时相对应的TCP，如图2.123所示。

图123：多TCP工具

3.拾取元素：

拾取的引导线可以是实体的边也可以是3D曲线，引导线可以不必在零件之上。勾选引导线方向反转后，引导线的头和尾会反转，如下图。同时截面线可以拾取面也可以拾取实体（勾选与实体求交）。

图124：引导线反转前                  图2.125：引导线反转后

参考平面：通过参考平面可在截面线生成轨迹时，控制虚拟截面和参考平面相平行，进而修改截面轨迹的生成方式。

截面间距：实现对截面线间距的交替要求，新增交替间距参数设置，可以设置两个不同的间距，使截面间距交替排列。

截面个数：是指生成的虚拟截面的个数。

起始距离：是指沿着引导线或引导面的起点开始一直到生成第一个截面的距离。

截面距离：每个虚拟截面之间的距离。

起始过盈：起始方向一侧多出来的距离。

终止过盈：终止方向一侧多出来的距离。

横向生成轨迹：改变生成的轨迹点的链接方式。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image87.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image88.png)
图2.126：非横向生成轨迹               图2.127：横向生成轨迹

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image89.png)
图2.128：截面线拾取元素

4.轨迹参数：

a.点步长是指两个轨迹点之间的长度，同一条轨迹点步长的数值越小，轨迹点的数量就会越多。

b.仅为直线生成首末点是指当一条边为直线时，生成轨迹时只会在直线的首点和末点生成两个轨迹点，如图2.129所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image60.png)
图2.129：仅为直线生成首末点

c.不考虑连接点是指在两条边的连接处的位置只考虑步长，不用必须在连接位置生成轨迹点；连接处生成一个点是指在两条边连接的位置需要生成一个轨迹点；连接处生成两个点是指在两条边连接的位置需要生成两个轨迹点。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image61.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image62.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image63.png)
图2.130：不考虑连接点  图2.131：连接处生成一个点 图2.132：连接处生成两个点

d.仅为圆弧生成三个点是指当选中的边是圆弧的时候，生成轨迹时只会在圆弧上生成三个轨迹点。（用这种方法会生成MoveC指令）

e.为样条线生成圆弧点是指将样条线强行整合成圆弧，并且生成圆弧的三个点。圆周角阈值是控制圆弧的弧度的值，其默认值为150。                                  整合圆周角阈值整合圆周角阈值

图2.133：为样条生成圆弧点

f.Y轴与切向一致是指生成轨迹后轨迹点的y轴与轨迹的切线方向是一致的。

g.隐藏截面是指可以将生成的虚拟截面隐藏起来。

h.统一截面姿态是指使各个虚拟截面按照同一个姿态来排列。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image90.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image91.png)
图2.134：统一截面姿态前             图2.135：统一截面姿态后

i.编辑截面可以通过激活的三维球更改所选择的截面位姿。

j.截面长度和宽度：可以设置更改虚拟截面的长和宽。

5.轨迹后处理：

操作可以选择无和z轴旋转最小，Z轴旋转最小是指在Z轴不变的前提下，使x、y轴的变化是最小的，这种变化都是基于第一个加工的点来说的，从图中可以看出，x、y轴的指向基本上是不变的。这是为了尽可能使6轴的旋转最小，从而防止轴超限的现象发生。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image64.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image65.png)
图2.136：z轴旋转最小（前）          图2.137：z轴旋转最小（后）

1. 面夹边

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image92.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image93.png)
图2.138：面夹边（上）                  图2.139：面夹边（下）

1.功能说明：在生成轨迹的过程中，其他的生成类型只能在同一个零件下生成。对于一些焊接的项目中，可能需要将两个焊接的零件焊接到一起，此功能可以方便用户在不同零件下，生成对应的轨迹。

2.选择工具和TCP：

a.使用的工具，选择时要注意是机器人手持工具还是手持工件，机器人手持工件时，就需要用到外部工具。生成轨迹时要注意到底是需要哪个TCP来进行工作。

b.关联TCP，一个工具上有时会含有多个TCP，生成轨迹时要注意需要用到哪个TCP来生成，要选择生成轨迹时相对应的TCP，如图2.140所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image54.png)
图2.140：多TCP工具

3.拾取元素：

连续的边和周围的面/侧面。

4.设置：

反转是指选取的边的方向反转，从而使轨迹生成的方向沿着这条边往另一个方向搜索其他的边。

5.轨迹参数：

a.点步长是指两个轨迹点之间的长度，同一条轨迹点步长的数值越小，轨迹点的数量就会越多。

b.仅为直线生成首末点是指当一条边为直线时，生成轨迹时只会在直线的首点和末点生成两个轨迹点，如图2.141所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image60.png)
图2.141：仅为直线生成首末点

c.不考虑连接点是指在两条边的连接处的位置只考虑步长，不用必须在连接位置生成轨迹点；连接处生成一个点是指在两条边连接的位置需要生成一个轨迹点；连接处生成两个点是指在两条边连接的位置需要生成两个轨迹点。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image61.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image62.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image63.png)
图2.142：不考虑连接点   图2.143：连接处生成一个点 图2.144：连接处生成两个点

d.仅为圆弧生成三个点是指当选中的边是圆弧的时候，生成轨迹时只会在圆弧上生成三个轨迹点。（用这种方法会生成MoveC指令）

f.为样条线生成圆弧点是指将样条线强行整合成圆弧，并且生成圆弧的三个点。圆周角阈值是控制圆弧的弧度的值，其默认值为150，如图2.145所示。                                  整合圆周角阈值整合圆周角阈值

图2.145：为样条生成圆弧点

g.Y轴与切向一致是指生成轨迹后轨迹点的y轴与轨迹的切线方向是一致的。

6.轨迹后处理：

操作可以选择无和z轴旋转最小，Z轴旋转最小是指在Z轴不变的前提下，使x、y轴的变化是最小的，这种变化都是基于第一个加工的点来说的，从图中可以看出，x、y轴的指向基本上是不变的。这是为了尽可能使6轴的旋转最小，从而防止轴超限的现象发生。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image64.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image65.png)
图2.146：z轴旋转最小（前）           图2.147：z轴旋转最小（后）

（10）沿着零线边界的一条边

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image94.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image95.png)
图2.148：沿零件边界一条边（上）      图2.149：沿着零件边界一条边（下）

1.功能说明：

用于三角片状的模型生成轨迹，在生成轨迹的过程中，沿着零件边界的一条边实现轨迹的生成。

2.选择工具和TCP：

a.使用的工具，选择时要注意是机器人手持工具还是手持工件，机器人手持工件时，就需要用到外部工具。生成轨迹时要注意到底是需要哪个TCP来进行工作。

b.关联TCP，一个工具上有时会含有多个TCP，生成轨迹时要注意需要用到哪个TCP来生成，要选择生成轨迹时相对应的TCP，如图2.150所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image54.png)
图2.150：多TCP工具

3.拾取元素：

选中零件边界的一条边，生成沿着模型整个外轮廓的轨迹。

4.设置：

a.反转是指选取的边的方向反转，从而使轨迹生成的方向沿着这条边往另一个方向搜索其他的边。

b.Z向与侧面平行就是让生成轨迹后，轨迹点的Z轴与轨迹侧面是平行的。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image58.png)
图2.151：Z向与侧面平行

c.垂直于面：生成轨迹后，轨迹点z轴的方向与所选中的面垂直

d.平行于面：生成轨迹后，轨迹点z轴的方向与所选中的面平行

e.侧面的角平分线：生成轨迹后，轨迹点z轴为所选中的面与侧面夹角的角平分线上。

5.轨迹参数：

a.点步长是指两个轨迹点之间的长度，同一条轨迹点步长的数值越小，轨迹点的数量就会越多。

b.仅为直线生成首末点是指当一条边为直线时，生成轨迹时只会在直线的首点和末点生成两个轨迹点，如图2.152所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image60.png)
图2.152：仅为直线生成首末点

c.不考虑连接点是指在两条边的连接处的位置只考虑步长，不用必须在连接位置生成轨迹点；连接处生成一个点是指在两条边连接的位置需要生成一个轨迹点；连接处生成两个点是指在两条边连接的位置需要生成两个轨迹点。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image61.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image62.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image63.png)
图2.153：不考虑连接点  图2.154：连接处生成一个点 图2.155：连接处生成两个点

d.仅为圆弧生成三个点是指当选中的边是圆弧的时候，生成轨迹时只会在圆弧上生成三个轨迹点。（用这种方法会生成MoveC指令）

e.为样条线生成圆弧点是指将样条线强行整合成圆弧，并且生成圆弧的三个点。圆周角阈值是控制圆弧的弧度的值，其默认值为150，如图2.156所示。                                 整合圆周角阈值整合圆周角阈值

图2.156：为样条生成圆弧点

f.Y轴与切向一致是指生成轨迹后轨迹点的y轴与轨迹的切线方向是一致的。

6.轨迹后处理：

操作可以选择无和z轴旋转最小，Z轴旋转最小是指在Z轴不变的前提下，使x、y轴的变化是最小的，这种变化都是基于第一个加工的点来说的，从图中可以看出，x、y轴的指向基本上是不变的。这是为了尽可能使6轴的旋转最小，从而防止轴超限的现象发生。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image64.png)
![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image65.png)
图2.157：z轴旋转最小（前）            图2.158：z轴旋转最小（后）
##### AGV路径规划

位置：位于【编程仿真】下的【轨迹规划】中，如图2.159所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image96.png)
图2.159：功能位置

功能说明：用于给AGV小车、送餐机器人等智能运动设备生成运动轨迹的方式，通过拾取智能运动设备的路径轨迹，即可自动生成设备的路径。需要注意，导航轨迹需要基于3D曲线生成轨迹，因此要保证场景中含有设备运动的3D曲线路径。
##### 绝对关节指令

位置：位于【编程仿真】下的【轨迹规划】中，如图2.160所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image96.png)
图2.160：功能位置

功能说明：生成机器人的绝对关节运动指令，机器人以单轴运动的方式运动至目标点，不存在死点，运动状态完全不可控制，此点一般可以作为机器人回零。
##### 直线指令

位置：位于【编程仿真】下的【轨迹规划】中，如图2.161所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image96.png)
图2.161：功能位置

功能说明：生成机器人的直线运动指令，机器人线性运动方式至目标点，运动路径为当前点与目标点两点决定一条直线，运动路径唯一，常用于机器人在工作状态移动。
##### 关节指令

位置：位于【编程仿真】下的【轨迹规划】中，如图2.162所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image96.png)
图2.162：功能位置

功能说明：生成机器人的关节指令，机器人以最快捷的方式运动至目标点，机器人运动状态不完全可控，但运动路径唯一，常用于机器人在较大空间范围内移动。
##### 导入轨迹

位置：位于【轨迹规划】中，如图2.163所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image97.png)
图2.163：“导入轨迹”位置

功能说明：将其他软件/PQArt中生成的轨迹导入到PQArt中。软件支持的轨

迹格式有aptsource，nc等。

导入轨迹格式如图

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image98.png)
图2.164：轨迹格式
##### 新建轨迹

位置：位于【轨迹规划】中，如图2.165所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image97.png)
图2.165：新建程序位置

功能说明：单击【新建轨迹】后，会在左侧的【机器人加工管理】的机器人下的轨迹树上生成一个“新建轨迹”节点。从而方便后续生成的POS点，自动加入到该轨迹内。
##### 新建程序

位置：位于【轨迹规划】中，如图2.166所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image97.png)
图2.166：新建程序位置

功能说明：通过后置功能将机器人可执行的代码导入到示教器中，从而实现真机运行。该功能可以添加不同的加工轨迹程序。

*新建程序前需要插入一个机器人。

使用方法：点击【新建程序】，填写模块名称，然后单击【确定】。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image99.png)
图2.167：新建模块

生成空白的程序模板，可在空白区域编写程序。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image100.png)
图2.168：后置代码编辑器

后置代码编辑器界面介绍：

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image101.png)
图2.169：后置代码编辑器

后置代码的显示方式：点的坐标、字符和注释用不同颜色区别开来，代码查看起来清晰明了。

有行号显示，方便定位某一行的代码。

折叠功能，同一组别或者代码可以实现手动折叠展开和收起。

导出文件编码：包括ANSI和UTF-8两种编码。ANSI编码不支持代码程序中包含中文字符，UTF-8则允许包含中文字符，从而根据特定品牌的机器的后置需求来选择这两种编码。

下载：只应用ABB机器人，将程序直接下载到相连接的示教器上。

导出：将后置出的文件可拷贝到真实示教器，从而完成真机运行。

保存：编写的程序会自动保存加载到程序编辑器中和机器人加工管理树上。

取消：不保存已编写的程序且退出程序编辑器。

*后置格式的具体样式，如字体颜色、背景色、折叠方式等都用XML控制。因此，用户可根据实际需求，自定义后置的具体显示样式。
### 仿真调试
##### 编译

位置：位于【编程仿真】下的【仿真调试】中，如图2.170-所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image102.png)
图2.170：“编译”位置

功能说明：编译功能用来解析轨迹点状态。

轨迹点状态：

生成轨迹后，除了Move-AbsJoint点、抓取轨迹和放开轨迹外，其他轨迹点外均为灰色（未知状态）。只有【编译】【仿真】【单机构/多机构运动到点】三个指令可解析轨迹点状态，轨迹点由灰色更改为其他颜色。

*因为点Move-AbsJoint 是一个确定的点，确定了机器人的关节角度值，所以生成后它的状态可直接解析出来。

编译时绘图区会出现进度条，提示编译的进度。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image105.png)
图2.171：编译进度条

同时输出面板中会显示出编译情况。各条轨迹正常时，面板会直接显示“编译完成”。
#### 图2.172：输出面板

若存在问题，那么在输出面板中会有提示，即某个轨迹点存在不可达、轴超限等问题。双击提示，机器人姿态会更改到事件被执行时的状态。
##### 仿真
#### 位置：位于【编程仿真】下的【仿真调试】中，如图2.173所示。

功能说明：仿真即形象逼真地模拟机器人在真实环境中的运动路径和状态，查看机器人是否以正确的姿态工作。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image107.png)
图2.173：“仿真”位置

仿真管理面板：

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image108.png)
图2.174：仿真管理面板
#### 按钮作用：

：关闭仿真管理面板；

：开始仿真和暂停仿真；

：循环仿真。

仿真速度：

通过拖动滑块来控制仿真时的速度。百分比越大，速度越快。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image112.png)
图2.175：仿真速度调试页面

碰撞检测：

碰撞检测：对装配体各零部件、各相对运动部分进行实际仿真，并在发生碰撞时碰撞部分以暗红色高亮显示，如图所示，可以检查机构在运动状态下是否存在碰撞，如图2.176所示。
#### 图2.176：碰撞检测

场景还原：结束仿真后，机器人会回到轨迹的起始点位置。

显示效果：显示出自定义的工艺效果。

输出事件：点击输出事件后，右侧输出面板上会显示所添加的指令事件，如“等待”事件等。

调试模式：机器人各关节参数可在仿真过程中变化。

优化模式：机器人各关节参数在仿真过程中固定。在仿真过程中，选中优化模式，可使软件运行更加流畅。

仿真轨迹情况：

所有相关运动机构均通过动态的时间轴依次罗列、形象直观地显示出来，方便用户查看机器人、工件等轨迹的运行时间和进度，如图2.177所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image115.png)
图2.177：各运动机构仿真轨迹情况

若在同一时间内出现多个时间轴，说明在这段时间内，有多条轨迹同时运行。
##### 后置
#### 位置：位于【编程仿真】下的【仿真调试】中，如图2.178所示。
#### 图2.178：后置位置
#### 功能说明：“后置”功能将在软件中生成的轨迹、坐标系等一系列信息生成机器人可执行的代码语言，可以拷贝到示教器控制真机运行，如图2.179所示。
#### 图2.179：后置处理界面
#### 轨迹点命名中第一点的编号：后置的起始编号可根据需求设定，可以是0/1，也可以是其他。
#### 轨迹点偏移：分别设置x,y,z方向上的偏移数据。
#### 机器人末端：根据需求，选择机器人末端/关节空间/工具末端
#### 坐标系：选取轨迹坐标系或机器人基坐标系，并选取相应的TCP点。

程序名称：程序的名称可自行输入和修改。一般来说，该名称为示教器所识别的模块名称。

是否输出IO：生成的后置文件中显示所添加的IO事件。

使用注释：

注释是指解释代码语言的文字；是否使用注释根据需要设定。
#### 图2.180：“使用注释”对比图

忽略轨迹错误：生成轨迹的轨迹点发生错误，选择忽略轨迹错误，继续生成后置文件。若不勾选，则会报错，无法生成后置文件。

后置代码编辑器

点击【生成文件】后，弹出后置代码编辑器，生成的代码如下：
#### 图2.181：后置代码编辑器

不同的机器人后置会生成不同的文件格式.KUKA机器人会后置出两个文件：DAT/SRC.其他机器人会根据实际控制器文件需求，后置出一个或多个的数据文件。

- 后置代码的显示方式：点的坐标、字符和注释用不同颜色区别开来，代码查看起来清晰明了。

- 有行号显示，方便定位某一行的代码。

- 折叠功能，同一组别或者段落的代码可以实现手动折叠展开和收起。

- 提示功能：输入轨迹点指令的首字母，会提示出MoveL,MoveC等字样。完整的轨迹点指令+[ 会提示出相关指令的参数格式。（目前支持的是ABB机器人）

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image120.png)
图2.182：提示功能1

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image121.png)
图2.183：提示功能2

- 高亮显示：选中某个字符后，所有相同的字符以蓝底高亮显示。

- 导出文件编码：包括ANSI和UTF-8两种编码。ANSI编码不支持代码程序中包含中文字符，UTF-8则允许包含中文字符，从而根据特定品牌的机器的后置需求来选择这两种编码。

- 导出：将后置出的文件可拷贝到真实示教器，从而完成真机的运行。

保存：后置代码会保存在编辑器中。

*后置格式的具体显示样式，如字体颜色、背景色、折叠方式等都用XML控制。因此，用户可依据实际需求，自定义后置的具体显示样式。
##### 视向动画
#### 位置：位于【编程仿真】下的【仿真调试】中，如图2.184所示。
#### 图2.184：“功能位置”

功能说明：在仿真过程中自动转换到特定视角，以便更清晰地查看到机器人或其他组件的运动情况。
#### 点击，在界面左侧弹出“视向动画”面板，界面下方弹出仿真管理面板，拖动仿真管理面板的进度条，在需要添加视向的位置暂停，调整好绘图区里显示的组件位置和视角，点击“添加”即可添加视向。添加多个视向时，视向间切换的距离默认“5s”，视图的显示事件和保留时间都根据需要更改。
#### 图2.185：功能面板
##### 输出动画
#### 位置：位于【编程仿真】下的【仿真调试】中，如图2.186所示。
#### 图2.186：“功能位置”

功能说明：机器人的运动轨迹可以输出为动画；查看动画的方式有两种：微信扫码查看和复制链接用浏览器打开查看。可实现将轨迹仿真的动画过程上传到云端；同时自动生成二维码链接，后续可用手机扫码后缩放、平移查看该动画，如图2.187所示。
#### 图2.187：链接与二维码
#### *可以分享上图所示的软件中，也可以复制链接，分享给别人。
##### 输出视频
#### 位置：位于【编程仿真】下的【仿真调试】中，如图2.188所示。
#### 图2.188：“功能位置”

录制仿真视频并存储为相应格式的视频文件，如图2.189所示。
#### 图2.189：“输出视频”面板
##### 性能分析
#### 位置：位于【编程仿真】下的【仿真调试】中，如图2.190所示。
#### 图2.190：“功能位置”
#### 功能说明：显示机器人运动整体的、全面的信息，包含运动的全程时间，节拍，机器人品牌型号，运动的平均速度，使用的工具，总轨迹数，总距离，总轨迹点数等。节拍统计可以很好的评估效率，即机器人在单位时间内完成的工作量，如图2.191所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image129.png)
图2.191 机器人性能分析示例
##### 碰撞设置
#### 位置：位于【编程仿真】下的【仿真调试】中，如图2.192所示。
#### 图2.192：“功能位置”

功能说明：碰撞设置是为了检测物体在仿真过程中是否发生碰撞。点击碰撞设置，再点击“新建碰撞对”，在新弹出的窗口中选择待检测的物体，将需要检测的物体分别放在“第一组”和“第二组”，当两组之间的物体发生碰撞时会被检测。如图所示例子中，需要检测的是“GLA-N-350”与“零件2”，和“GLA-N-350”与“快换工具盘AQC-20-T”之间的干涉情况。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image131.png)
图2.193：碰撞设置窗口

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image132.png)
图2.194：选择待检测物体

选择完毕后，点击“确定”，在碰撞设置窗口中显示已设定好的碰撞对，可以选择是否勾选。勾选后，仿真中会进行该碰撞对的检测。在界面右侧的输出面板中会输出碰撞检测结果，如下图所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image133.png)
图2.195：勾选碰撞对

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image134.png)
图2.196： 仿真输出结果
##### 事件模板
#### 位置：位于【编程仿真】下的【仿真调试】中，如图2.197所示。
#### 图2.197：“功能位置”

设置自定义事件模板，在后续添加自定义仿真事件时，可以直接选用该模板。

点击后，填写“模板名字”和“模板内容”后，点击“录入”即可在右边看到定义好的模板。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image136.png)
图2.198： 自定义事件模板界面

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image137.png)
图2.199： 自定义事件选用模板
### 设置
##### 选项

含着软件一些基本系统设置，用户可根据自身需求进行修改。包括文档显示、系统设置、仿真设置、显示坐标系名称、轨迹显示、工具显示、零件显示、底座显示、生成控制一共九个方面的内容。
#### 文档显示：更改背景颜色以及地面的尺寸、颜色、网格颜色。

1. 系统设置：可调整撤销步数、状态栏是否显示、显示精度、输入文件设置（包括合并多个个体，使用文件中显示数据，忽略小模型三项，用户可自行勾选）、点指令风格、机器人关节空间显示精度，并能选择是否能通过鼠标滚轮向前放大。

1. 仿真设置：可选择是否设置运动学真实仿真，以及进行加速度值的设定。

1. 显示坐标系设置：可选择是否显示坐标系名称。

1. 轨迹显示：可改变轨迹线的颜色，并能设置是否显示轨迹点、轨迹姿态（轨迹姿态的显示可以选择显示坐标或显示Z向）、轨迹序号、特殊工艺点名字、TCP姿态、寻位标号、轨迹线（包括轨迹线、轨迹间连接线、轨迹名字），以及是否设置亮显只显示一个点，设置完成后可按照需要选择应用到全部轨迹，此处默认为勾选状态。

1. 工具显示：可选择TCP的显示状态，包括不显示、显示当前、显示全部三种，同时，还可勾选是否显示TCP名字；

1. 零件显示：可设置零件在默认显示和选中两种状态下，分别显示与否CP/RP，即抓取点与放开点

1. 底座显示：可设置是否显示底座的安装点；

1. 生成控制：可设置是否自动合并POS点，勾选该选项，则插入的POS点将被自动合并至前面轨迹内。
## 定义组件
### 机构
##### 3.1.1 定义机构
#### 位置：位于【定义组件】下的【机构】中，如图3.1所示。
#### 图3.1：功能位置

功能说明：定义机构，即定义机器人功能的延伸、拓展，依照流程可以定义出1~N轴的任意运动机构。对需要定义为机构的模型进行导入处理，然后点击图标，在弹出的窗口中选择已经完成预处理的模型，按照流程指引逐步完成操作。完整定义流程一般可分为四步，即导入模型、模型预处理、定义、检测。

1. 导入模型

点击“输入”，导入所需的step格式模型。

1. 模型预处理

导入的模型由于零部件层次关系不统一，需要对各个零部件进行预处理使之符合定义所要求的层次结构。在设计环境面板上可以显示出运动机构零部件的树结构，一般要求根目录为一个总装，命名为机器人的官方名称，子节点下依次排列BASE、J1、J2、…、Jn，如下图所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image140.png)
图3.2： 模型预处理的设计环境面板结果

下面以定义导轨为例：

（1）如图所示，将机构按照固定轴以及可动关节轴进行组合装配，并命名为BASE及J1,J2等（*命名字母需大写）。
#### 图3.3：功能位置

（2）根据实际生产需求，更改工件的颜色，使之尽可能与实体一致。
#### 图3.4：更改工件颜色
#### 定义三维球，首先点击空格键，使三维球与工件分离，根据三维球的使用方法，将三维球中心点放置在工件最底端，并使z轴方向向上，x轴方向向前。再次点击空格键，调整参数，使坐标系中心点坐标为（0，0，0），z轴方向坐标为（0，0，1），x轴方向坐标为（1，0，0），与视图左下角世界坐标系一致。
#### 图3.5：调整三维球位置
#### 图3.6：修改参数
#### 定义

定义机构以世界坐标系为参考点进行DH参数建模，确定运动机构中各个轴的姿态、软件零点、机械零点、运动范围和运动方向等信息。定义机构包括“了解基础知识”→“坐标检查”→“关节检查”→“参数输入”四个步骤，其要点就在于N轴之间的坐标系转换。通过单击菜单栏中“定义组件”下的“定义机构”，按照对话框中的指示完成机构定义。

（1）了解基础知识

定义机构涉及多方面知识，为了达到定义机构的目标，取得良好的定义效果，需要了解基本的知识，实现流畅操作。

如图3.7所示，在“帮助信息”界面，点击蓝色下划线字体跳转到更详细的帮助信息。了解并熟知列表中的知识后，勾选“我已熟知上述内容”，点击“下一步”。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image147.png)
图3.7： 帮助信息界面

（2）坐标检查

运动机构在DH参数建模时以世界坐标系为参考零点。此时默认的坐标系选择为“世界坐标系”，如图3.8所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image148.png)
图3.8： 坐标检查界面

1. 关节检查

首先，确定机构类型。机构类型包括通用机构、变位机和导轨。在案例中涉及到的1~N轴的机器人都属于通用机构。

其次，确定运动机构的关节数，确保设计环境中的装配结构与模型预处理结果一致。根据公式确定，关节数量=运动方式为平移的关节+运动方式为旋转的关节。

链接最大外部轴数：定义机器人所链接外部轴的最大轴数，用于配合通用机构后置时刻输出的轴数量。值得注意的是，默认链接的最大外部轴数为6。例如，当限定链接最大外部轴数为2，该机构与某个外部轴创建链接，后置程序中只能输出两个轴的轴数据。

一般情况下，软件会自动识别出机构的关节数。但若之前未对模型进行预处理，会弹出警告提示，只有在模型预处理成功后才能成功进行下一步的操作，如图3.9所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image149.png)
图3.9：关节处理界面

1. 参数输入

参数输入主要包括设定模型的DH参数、软件零点、机械零点、各个轴的运动范围及运动方向等。坐标转换的最终目的是确定机器人各连杆之间的相互位置关系，如图3.10所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image150.png)
图3.10：参数输入界面

a.机器人基本信息

机器人基本信息包括“机构类型”、“机构名称”、“机构品牌”、“机构型号”，按照实际情况填写即可。

“机构类型”可选择“通用机构”、“变位机”和“导轨”。没有特殊需要一般默认选择“通用机构”即可。

“机构品牌”的下拉菜单中有多个机器人品牌以供备选，如没有找到所需品牌，选择“自定义”即可。

“机构名称”和“机构型号”可自拟。其中“机构名称”必须填写，“机构型号”可选填。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image150.png)
图3.11：机器人基本信息位置

b．姿态

可供备选的姿态方向格式包括四元数、旋转矢量法和欧拉角。ABB机器人多用四元数来表示，其他品牌机器人一般用欧拉角来表示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image150.png)
图3.12：机器人姿态位置

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image152.png)
图3.13: 可选择的机器人姿态表示方法

c．后置类型

选择与当前所定义的机构相匹配的后置类型。若列表中无对应的后置类型，选择“自定义”。需要注意的是，选择“自定义”之前，需要将提前准备好的后置文件（格式为ropost）导入。而自定义的后置文件可以通过PQArt的“自定义后置”功能来生成，如图3.14所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image150.png)
图3.14：机器人后置类型位置

d．逆解类型

完成了后置类型的定义之后，选择相应的逆解类型，包括R—Revolute，代表旋转关节；P—Prismatic，代表平移关节。其中，3R1P表示常见的四轴机器人（旋转-旋转-平移-旋转）；6R表示通用6轴机器人，该类型机器人的最后三个旋转轴交于一点；6R非球型表示最后三轴不相交于一点的6轴旋转机器人，如图3.15所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image150.png)
图3.15：机器人逆解类型位置及可选择类型

e.机器人各轴坐标系之间转换的参数

为进行DH参数建模，需要对各轴的坐标系进行转换，确定各轴坐标系之间转换的参数。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image150.png)
图3.16：填写机器人各轴坐标系之间转换参数的位置

所需参数：

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image155.png)
图3.17： 坐标系转换

theta(°) 表示坐标系Z轴旋转的角度，d(mm)代表Z轴平移的距离； a(mm) 表示坐标系X轴平移的距离，alpha(°)代表X轴旋转的角度。

“轴类型”可选择该轴为平移轴还是旋转轴。

“关节号”依次从基座，第一轴到最后一轴按顺序排列显示。如果顺序不对，应先点击前面的序号，在弹出的下拉框中选择正确的对应关节。

机器人参数处理

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image150.png)
图3.18：机器人参数处理

机器人各关节的位置和运动信息可直接从外部导入，点击“导入参数”，选择写有机器人关节信息的“.txt”文件即可。

“自定义参数”支持自行添加相关参数，需要添加好参数名称和参数值，点击“确定”。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image156.png)
图3.19： 自定义参数

“保存参数”可以保存当前设定的所有参数。

f. 定义每个轴的坐标系.

坐标系功能：用来确定轴的位置；用Z轴确定每个轴的运动方向。建模过程是从世界坐标系开始，依次转换每个轴的坐标系。

BASE坐标系转换为1轴坐标系。首先点击界面中的【更新】按钮，弹出世界坐标系。运动机构的底座是不动的，一般情况下默认为与世界坐标系重合，如图3.20所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image157.png)
图3.20：世界坐标系

Z轴方向决定的是每个轴的运动方向，上图所示的红色箭头为1轴的运动方向，可以发现，1轴的运动方向与BASE坐标系的Z轴方向一致，此时BASE一栏的DH参数无需填写。

J1坐标系转换为J2坐标系的DH参数可以借助“测量”工具完成，具体步骤如下。

步骤一.显示坐标1和坐标系2，如图3.21所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image158.png)
图3.21：J1坐标系转换为J2坐标系

界面中，J1后的参数为J1坐标系转换到J2坐标系的平移距离和旋转角度。坐标系1是世界坐标系（1轴坐标系），坐标系2是2轴坐标系。红色箭头为2轴的运动方向，需让J2坐标系的Z轴方向与该方向一致。图中的坐标系2即为转换完成后的2轴坐标系。

步骤二.测量两坐标系间的平移距离。

在这里，平移距离的数据可以用“测量点”来获得。右击“机器人加工管理面板”的空白处，选择“测量点”功能，测量的是拾取的点在世界坐标系中的位置。点击选择“测量点”后，拾取J1上的一个点，弹出的对话框中会显示出该点的三维坐标。

对于定义机构来说，在J1坐标系（世界坐标系）转换为J2坐标系的过程中，该指令可以测量2轴上某点的位置，从而得到的数据即为J1坐标系需要平移的距离。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image159.png)
图3.22：测量点的位置

其他坐标系转换时需用测量工具测量（详情参考章节4.6）而得。

鼠标单击绘图区空白处，按下大写字母A，弹出世界坐标系（或点击设计环境中的全局坐标系），弹出世界坐标系。

利用测量工具，测量世界坐标系原点和1轴之间的距离，如图3.23。经过测量，获知坐标系原点与1轴之间的距离为4200mm，因为此次平移的方向为X轴的负方向，所以J1中X轴平移参数 a(mm) 数值为-4200。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image161.png)
图3.23：1轴坐标系平移距离

平移后点击“更新”，可在绘图区查看到平移后的效果。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image162.png)
图3.24：转换后的2轴坐标系

接下来更改Z轴方向，需让Z轴与2轴运动方向保持一致，使坐标系的X轴旋转-90°即可。从1轴到2轴的坐标系转换完成。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image163.png)
图3.25：转换完成后的2轴坐标系

步骤三.依次确定其他轴的坐标转换

其中，关节坐标系转换到法兰坐标系的参数，应先确定法兰盘坐标系在真实环境中三个轴的姿态，再确定四个参数。

g. 坐标系偏移

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image164.png)
图3.26: 机器人坐标系偏移

示教器坐标系状态下，真实环境中的运动机构会有一个姿态。通过“平移XYZ”和旋转“XYZ”将当前软件中模型的姿态调整到与真实环境中的姿态一致。这是对运动机构位姿的整体调整。

h.确定软件零点、机械零点、限位以及运动方向等。

确定好运动机构的机械零点后，观察当前机构模型与机械零点状态是否有差异。若有差异，需要对各个轴的位置进行调整。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image165.png)
图3.27： 软件零点与机械零点

最大限位与最小限位指各个轴运动（平移/旋转）的最大与最小距离/角度，即是轴的运动范围。

运动方向可设定各个轴运动方向的正反。可通过“更新”，实时查看运动机构的运动方向是否正确。

i.保存

点击“保存”，将定义完的运动机构保存到指定位置，格式为robr/robrd。

（5）检测

定义完运动机构后需对其进行检测，查看是否满足定义要求。

将定义好的运动机构导入进来后，拖动调试面板中的滑动器来控制机构的各轴运动，查看其运动方向是否正确、是否存在关节脱离的情况等。一般情况下，定义正确的机构，它的各个轴和关节都可以正常运动。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image166.jpeg)
图3.28：  检测定义好的运动机构
##### 3.1.2 导入机构
#### 位置：位于【定义组件】下的【机构】中，如图3.29所示。
#### 图3.29：功能位置

功能说明：通过该功能可以导入预先定义的自定义机构，文件格式为.robr或.robrd。
### 工具

工具是机器人工作时所使用的机械性或智能性器具，主要分为法兰工具、快换工具、外部工具三类：

1.法兰工具：安装在机器人法兰盘上的工具，法兰盘通常是指在一个类似盘状的金属体的周边开几个孔，用于固连其它工具等；

2.快换工具：由机器人侧用和工具侧用组成。机器人侧用指的是与机器人法兰盘连接的工具，工具侧用指的是与法兰工具连接的工具。当机器人需要完成两种及以上的任务时，通过快换工具可以快速更换工具，而不用从法兰盘上拆下工具，省时省力；

3.外部工具是没有安装在机器人上的工具，如打磨机、砂轮等。有时机器人需要手持工件配合使用外部工具。
##### 定义工具
#### 位置：位于【定义组件】下的【工具】中，如图3.30所示。
#### 图3.30：功能位置

功能说明：在定义工具之前，需要先通过“输入”导入工具模型于场景中。在定义工具时，需要设置FL、CP、TCP，三者表示的含义如下。

FL：法兰工具与机器人法兰盘的相接点，即法兰工具的安装点；

CP：法兰工具与快换工具的相接点，在机器人侧用与工具侧用的相接处；
#### TCP：工具加工点，即工具工作的位置。

1. 定义法兰工具

法兰工具是安装在机器人法兰盘上的工具，用于和机器人六轴末端进行装配。

点击【定义工具】，并于场景中选择导入的工具模型后，选择“工具类型”

为法兰工具，之后添加并编辑附着点。点击来添加法兰工具和机器人的连接点，即工具安装点，通过调整工具附近弹出的三维球来调整FL至正确位置上，如图3.31所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image168.png)
图3.31： FL位姿调整效果

再点击来调整工具中心点，以确定工具加工工件的位置，通过调整工具附近弹出的三维球来调整TCP至正确位置上。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image170.png)
图3.32： TCP位姿调整效果

添加完成后，若需进一步调整，可以通过点击来删除已添加的安装点和加工点。可以通过点击来更改安装点和加工点的信息。可以通过点击来复制已添加的点。

如图3.33所示，参数设置完成后，可以点击“类型选择”右侧的“工具信息”与“作者信息”，并按照实际需求进一步补充相关内容。设置无误后，点击“确认”，则法兰工具定义完成。也可点击“另存”，将其保存至另一位置，文件格式为“.robt”。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image174.png)
图3.33：  定义法兰工具
#### 定义快换工具

快换工具表示，当机器人需要完成两种及以上任务时，可以快速更换，而无需从法兰盘上拆下。
#### 点击【定义工具】，并于场景中选择对应导入的工具模型后，选择“工具类型”为快换工具，之后添加并编辑附着点。点击来添加快换工具与法兰工具的相接点，即工具安装点，通过调整工具附近弹出的三维球来调整CP点至正确位置，注意，需要调整CP点的Z轴与机器人侧用的Z轴相对，X轴和Y轴根据实际情况进行调整，如图3.34所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image176.png)
图3.34： CP位姿调整效果

再点击来调整工具中心点，以确定工具加工工件的位置，通过调整工具附近弹出的三维球来调整TCP至正确位置上。参考图3.35所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image177.png)
图3.35： TCP位姿调整效果

添加完成后，若需进一步调整，可以通过点击来删除已添加的安装点和加工点。可以通过点击来更改安装点和加工点的信息。可以通过点击来复制已添加的点。
#### 图3.36： 定义快换工具

如上图所示，参数设置完成后，可以点击“类型选择”右侧的“工具信息”与“作者信息”，并按照实际需求进一步补充相关内容。设置无误后，点击“确认”，则快换工具定义完成。也可点击“另存”，将其保存至另一位置，文件格式为“.robt”。

1. 定义外部工具

外部工具是独立于机器人之外的工具，如打磨机、砂轮等，该类工具无需安装到任何设备上，只需添加工具加工工件的TCP点即可。

点击【定义工具】，并于场景中选择对应导入的工具模型后，选择“工具类型”为外部工具，之后添加并编辑附着点。点击“+TCP”来调整工具中心点，以确定工具加工工件的位置，通过调整工具附近弹出的三维球来调整TCP至正确位置上，如图3.37所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image179.png)
图3.37： TCP位姿调整效果

添加完成后，若需进一步调整，可以通过点击来删除已添加的安装点和加工点。可以通过点击来更改安装点和加工点的信息。可以通过点击来复制已添加的点，如图3.38所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image180.png)
图3.38： 定义外部工具

如上图所示，参数设置完成后，可以点击“类型选择”右侧的“工具信息”与“作者信息”，并按照实际需求进一步补充。设置无误后，点击“确认”，则外部工具定义完成。也可点击“另存”，将其保存至另一位置，文件格式为“.robt”。
##### 导入工具
#### 位置：位于【定义组件】下的【工具】中，如图3.39所示。
#### 图3.39：功能位置
#### 功能说明：若存在已定义完成的工具需要导入PQArt中，可通过点击“导入工具”将工具导入其中。
### 零件
##### 定义零件
#### 位置：位于【定义组件】下的【零件】中，如图3.40所示。
#### 图3.40：功能位置
#### 功能说明：零件的模型有多种选择，可将工具、零件和底座等都看作是零件进行自定义，基本可以满足市场上存在多种零件的需求。在定义零件之前，需要先通过“输入”导入零件的模型于场景中，如图3.41所示。
#### 图3.41：定义零件面板

填写作者和公司信息，可自定义填写简介，确保信息设置无误后，点击“确认”，则零件定义完成。点击“另存”，则可将其存于另一位置，文件格式为“.robp”。
##### 导入零件
#### 位置：位于【定义组件】下的【零件】中，如图3.42所示。
#### 图3.42：功能位置
#### 功能说明：若存在已定义完成的零件需要导入PQArt中，可点击“导入零件”将零件导入其中。
### 3.4 底座
##### 定义底座
#### 位置：位于【定义组件】下的【底座】中，如图3.43所示。
#### 图3.43：功能位置
#### 功能说明：首先通过“输入”导入底座模型于场景中，导入完成后，点击“定义底座”，在场景中选择导入的底座模型，点击确认，并设置模型信息与作者信息。底座需要添加一个安装点，导入底座后，通过安装点实现与机器人的自动装配。在定义底座时，安装点已被自动生成，因此，用户只需根据需要编辑调整安装点位置即可。在模型信息的界面，用鼠标点击即可调整安装点位置，通过调整模型上弹出的三维球来进行安装点的调整，安装点的Z轴为机器人安装到底座上的安装方向，一般情况下，Z轴朝上。
#### 图3.44：设置底座参数

信息设置无误后，点击“确认”，则底座定义完成。也可选择“另存”，将定义完成的底座保存到另一位置，文件格式为“.robs”。
##### 导入底座
#### 位置：位于【定义组件】下的【底座】中，如图3.45所示。
#### 图3.45：功能位置
#### 功能说明：首先导入一个机器人，再通过“导入底座”将定义好的底座导入进来。底座导入完成后，机器人会自动安装到底座上，这说明底座的定义正确，如图3.46所示。
#### 图3.46：底座安装示意图
### 3.5状态机
##### 3.5.1 定义状态机
#### 位置：位于【定义组件】下的【状态机】中，如图3.47所示。
#### 图3.47：功能位置

功能说明：在自定义状态机之前，需要先通过“输入”导入状态机模型于场景中。目前，状态机支持一轴结构，模型导入成功后，需要将状态机的模型整理为“Base”和“J1”两部分，即将其分为底座和活动关节，如图3.48所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image185.png)
图3.48：状态机模型整理

模型导入并整理完成后，选择“定义状态机”，在弹出的窗口中进行模型选择，选择模型列表为“场景”，并选择导入的状态机模型名称，点击确定。之后，需要根据状态机本身的运动情况，来对它不同的运动状态进行定义。

在弹出的定义状态机窗口中，默认选择的移动关节为“J1”关节，根据需要选择运动方式为“旋转”或“平移”。“运动范围”即为关节运动的最小值和最大值，根据实际需求自行设置即可。点击后，可以通过状态机模型上出现的三维球来调整关节J1的移动方向，确认无误点击应用。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image187.png)
图3.49：状态机参数设置

通过点击并根据状态机的运动情况，设置运动时间和关节运动值，使其能完成几个固定动作（如伸出、缩回等）。若发现状态添加有误，可以点击将其删除，根据状态添加完成后如下图所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image190.png)
图3.50： 状态机状态添加

设置完成后，点击“确认”，则状态机定义完成。点击“另存”，可将其存于另一位置，文件格式为“.robm”。

状态机定义完成后，选中该状态机，点击鼠标右键并选择“切换状态”，则可以查看状态机在不同状态下的运动情况，如图3.51所示。

图3.51：选择状态
##### 3.5.2 导入状态机
#### 位置：位于【定义组件】下的【状态机】中，如图3.52所示。
#### 图3.52：功能位置

功能说明：若存在已定义完成的状态机需要导入PQArt中，可点击“导入状态机”将状态机导入其中。
### 3.6 工艺效果仿真
##### 3.6.1 定义效果
#### 位置：位于【定义组件】下的【工艺效果仿真】中，如图3.53所示。
#### 图3.53：功能位置

功能说明：借助仿真，可以实现喷涂、焊接，熔覆堆焊等加工工种的仿真过程效果实时呈现。

定义效果前，首先保证零件位于世界坐标系原点。其中在坐标系节点下找到世界坐标系-WCS，单击后，可在绘图区看到世界坐标系，如图3.54所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image192.png)
图3.54：零件位于世界坐标系原点

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image193.png)
图3.55： 世界坐标系显示

保证零件位置正确后，点击“定义效果”，弹出定义效果窗口，如图3.56。自定义效果“名字”，在“选择模型”处选定该模型，根据效果显示的时间选定“开始事件”与“结束事件”，“长度”表示铺设相邻两零件模型时两模型中心点的间距，如图3.56所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image194.png)
图3.56： 定义效果窗口
##### 3.6.2 管理效果
#### 位置：位于【定义组件】下的【管理效果】中，如图3.57所示。
#### 图3.57：功能位置

功能说明：管理效果窗口中可对已有的工艺效果进行编辑、添加或删除，也可加载已定义好的效果，或保存现有效果参数（文件格式.robe）。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image195.png)
图3.58： 管理效果
### 3.7 后置
##### 自定义后置
#### 位置：位于【定义组件】下的【后置】中，如图3.59所示。
#### 图3.59：功能位置

功能说明：自定义后置，即自定义机器人的后置代码，大幅度增加了后置代码书写排列的灵活性，满足多种后置需求。自定义后置一般与自定义机器人相关联。自定义机器人时需选择后置类型，将自定义的后置文件导入，即可为自定义的机器人设置后置格式。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image196.png)
图3.60：后置模板

后置模板选择部分可以在下拉菜单中找到包括ABB、KUKA、FAUNC等众多常用品牌和型号的机器人后置文件模板。若没有找到所需的机器人后置模板可使用“自定义”模板，如图3.61所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image196.png)
图3.61：概览和细节

概览和细节：包含后置代码的全部对象。“概览”对所有后置元素进行分类，相当于文件夹；“细节”相当于子文件夹，展示的是“概览”中每个类别下包含的具体元素。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image196.png)
图3.62：后置代码编辑区域

后置代码编辑区域：该区域包括树形结构图、局部预览和全局预览。树形结构图用于确定后置代码的格式，RobotArt支持多个不同格式的文件撰写。

树形结构图分为三个部分：文件头、数据部分（一般是被轨迹组的迭代器包括，或与轨迹组的迭代器平级）、文件尾。应根据实际要求来设定后置格式，文件头与文件尾为非必要结构。

当前预览：预览选中的对象；全局预览：预览到后置代码最终的形式。

结构图说明：

（1）元素的删除与编辑：右击各个元素，可实现删除操作，可编辑其属性。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image197.png)
图3.63：结构图元素右键菜单

属性包括选中对象的精度（数值保留的小数点）、表达式以及是否选择为关键字。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image198.png)
图3.64： 节点的属性面板

小数点保留五位：

关键字：指所有无法更改数据的元素，包括轨迹组的迭代器、轨迹的迭代器数据已固定的元素。如换行（可插入字符）、字符等可更改数据内容的元素不是关键字。

是否是关键字：是否在后置代码中亮显所选的元素。

1. 查找可作为参照的后置代码

找到目标机器人准确的后置代码文件。以其为参照，自定义目标机器人后置代码。下图为LBD-LT1500的后置代码。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image200.png)
图3.65： 机器人LBD-LT1500的后置代码

2.确定后置代码的表示含义和格式

无需改动默认固定字符，仅需对其他部分进行更改。确定后置代码的格式时，需要注意两个部分：a.各元素之间的分隔符，以及换行的位置；b.每个数据的意义。在此代码中，各数据的意义如表。

表： 机器人LBD-LT1500的后置代码含义

| VL= TOOL= J1/J2/J3/J4/J5/J6=N | 字符 |
| --- | --- |
| VL后的数据 | 速度值 |
| “TCP” | TCP名 |
| J1-J6 数值 | 关节角 |
| XYZ和ABC | 轨迹点的位置和姿态 |
| N后的数值：1、2、3、4、5...... | 全局点序号 |

3.确定运算表达式

后置中，所有数值类元素都有运算表达式，即this+运算符。默认的位移/距离单位为mm，速度值单位为mm/s，关节角单位为弧度。如，将关节角的单位由弧度转换为角度，运算表达式为“this*3.14/180”。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image201.png)
图3.66： 属性中的运算表达式

4.确定每个节点之间的层级关系

编辑结构树时，字符与换行可以拖拽到任意节点下。基本结构树包含文件头、轨迹组的迭代器、文件尾，如图3.67所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image202.png)
图3.67： 文件结构

在定义后置中，最后生成的结构图如图，先后将各个元素按照图中顺序拖入结构树中即可。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image203.png)
图3.68：机器人LBD-LT1500的自定义后置结构树

对于层级关系的几点要求：

a.“轨迹组的迭代器”层次关系如图。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image204.png)
图3.69： 轨迹组的迭代器

b.moveL、moveJ、moveAbsj和moveC必须放到点指令下。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image205.png)
图3.70：点指令下包含的元素

c.“发送事件”下必须包括默认IO事件信息和IO值（自定义事件和等候时间事件除外）。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image206.png)
图3.71： 发送事件

d.文件尾只能包括字符和换行。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image207.png)
图3.72： 文件尾

e．一般会在文件的末尾添加一个“点的IO事件”节点和“自定义事件”的子节点，用以应对新的事件需求，保证额外添加自定义事件后，可以输出后置代码。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image208.png)
图3.73：末尾添加一个点的IO事件

5.保存文件

树形结构图确定完毕后，对文件进行保存，如图3.74所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image209.png)
图3.74： 文件操作

【另存为】将代码保存到指定位置，文件格式为ropost；

【加载】导入格式为ropost的后置文件，实现再次编辑。
## 校准

校准，作为连接离线编程软件和真机运行之间重要的桥梁，是PQArt中重要的功能群组。其主要包括手动校准、自动校准和坐标系标定三个子功能栏。
### 自动校准

位置：在【校准】下的【自动校准】中，如图4.1所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image210.png)
图4.1：功能位置

新增功能校准装配体：

功能说明：通过此功能，无需进行其他设备的定义，可将场景中的三维数模直接进行校准，对于变位机等一些设备来说，可采用此功能先进行校准，将校准好的模型再定义为场景设备，便于和实际保持一致，如图4.2所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image211.png)
图4.2：校准装配体
##### 三点校准法

位置：在【校准】下的【自动校准】中，如图4.3所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image210.png)
图4.3：功能位置

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image212.png)
图4.4：三点校准面板界面

功能说明：首先根据需求选择校准目标类型以及相应的坐标系。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image213.png)
图4.5：校准目标类型选择

通过校准三个点的坐标校对机器人的位置。具体操作包括三步。

1.从设计环境中拾取模型上三个点（不共线）；

2.测量真实环境模型上对应的三个点坐标，并输入坐标；

3.点击“对齐”后，设计环境中的模型就会变换到与真实环境一致的位置。

*选取的三个点不共线。设计环境中指定的三个点要和真实环境中测量的三个点位置保持一致。

如图，三点校准界面中，坐标系指工件位置所参考的坐标系。这里的坐标系包括基坐标系和法兰坐标系。坐标系可选择基坐标系和法兰坐标系。基坐标系固定在机器人基座内，用来说明机器人在世界坐标系中的位置。法兰坐标系固定于机器人的法兰盘上，是工具的原点（一般常见的法兰坐标系都是Z轴朝外，X轴朝下）。模型应选择当前需要校准的工件。

设计环境指PQArt软件中的绘图区；真实环境：真机操作环境。

导入：将保存在txt文件内的真实环境中测量的数据导入到软件中。

保存：输入真实环境中测得的三个点数据后，将其保存到文件中（txt），方便下一次读取数据。

误差分配方式：可选择平均分配方式或以第一个点为基准，并设置所需误差值。
##### 多点校准

位置：在【校准】下的【自动校准】中，如图4.6所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image210.png)
图4.6：功能位置

功能说明：借助已经校准完成的机器人工具，采集被校准零件上的3-5个圆孔边线上的数据（机器人工具TCP点，通过示教器人工操作，接触被测圆孔端面上均布的一些点，每个圆孔至少要采集三个点以上的数据点）；然后通过“多点校准”的功能，来实现对多面体的校准。从而使设计环境和真实环境下，被加工零部件和机器人本体的相对空间位置关系保持一致。
#### 图4.7：多点校准功能面板
##### 点轴校准

位置：在【校准】下的【自动校准】中，如图4.8所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image210.png)
图4.8：功能位置

功能说明：该功能进行了优化，拾取半圆柱面或曲面上的圆柱面，能够求出圆柱面轴的位置和入刀点位置。另外，使用这个功能有多种情况，需要注意一下，结果是一样的：

a.拾取孔洞与断面的相交边，则会固定住3个移动和2个旋转，五个自由度；后续拾取点后，则锁住被校准零件的最后1个旋转自由度。

b.拾取孔洞的侧面，则会固定住2个移动和2个旋转，共4个自由度；后续拾取点后，则改点会强制与实际物体位置点进行强制重合匹配，从而被校准的零件最后的1个移动和1个旋转的自由度会被加上。这种情况下，会引起被测零件强制移动。造成轴部分周边校准精度下降。
#### 图4.9：点轴校准功能面板
#### 点的指定：“指定轴”下的X Y Z指的是该条轴坐标系三个方向上的向量，在零件上指定时应选择与轴垂直的一个圆环或者曲面。此时确定的是轴的位置，不包括方向。“校准点”可选择零件上的任意一点。

导入轴数据：将实际环境中测得的轴数据文件导入，文件格式为txt，不支持手动输入，节省了录入数据时间。
#### 轴反转：输入虚拟环境和真实环境中的数据后，点击【对齐】，可看到校准后的效果。若发现轴向与预期的不一致，点击【轴反转】即可。“轴反转”即确定了轴的方向。

*真实环境内采集的用来确定轴的点（至少三个），必须来自于与轴线共轴的圆柱端面边线或圆孔边线上采集；设计环境内，拾取的校准点，注意不要和轴线相交。
##### 三面校准

位置：在【校准】下的【自动校准】中，如图4.10所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image210.png)
图4.10：功能位置

功能说明：借助已经校准完成的机器人工具，采集被校准零件上的三个空间面上的数据（机器人工具TCP点，通过示教器人工操作，接触被测平面，每个面至少要采集三个点以上的数据），然后通过“三面校准”的功能，来实现对多面体的校准。从而使设计环境和真实环境下，被加工零部件和机器人本体的相对空间位置关系保持一致。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image216.jpeg)
图4.11：三面校准法面板
##### 点云校准

位置：在【校准】下的【自动校准】中，如图4.12所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image210.png)
图4.12：功能位置
### 坐标系标定
##### 4.2.1 新建坐标系

位置：在【校准】下的【坐标系标定】中，如图4.13所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image210.png)
图4.13：功能位置

功能说明：新建坐标系即新建一个工件坐标系，用来表示工件的位置和姿态。通过拾取工件上的任意三个点来建立坐标系。该指令也是校准工件与机器人相对位置的方法之一，效果与三点校准法一样，如图4.14所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image217.png)
图4.14：创建坐标系界面

- 获取：拾取工件上的点以确定坐标系三个轴的位置和姿态；

- 坐标系预览：预览所建的坐标系；

- 存为用户坐标系：确认当前所建坐标系的操作并保存坐标系。

方法：点击界面中的获取按钮后，在工件上拾取点。依次拾取三个点，分别确定坐标系原点、X轴、Y轴/Z轴的位置。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image219.png)
图4.15：新建坐标系

轨迹关联工件坐标系

在轨迹的右键属性内，通过修改使用的坐标系为“工件坐标系”，可以促使该轨迹的所有的点坐标值按照自定义的工件坐标系来表示，如图4.16所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image220.png)
图4.16：工件坐标系的使用方法

*可以通过查看“轨迹点属性”值或后置来查看替换坐标系的前后的区别

编辑工件坐标系

新建工件坐标系后，该坐标系会在机器人加工管理面板中的“工件坐标系”下挂有子节点，在此处可通过右键菜单对工件坐标系进行各种处理，实现工件坐标系的编辑、复制、删除、隐藏、显示、重命名等，还可查看和更改属性特征，如图4.17所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image221.png)
图4.17： 工件坐标系的右键菜单

三维球编辑：通过拖动旋转三维球，改变用户坐标系的姿态和位置。

编辑：编辑工件的位置和姿态，可用来进行工件校准。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image222.png)
图4.18：工件坐标系校准界面

*编辑坐标系时场景中一定要有机器人存在。

*基于坐标系：通过切换基于的坐标系，工件坐标系的校准数据值，会相应变为基于参考坐标系的数值。

复制：复制当前选中的工件坐标系。复制的坐标系会与原坐标系重合。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image223.png)
图4.19：复制工件坐标系

删除、隐藏、显示和重命名：

删除：删除当前选中的工件坐标系；

隐藏：隐藏当前选中的工件坐标系后，绘图区中的坐标系消失，机器人加工管理面板中的坐标系子节点变为灰色；

显示：将已隐藏的工件坐标系重新显示出来；

重命名：修改所选工件坐标系的名称。

属性：选择坐标系关联的工件
#### 图4.20：工件坐标系“属性”界面
##### 4.2.2 线面坐标系

位置：在【校准】下的【坐标系标定】中，如图4.21所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image210.png)
图4.21：功能位置

功能说明：在一些没有特征点的模型中，软件不能准确的捕捉到模型的尖点，无法生成用户坐标系，为解决这个问题PQArt推出新的坐标系生成方式，通过拾取模型上的一条边和一个面生成用户坐标系，拾取的边的起点作为坐标系的原点，边的终点作为坐标系的x轴方向，边的起点在拾取面上的投影为z轴方向，如图4.22所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image225.png)
图4.22：线面坐标系
##### 4.2.3 坐标系转换

位置：在【校准】下的【坐标系标定】中，如图4.23所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image210.png)
图4.23：功能位置
#### 功能说明：此功能主要是配合校准手持零件使用，首先选择姿态方向格式，共有四种，分别为四元数、欧拉角XYZ、欧拉角ZXZ、欧拉角ZYX、欧拉角ZYZ。
#### 图4.24：姿态方向的选取
#### 下图中第一个坐标系为“机器人法兰相对于BASE”的数值，第二个坐标系为“外部工具TCP”的数值，通过调整机器人姿态，让零件的不同特征点触碰外部TCP尖点，就会计算出不同的数据，根据这些数据的XYZ导入到不同校准方法的实际数据中进行校准。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image227.png)
图4.25：坐标系转换功能面板
##### 4.2.4 计算方向

位置：在【校准】下的【坐标系标定】中，如图4.26所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image210.png)
图4.26：功能位置

功能说明：可用于计算实际机器人的工具TCP的Z轴方向，让工具X方向尽可能贴合机器人的X方向，校准并读取第一个工具坐标系的XYZ，再使工具向外延长一段距离，校准并读取第二个坐标系的XYZ，进而可以计算出工具TCP的姿态。
#### 图4.27：计算方向功能面板
##### 4.2.5 反推坐标系

位置：在【校准】下的【坐标系标定】中，如图4.28所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image210.png)
图4.28：功能位置

功能说明：此功能用于反推出用户坐标系的位置和姿态，首先需要软件中的机器人关节值和实际机器人关节值保持一致，通过选择机器人法兰末端或者工具末端TCP，输入对应的末端数据，进而计算出用户坐标系的位置和姿态，如图4.29所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image229.png)
图4.29：反推坐标系功能面板
## 自由设计
### 创建草图

位置：在【自由设计】下的【创建草图】中的【新建草图】，如图5.1所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image230.png)
图5.1：功能位置

功能说明：点击图标功能面板如图5.2，选择建立草图的参考元素，包括草绘方向、原点、反转平面以及偏移距离。“草绘方向”是指选择与草图平面平行的参考元素。“原点”是指草图的中点。勾选“反转方向”，即可翻转平面法向量的正方向。“偏移距离”是指草图平面与参考平面间的距离。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image232.png)
图5.2: 新建草图面板

（1）建立与坐标系平面平行的平面

选定“XY方向”，“XZ方向”“YZ方向”分别是建立XY平面，XZ平面和YZ平面平行的平面。然后选择“原点”，“拾取的点”可以在绘图区选择原点，或者选择“世界坐标系原点”。确定是否勾选“反转方向”和偏移距离。最后，点击“确定”，草图建立完成。

（2）建立任意方向的平面

选择“点”或“三个点”，在绘图区选中指定点作为参考。如果选择“点”即是建立以该点为原点，与该点所在草图平行的平面。在绘图区选定特定点后（被选中的点会变为蓝色，如图所示），确定是否勾选“反转方向”和偏移距离后，点击“确定”，草图建立完成。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image233.png)
图5.3： 选中“点”元素
### 创建基本图元

点击新建草图后，在模型平面上任意创造基本图元，应用面板上所展示的功能，进行图元的绘制或文字的生成。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image234.png)
图5.4：功能界面

点击新建草图后，可在工件上运用点、直线、圆弧+圆、椭圆弧、椭圆、矩形、正多边形、键槽、多段线、圆角、文字等图元，进行绘制。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image235.png)
图5.5：绘制界面
### 曲线绘制

创建草图后，点击曲线绘制，设置好参数后，点击确定。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image236.png)
图5.6：绘制曲线

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image237.png)
图5.7：绘制曲线效果
## 程序编辑

在PQArt虚拟仿真中设备通过仿真程序编辑器中的代码，模拟真实设备的运动状态，显示代码的行号，支持函数和逻辑指令的添加，可以在编辑器中数字、注释和指令等关键字以不同颜色显示。
### 启动编辑
##### 同步
#### 位置：在【程序编辑】下的【启动编辑】中，如图6.1所示。
#### 图6.1：功能位置

功能说明：用于同步环境中添加的机器人轨迹和信号指令，同步的代码为机器人可识别的程序代码，目前支持ABB、KUKA、Fanuc、ADT、STEP以及Efort六大机器人品牌。如图6.2所示为程序编辑窗口。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image239.png)
图6.2 程序编辑窗口
##### 编辑
#### 位置：在【程序编辑】下的【启动编辑】中，如图6.3所示。
#### 图6.3：功能位置

功能说明：可将同步过的机器人程序代码进行编辑。
##### 退出

位置：【程序编辑】下的【启动编辑】栏内的【退出】，如图6.4所示。
#### 图6.4：功能位置

功能说明：用于退出程序编辑器。
### 导入

位置：【程序编辑】下的【导入】栏内的【导入】，如图6.5所示。
#### 图6.5：功能位置

功能说明：导入程序：可将电脑磁盘中保存的可识别的机器人程序代码导入到程序编辑器中进行编辑仿真。
### 编辑

6.3.1. 撤销

位置：【程序编辑】下的【编辑】栏内的【撤销】，如图6.6所示。
#### 图6.6：功能位置

功能说明：用于撤销编辑过程中的操作。

6.3.2. 恢复

位置：【程序编辑】下的【编辑】栏内的【恢复】，，如图6.7所示。
#### 图6.7：功能位置

功能说明：可将编辑过程中撤销的操作进行恢复。

6.3.3. 复制

位置：【程序编辑】下的【编辑】栏内的【复制】，如图6.8所示。
#### 图6.8：功能位置

功能说明：对选中的文本内容进行复制。

6.3.4. 剪切

位置：【程序编辑】下的【编辑】栏内的【剪切】，如图6.9所示。
#### 图6.9：功能位置

功能说明：对选中的文本内容进行剪切。

6.3.5. 粘贴

位置：【程序编辑】下的【编辑】栏内的【粘贴】，如图6.10所示。
#### 图6.10：功能位置

功能说明：将复制或剪切的内容进行粘贴。

6.3.6. 查找

位置：【程序编辑】下的【编辑】栏内的【查找】，如图6.11所示。
#### 图6.11：功能位置

功能说明：输入需要搜索的目标文字进行查找。

6.3.7. 替换

位置：【程序编辑】下的【编辑】栏内的【替换】，如图6.12所示。
#### 图6.12：功能位置

功能说明：可将目标内容替换为新的编写内容。

6.3.8. 保存

位置：【程序编辑】下的【编辑】栏内的【保存】，如图6.13所示。
#### 图6.13：功能位置

功能说明：将编辑好的机器人程序代码进行保存。

6.3.9. 机器人变量表

位置：【程序编辑】下的【编辑】栏内的【机器人变量表】，如图6.14所示。
#### 图6.14：功能位置
#### 功能说明：用于添加机器人轨迹添加时用到的一些信号地址。
### 指令
##### 运动

位置：【程序编辑】下的【指令】栏内的【运动】，如图6.15所示。
#### 图6.15：功能位置

功能说明：用于添加机器人的运动指令，包含MoveAbsJ、MoveJ、MoveL以及MoveC等指令。

*Move-Line：机器人以线性移动方式运动至目标点，当前点与目标点二点为一条直

线，机器人运动状态可控，运动路径保持唯一。

*Move-Joint：关节运动指令，表示的是机器人做关节运动，按照关节角度值来达到指定的点。机器人以最快捷的方式运动到目标点，机器人运动状态不完全可控，但运动路径保持唯一，常用于机器人在空间大范围移动。

*MoveC：全称是Move-Circle，为圆弧运动指令，机器人通过中间点以圆弧移动方式运动目标点，当前点、中间点与目标点三点决定一段圆弧，机器人运动状态可控，运动路径保持唯一。

*Move-AbsJoint：绝对运动指令，按照角度指令来移动。
##### 控制

位置：【程序编辑】下的【指令】栏内的【控制】，如图6.16所示。
#### 图6.16：功能位置

功能说明：可以添加一些机器人代码的逻辑控制指令和函数，包含IF、WHILE、FOR、Main等指令。
##### IO

位置：【程序编辑】下的【指令】栏内的【IO】，如图6.17所示。
#### 图6.17：功能位置
#### 功能说明：用于添加机器人可识别的一些信号指令，包含Set、Reset、WaitDI、WaitDO、WaitTime等指令。
##### 运算

位置：【程序编辑】下的【指令】栏内的【IO】，如图6.18所示。
#### 图6.18：功能位置

功能说明：可以添加一些机器人的逻辑运算符号，包含加号、减号、等于、大于、小于等符号。
### 调试

功能说明：在虚拟仿真流程中，进行虚拟仿真流程的检查、启动、暂停、停止。
### 程序输出
##### 输出

位置：【程序编辑】下的【程序输出】，如图6.19所示。
#### 图6.19：功能位置

功能说明：可将轨迹同步后生成的控制程序文件输出至电脑其他磁盘位置处。
##### 传送至控制器

位置：【程序编辑】下的【程序输出】，如图6.20所示。
#### 图6.20：功能位置

功能说明：可将轨迹同步后生成的控制程序文件传输至机构指定的控制器。
### 6.7.下载程序

位置：【程序编辑】下的【下载程序】，如图6.21所示。
#### 图6.21：功能位置
#### 功能说明：通过输入用户名及文件路径进行程序下载。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image240.png)
图6.22 下载程序对话框
## 显示
### 显示
###### 管理树

位置：在【显示】中，如图7.1所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image241.png)
图7.1：功能位置

功能说明：控制机器人加工管理面板的显示与隐藏。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image242.png)
图7.2：管理树界面
###### 控制面板

位置：在【显示】中，如图7.3所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image241.png)
图7.3：功能位置

功能说明：控制调试面板、输出面板和机器人控制面板的显示或隐藏。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image243.png)
图7.4：控制面板
###### 显示全部

位置：在【显示】中，如图7.5所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image241.png)
图7.5：功能位置

功能说明：将绘图区中隐藏的模型对象全部显示出来。
###### 7.1.4地面

位置：在【显示】中，如图7.6所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image241.png)
图7.6：功能位置

功能说明：地面可以提高软件的体验度，使仿真环境看起来更加真实，地面还提供了编辑功能，用户可以在选项中的文档显示页面，选择是否显示地面和网格，修改地面和网格的大小和颜色，如图7.7所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image244.png)
图7.7：地面
###### 7.1.5显示时序图

位置：在【显示】中，如图7.8所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image241.png)
图7.8：功能位置

功能说明：显示所有机构的时序顺序。
###### 7.1.6拖曳线

位置：在【显示】中，如图7.9所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image241.png)
图7.9：功能位置

功能说明：用于显示出机器人不同轴、法兰和工具TCP点的运行轨迹，通过勾选对应的显示位置，会自动生成机器人轨迹的运行路径，基于此运行路径可以更好的规避机器人发生碰撞的情况，如图7.10所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image245.png)
图7.10：拖曳线
## 多机协同
### 设置
##### 协同设置
#### 位置：在【多机协同】中的【设置】下，如图8.1所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image246.png)
图8.1：功能位置

功能说明：单击功能面板上“多机协同/协同设置/创建新系统”，新系统起个名字，比如叫“上船”。注意三个机器人在新系统内的次序，必须是KMC_MASERT、slave1、slave2的次序，否则后置的出的KUKA机器人的代码内，同步指令因参数错误会报错。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image247.jpeg)
图8.2：协同设置
##### 同步指令
#### 位置：在【多机协同】中的【设置】下，如图8.3所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image246.png)
图8.3：功能位置

功能说明：单击功能面板上的“多机协同/同步指令”，找到三个机器人上需要设置为同步的三段轨迹，通过选择设置，把他们集中到一列内；在勾选是否同步复选框的同时，设置同步名称，从而完成轨迹同步指令的设置。（三段轨迹内，每个点都会加上同步指令，且同步变量的名称会自动添加编号）

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image248.jpeg)
图8.4：同步指令
##### 同步设备速度
#### 位置：在【多机协同】中的【设置】下，如图8.5所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image246.png)
图8.5：功能位置
#### 功能说明：首先输入需要进行多机协同的“辅设备”名字，设置主设备与辅设备的关系，其次设置重置速度，点击“确定”，完成同步设备速度的设置。
#### 图8.6：同步设备速度
##### 同步轨迹速度
#### 位置：在【多机协同】中的【设置】下。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image246.png)
图8.7：功能位置
#### 功能说明：根据需求分别选取Master轨迹、Slave1轨迹及Slave2轨迹，设置完成后，点击“确定”，完成同步轨迹速度的设置，如图8.8所示。
#### 图8.8：同步轨迹速度
## 二次开发
### 自动化
##### 运行Python脚本

位置：在【二次开发】下的【自动化】中，如图9.1所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image251.png)
图9.1：功能位置
#### 功能说明：自行导入编程好的Python程序，可选文件格式有txt Files / python Files两种，导入完成后，运行Python脚本。
#### 图9.2：功能面板
##### 扩展指令

位置：在【二次开发】下的【自动化】中，如图9.3所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image251.png)
图9.3：功能位置

功能说明：

（1）此功能类似可参数化的自定义事件的添加，通过选择一个轨迹点，然后点击自定义事件，输入对应得参数，生成此轨迹点对应得事件内容；

（2）此功能可通过用户自己配置对应的参数格式，不同机器人的参数要求以及格式要求是不一致的，因此需要用户针对不同品牌的不同系统，配置针对性的参数文件；

（3）其中“Catalogue.xml”文件为控制选择指令界面的文件，所有的指令内容需要在此文件中配置；而其他的文件均为参数设置界面的文件，每个指令的具体参数设置均在对应的文件中配置；

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image253.png)
图9.4：选择指令

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image254.png)
图9.5：参数设置界面

配置文件位置：C:\ProgramFiles\CHLRob\PQArt\Ent\bin\RobotArt\zh-CN\Process\Custom；

*绿色部分表示安装路径的磁盘目录，默认安装路径为C盘，安装路径以用户实际安装目录为准；

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image255.png)
图9.6：配置文件目录
##### 导入轨迹特征

位置：在【二次开发】下的【自动化】中，如图9.7所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image251.png)
图9.7：功能位置

功能说明：此功能需要配合编辑轨迹特征中的【保存轨迹特征】和生成轨迹中的【轨迹后处理】使用，将一条轨迹中的特征选中并保存轨迹特征，然后通过导入轨迹特征将所保存的特征再次导入到软件当中，再次导入的特征可以通过生成轨迹时的轨迹后处理处选择添加，从而使新生成的轨迹直接具有上一条轨迹保存出去的特征属性，如图9.8所示。
#### 图9.8：保存轨迹特征
##### 使用轨迹模板

位置：在【二次开发】下的【自动化】中，如图9.9所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image251.png)
图9.9：功能位置

功能说明：导入所需的轨迹模板，并选取需要操作模型的坐标系，点击“确定”完成设定。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image257.png)
图9.10：功能面板
## 帮助
### 帮助

位置：在【帮助】中，如图10.1所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image258.png)
图10.1：功能位置

功能说明：

PQArt会员信息：显示PQArt账号的基本信息，包括用户角色，账号剩余天数，账号注册、激活、截止时间等。

个人信息：展示并支持修改用户个人信息：姓名、性别、单位等。

安全设置：用于PQArt账号绑定手机、QQ、微信、邮箱等；显示/修改用户名、密码等。

使用帮助：学习软件教程；疑难解答

个人资产：显示PQ币的数量；了解赚币攻略；赚取PQ币

消息中心：查看并处理系统消息与互动消息。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image259.png)
图10.2：功能界面
### 关于

位置：在【帮助】中，如图10.3所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image258.png)
图10.3：功能位置

功能说明：

更新版本：用于将软件更新到最新版本；

切换账户：使用其他账户登陆软件；

退出登录：退出当前账号；

重登录：重新登陆账号。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image260.png)
图10.4：功能界面
## 机器人加工管理
### 管理面板

机器人加工管理面板主要是全局浏览软件中所有模型和操作，使所有目标对象方便管理、简便操作以及直观清晰地查看，如图11.1所示。

位置：位于软件界面左侧。

功能说明：面板下挂有十个节点，包括场景、零件、坐标系、外部工具、快换工具、法兰工具、底座、状态机、机器人以及工作单元。机器人下还有坐标系、工具、底座、轨迹和程序等子节点。

点开查看该条目下的子节点；点击收起子节点列表。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image263.jpeg)
图11.1：机器人加工管理面板

一般来说，每个子节点的右键菜单中都包括了该对象的所有操作，快捷方便地执行多种指令。

【工作的设备】选择处于工作状态的设备（机器人）。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image264.png)
图11.2：选择当前工作设备

【坐标系】通过该功能，选中工具的三维球的朝向，可以在自身坐标系朝向和参照全局坐标系朝向之间进行自由切换。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image264.png)
图11.3：选择参考坐标系
### 场景

一般情况下绘图区为空，需要先导入工作设备和执行对象，包括机器人、工具、零件、底座、状态机等，即进行场景搭建，如图11.4所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image265.png)
图11.4：场景搭建菜单栏
### 零件

机械中不可分拆的单个制件，是机器的基本组成要素，也是机械制造过程中的合格的具有一定功能的物件，通过零件的组合能构成部件，部件组合能构成为产品。在PQArt中，零件的格式为robp。
##### 11.3.1抓取（生成轨迹）和抓取（改变状态—无轨迹）
#### 位置：零件的右键菜单内。

功能说明：

|  | 抓取（生成轨迹） | 抓取（改变状态-无轨迹） |
| --- | --- | --- |
| 应用场景 | 零件抓取机器人/零件抓取零件 |  |
| 基本概念 | 有轨迹显示 | 无轨迹显示 |
| 二者区别 | 一种动作，零件会根据该指令运动。生成的轨迹其实只有一个轨迹点。 | 一种状态，无动作的产生 |

操作对象是机器人时

机器人和工具也有这两个指令，但区别在于：机器人和工具使用该指令抓取零件时，机器人做的是关节运动（局部运动）；但使用零件的【抓取】指令，机器人做的是整体运动。

如在图示场景中，要达到机器人被底座托着顺着导轨左右移动的效果，需让底座抓取机器人。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image266.jpeg)
图11.5：零件的抓取

右击底座，选择下拉菜单中的【抓取（改变状态-无轨迹）】

选中“ABB-IRB120”，点击，将其添加到“已选择物体”中后，点击【确认】

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image268.png)
图11.6：零件抓取操作步骤

这时零件底座已经抓取了机器人，在导轨上移动时，机器人也会随之而动。

操作对象是零件时

以机器人上下料为例，让推杆推动小滑块到传送带上，这时需要先让推杆抓取小滑块。详细的操作步骤见图示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image269.jpeg)
图11.7：零件抓取操作步骤
##### 11.3.2放开（生成轨迹）和放开（改变状态—无轨迹）
#### 位置：零件右键菜单内。
#### 功能说明：

| 应用场景 | 零件放开机器人/零件放开零件 |  |
| --- | --- | --- |
| 基本概念 | 有轨迹显示 | 无轨迹显示 |
| 二者区别 | 一种动作，机器人会根据该指令运动。生成的轨迹其实是一个轨迹点。 | 一种状态，无动作的产生 |
##### 11.3.3添加抓取点
#### 添加的步骤如下图所示：
#### 图11.8：添加CP点步骤

选择要固定的姿态：

这里提供了三种附着点的姿态，设置的是抓取时机器人的抓取姿态。

一般情况下的抓取规则：工具TCP的Z轴与CP点的Z轴相对，两者的X轴同向，Y轴反向。

XYZ都不变：机器人抓取时按照一般情况下的抓取规则抓取；

Z不变，X可反向：抓取时如遇到不可达或者其他障碍情况，机器人可打破一般抓取规则，抓取方向为CP点X轴旋转180°的方向。

Z不变，XY任意：此种设定让机器人的抓取姿态更为灵活。根据零件的位置，机器人可不受限制地选择抓取的方向。
#### 图11.9：编辑CP点步骤

添加完CP点后，效果如下图所示：

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image272.png)
图11.10：生成的CP点
##### 11.3.4编辑零件特征

在编辑零件窗口中输入所需参数，进行零件特征的编辑，如图11.11所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image273.png)
图11.11：编辑面板
##### 11.3.5编辑草图位置
#### 位置：带有草图的零件右键菜单内。
#### 功能说明：【编辑草图】功能只在带有草图的零件右键菜单内出现，该指令的主要作用是可对零件上的草图进行二次修改、编辑。
#### 使用方法：
#### 通过【输入】功能导入stp格式的零件模型。
#### 模型导入后：
#### 图11.12：导入效果
#### 在模型上创建草图，新创建的草图节点会显示在“场景”下；
#### 多选两个场景文件，右击，选择【装配】，将其装配成为一个场景；
#### 将装配文件定义成零件；
#### 图11.13：功能面板及效果

右击【加工零件】，即可选择【编辑草图】
##### 11.3.6 插入POS点
#### 位置：零件右键菜单内。

功能说明：零件的POS点指的是驱动点，也就是驱动零件移动的点。

使用方法：移动零件时，在初始位置插入POS点1，之后利用三维球将零件定位到目标位置，在目标位置插入POS点2。插入两个POS点后，零件便会生成移动轨迹。

*插入的POS点被视为轨迹点，POS点的右键菜单中包含了诸多与轨迹点相同的操作指令。

示例

以为零件小滑块插入POS点为例

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image278.jpeg)
图11.14：小滑块前后位置的对比

右击小滑块，选择下拉菜单中的【插入POS点】。之后就可以在机器人加工管理面板中看到插入驱动点的特征。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image279.png)
图11.15：小滑块的树形图特征

将小滑块拖动到图示目标位置，插入驱动点2，仿真，可以看到小滑块从顶部垂直下落到底部的整个过程。
##### 11.3.7速度设置

设置零件的线速度和角速度，如图11.16所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image280.png)
图11.16：功能界面
##### 11.3.8三维球调整（零件）
#### 功能说明：三维球调整即通过三维球调整零件的位置和姿态，使得零件即使处于被抓取状态也可自由调整位姿。

抓取状态时零件初始位置如下图：

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image281.png)
图11.17：零件抓取状态

三维球调整，向上平移零件后：

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image282.png)
图11.18：零件“三维球调整”后的状态

该功能也可调整未被抓取的零件，只是这种情况下与选中零件弹出三维球的效果一样。

“三维球调整”后零件位置发生变化，但零件CP相对工具位置并没变动。
##### 11.3.9添加至工作单元

功能说明：将编辑好的零件添加至已有的工作单元或输入名称新建工作单元，点击“确定”完成设定，如图11.19所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image283.png)
图11.19：功能面板
##### 11.3.10重置局部坐标系

功能说明：根据加工需求，不需要更改整体坐标系，重新设置零件所需部分的局部坐标系。
##### 11.3.11复制

功能说明：进行物料/零件的复制，复制生成一个参数设置相同的零件。
##### 11.3.12另存零件
#### 功能说明：有选择地另存零件和零件上关联的轨迹（只保存零件，还是零件+轨迹一块保存），实现零件和轨迹的导出和重复利用，如图11.20所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image284.png)
图11.20：“另存零件”
##### 11.3.13隐藏，显示，删除和重命名

功能说明：

- 隐藏：隐藏当前选中的零件。隐藏后，零件会消失在绘图区，且机器人加工管理面板中的零件节点变成灰色；

- 显示：将已隐藏的零件显示出来。方法是再次选中机器人加工管理面板中的零件节点，右击，选择【显示】，零件会重新出现在绘图区；

- 删除：删除当前已导入的零件；

- 重命名：修改当前零件的名称。
##### 11.3.14几何属性
#### 位置：位于零件的右键菜单内。
#### 功能说明：“几何属性”用来查看/修改工具的材质，颜色以及透明度等。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image285.png)
图11.21：功能界面
##### 11.3.15自定义菜单

自行设置菜单功能栏

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image286.png)
图11.22：功能界面
### 坐标系
##### 11.4.1 PQArt中的坐标系

世界坐标系：整个环境界面的坐标系，多数情况下位于机器人足部，一般可自由定义。

基坐标系：用于表明工件或者工装在世界坐标系中的位置，可自由定义。

法兰坐标系：固定于机器人的法兰盘上，是工具的原点（一般常见的法兰坐

标系都是Z轴朝外，X轴朝下）

工具坐标系：即工具的中心点，可自由定义。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image287.png)
图11.23：坐标系示意

工件坐标系：表示工件的位置，默认表示在世界坐标系中。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image288.png)
图11.24：工件坐标系
##### 11.4.2编辑工件坐标系

位置：新建的坐标系会显示在机器人加工管理面板中的“坐标系下的用户坐标系”节点之下。

功能说明：可实现工件坐标系的编辑、复制、删除、隐藏、显示、重命名等功能，还可查看或更改属性，如图11.25所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image221.png)
图11.25：工件坐标系右键菜单

编辑：编辑工件的位置和姿态，可用来进行工件校准。X Y Z Q1 Q2 Q3 Q4等参数需要在真实环境中在示教器上测得，然后填入软件中，代表的是工件相对于机器人的位置和姿态。工件坐标系校准与三点法工件校准效果是一样的，可根据需要选用。

*编辑坐标系时场景中一定要有机器人存在。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image222.png)
图11.26：“工件坐标系校准”界面

修改关联工件位置：工件坐标系是否与工件相关联。

复制：复制当前选中的工件坐标系。复制的坐标系会与原坐标系重合。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image223.png)
图11.27：复制工件坐标系

删除：将新建的工件坐标系删除。

隐藏：隐藏当前选中的工件坐标系。隐藏后，工件坐标系消失在绘图区，机器人加工管理面板上的坐标系节点变成灰色。

显示：将已隐藏的工件坐标系显示出来。

重命名：修改所选工件坐标系的名称。

属性：选定坐标系关联的工件。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image224.png)
图11.28：工件坐标系属性
##### 11.4.3轨迹关联坐标系

每条轨迹可根据需要关联不同的坐标系，后置时也可以显示出点关联的坐标系。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image289.png)
图11.29：“选项”界面

功能说明：在“使用坐标系”中，可选择当前轨迹所关联的坐标系。下拉列表中会显示出绘图区中存在的所有坐标系。
##### 11.4.4 DH坐标系

DH坐标系：机器人每个连杆上的一个固定坐标系，每个坐标系都描述了相邻两连杆的空间关系，并表示了每个连杆在空间中的位置和姿态。

在PQArt中，DH坐标系的应用包括：在定义机构和定义机器人的过程中，通过DH参数建模、建立DH坐标系来定义。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image290.png)
图11.30：定义机器人面板

显示/查看机器人各个轴的位置和姿态：

机器人右键菜单的【属性】中，选择是否显示出官方机器人/自定义机器人的DH参数。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image291.png)
图11.31：DH坐标系的显示与隐藏
### 外部工具

外部工具：独立于机器人之外的工具，如打磨机、砂轮等。有时机器人需要手持工件配合使用外部工具。

安装方式：外部工具从【工具库】中导入，导入后即可独立于机器人之外，配合机器人进行零件的加工。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image292.png)
图11.32：外部工具
### 快换工具
#### 快换工具：由机器人侧用和工具侧用组成。机器人侧用指的是与机器人法兰盘连接的工具，工具侧用指的是与法兰工具连接的工具。当机器人需要完成两种及以上的任务时，通过快换工具可以快速更换工具，而不用从法兰盘上拆下工具，省时省力。

安装方式：工具侧用从【工具库】中导入，导入后需要执行安装操作（通过工具右键菜单的[安装]指令），才能安装到机器人侧用工具上。
#### 图11.33：快换工具

快换工具的安装：导入快换工具后，详细的安装步骤见下图：

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image294.jpeg)
图11.34：快换工具安装步骤

安装好后的快换工具如下图所示：

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image295.png)
图11.35：快换工具安装图

对于快换工具来说，导入后还需要手动安装到法兰工具上去。

命令位置：位于快换工具的右键菜单内。

功能说明：导入快换工具后，单击快换工具的右键菜单，选择【安装（生成轨迹/改变状态-无轨迹）】；卸载快换工具时，选择右键菜单内的【卸载（生成轨迹/改变状态-无轨迹）】。

|  | 安装（生成轨迹） | 安装（改变状态-无轨迹） |
| --- | --- | --- |
| 应用场景 | 安装快换工具时 |  |
| 基本概念 | 安装工具、同时生成轨迹 | 安装工具、但不生成轨迹 |
| 二者区别 | 一种动作，机器人会根据该指令运动 | 一种状态，无动作的产生 |
| 实例 | 可看到运动的轨迹 | 无任何动作，只是状态 |

|  | 卸载（生成轨迹） | 卸载（改变状态-无轨迹） |
| --- | --- | --- |
| 应用场景 | 卸载快换工具时 |  |
| 基本概念 | 卸载工具、同时生成轨迹 | 卸载工具、但不生成轨迹 |
| 二者区别 | 一种动作，机器人会根据该指令运动 | 一种状态，无动作的产生 |
| 实例 | 可看到运动的轨迹 | 无任何动作，只是状态 |
### 法兰工具

法兰工具：安装在机器人法兰盘上的工具。
#### 法兰盘：通常是指在一个类似盘状的金属体的周边开上几个固定用的孔，用于和机器人六轴末端的法兰进行装配。

安装方式：法兰工具从【工具库】中导入，导入后即直接安装在机器人的法兰盘上。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image300.png)
图11.36：法兰工具
### 底座

底座概念：底座是机器人底部的承接块。PQArt支持的底座格式为robs。

底座作用：作为机器人的基座，用来固定机器人，或者调节机器人的高度。

功能说明：通过【设备库】将底座导入后，底座会自动安装到机器人基座之下。
#### 图11.37：底座安装示意图
#### *导入底座之前需先导入机器人。多机器人环境下，底座默认插入到当前激活的机器人底部。
##### 11.8.1 安装底座
#### 位置：位于底座的右键菜单内
#### 功能说明：可以将机器人按照设置好的角度安装到底座上，如图11.38所示。
#### 图11.38：安装底座界面
##### 11.8.2 隐藏，显示，删除和重命名
#### 位置：位于底座的右键菜单内。
#### 功能说明：

- 隐藏：隐藏当前选中的底座。隐藏后，底座会消失在绘图区，且机器人加工管理面板中底座的节点变成灰色；

- 显示：将已隐藏的底座显示出来。方法是再次选中机器人加工管理面板中的底座节点，右击，选择【显示】，零件会重新出现在绘图区；

- 删除：删除当前已导入的底座；

- 重命名：修改当前底座的名称。
##### 11.8.3 替换底座
#### 位置：位于底座的右键菜单内。

功能说明：“替换底座”即将当前的底座替换为另外的新的底座。新底座既可以从软件的底座库中选择，也可以导入自定义的底座。
##### 11.8.4 几何属性
#### 位置：位于底座的右键菜单内。
#### 功能说明：“几何属性”用来查看/修改底座的材质，颜色以及透明度等。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image303.png)
图11.39：几何属性界面
### 状态机

状态机是只有几种特定状态的机构。工作站中的仓储-托盘、加工-滑动门、打磨-转位夹具等都是状态机。如果需要这种状态机改变状态，需要在轨迹点上添加相应的【自定义事件】来驱动。同时，为方便调用，这些事件已经添加到工艺设置的自定义事件模板内，并且各状态机状态的命名上，采用了“状态机名称+状态事件名称”的形式命名，简单、易懂。
### 机器人
#### 机器人基本操作：导入机器人，回机械零点，同步到此机构，激活机器人，读取和保存关节值，抓取与放开，替换机器人，另存机器人。
#### 机器人高级属性：设置机器人，修改机器人，机器人属性，修改后置格式，逆解算法设置，默认速度设置，隐藏显示和重命名。
##### 11.10.1回机械零点

位置：位于机器人右键菜单内。

概念：机械零点即机器人出厂时的初始姿态。
#### 功能说明：对机器人进行一系列操作后，机器人各轴和初始姿态相差甚大，
#### 这时让机器人回到机械零点，比较容易进行新操作。“回到机械零点”的三种操作：

下图所示的机器人，部分轴已经经过旋转，不是初始状态，要使其回到机械零点状态有三种不同的操作：

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image304.png)
图11.40：ABB机器人的非零点状态
#### 选中机器人，右击，选择下拉菜单中的【回到机械零点】。
#### 选中机器人，单击右侧机器人控制面板上的【回机械零点】。
#### 将调试面板中机器人的关节角数值全部改为机器人出厂时的初始值（不一定都是0）。

回到机械零点后如下：

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image306.png)
图11.41：ABB机器人机械零点状态
#### * KUKA机器人回机械零点时J2为-90度，J3为90度。
##### 11.10.2编辑Home点

位置：机器人右键菜单内的“【编辑Home点】”。

功能说明：该命令可以将机器人的一些常用的姿态保存起来，以方便大批量轨迹添加时随时切换、调整机器的空间姿态，加速、简化轨迹的添加过程。

同时，通过【编辑Home点】命令，也可以对存储的Home点进行修改、删除等操作。
#### 图11.42：保存Home点界面
##### 11.10.3创建与解除外部轴链接

位置：机器人右键菜单【创建外部轴链接】【解除外部轴链接】。

功能说明：
#### 选中机器人，右击，然后单击右键菜单上的【创建外部轴链接】，即可展开“链接外部轴”设置界面， 从“直线导轨”下拉菜单选择想要与机器人链接的导轨，然后单击界面中的确定按钮，即可创建链接。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image308.png)
图11.43：机器人与导轨创建链接

选中机器人，右击，然后单击右键菜单上的【创建外部轴链接】，即可展开“链接外部轴”设置界面， 从“变位机”下拉菜单选择想要与机器人链接的变位机，然后单击界面中的确定按钮，即可创建链接。
#### 图11.44：机器人与变位机创建链接

解除外部轴链接：此命令可清空或解除已与机器人创建好的外部轴链接。
#### 图11.45：解除外部轴链接
##### 11.10.4按轴抓取
#### 可选取机器人模型不同的轴，实现抓取，如图11.46所示。
#### 图11.46：功能界面
##### 11.10.5抓取（生成轨迹）和抓取（改变状态—无轨迹）
#### 位置：位于机器人右键菜单内。

功能说明：

|  | 抓取（生成轨迹） | 抓取（改变状态-无轨迹） |
| --- | --- | --- |
| 应用场景 | 机器人抓取工件时 |  |
| 基本概念 | 抓取物体、同时生成轨迹 | 抓取物体、但不生成轨迹 |
| 二者区别 | 一种动作，机器人会根据该指令运动 | 一种状态，无动作的产生 |
| 实例：打磨 | 可看到运动的轨迹 | 无任何动作，只是状态 |
##### 11.10.6放开（生成轨迹）和放开（改变状态——无轨迹）
#### 位置：位于机器人右键菜单内

功能说明：

|  | 放开（生成轨迹） | 放开（改变状态-无轨迹） |
| --- | --- | --- |
| 应用场景 | 机器人卸载工件时 |  |
| 基本概念 | 放开物体、同时生成轨迹 | 放开物体、但不生成轨迹 |
| 二者区别 | 一种动作，机器人会根据该指令运动 | 一种状态，无动作的产生 |
| 实例：打磨 | 可看到运动的轨迹 | 无任何动作，只是状态 |

*使用【放开（改变状态-无轨迹）】后，虽然绘图区显示工具依然在抓着零件，但实际上两者已经分离了。因为选择的只是状态的改变，而不是动作的生成。
##### 11.10.7插入POS点
#### 位置：该功能位于机器人右键菜单内。
#### 功能说明：这里插入POS点的效果与右击工具插入POS点的效果是一样的。

POS点为过渡点，其实就是独立于轨迹之外的一个点，可以选择插入不同的POS点方式。

三种POS点的含义是什么？

| MoveL: Move-Line | 机器人以线性移动方式运动至目标点，当前点与目标点成为一条直线，机器人运动状态可控，运动路径保持唯一。 |
| --- | --- |
| MoveJ: Move-Joint | 机器人以最快捷的方式运动至目标点，机器人运动状态不完全可控，但运动路径保持唯一，常用于机器人在空间大范围移动。 |
| MoveAbsj: Move-Absjoint | 绝对运动指令，机器人按照角度指令来移动。机器人运动状态可控。 |

什么时候插入pos点？

插入POS点可应用于多种情况。在可达范围内，当机器人想要运动到某个点，或者想要按照某条轨迹这样那样运动，但是受到了各种因素的阻碍时就可插入pos点。
##### 11.10.8设置机器人
#### 功能说明：该功能是对机器人六个轴的关节角度转动范围、机械零点和轴配置进行设置。例如：在实际操作环境中为了防止机器人发生碰撞，可以通过改变轴限位的值，来限制各轴的活动范围。
#### 图11.47：功能界面

机械零点设置：改变机器人处于机械零点时各轴的关节角，即改变机器人机械零点状态。
##### 11.10.9设置工作方式
#### 功能说明：选择自主/协作的工作方式，协作工作时，需要选择与机器人协作的物体，如图11.48所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image318.png)
图11.48：功能面板
##### 11.10.10运动参数设置
#### 位置：该功能位于机器人右键菜单内。
#### 功能说明：
#### 默认速度设置：
#### 设置关节速度百分比，快速移动速度、加工速度、进退刀速度以及切入切出速度。
#### 图11.49：功能面板
#### 自定义参数设置：
#### 根据需求，自行设置参数名称以及参数值。
#### 图11.50：功能面板
#### 仿真公式设置：
#### 图11.51：功能面板
#### 运动学仿真设置：
#### 设置加速度，并选择内置或自定义算法进行运动学仿真。
#### 图11.52：功能面板
##### 11.10.11替换机器人/替换自定义机器人
#### 位置：位于机器人右键菜单内。
#### 功能说明：用于替换当前的机器人为其他目标机器人。
#### 替换机器人：从【选择机器人】界面中导入机器人，单击【插入】即可；
#### 替换自定义机器人：直接从本地导入自定义的机器人。
##### 11.10.12复制
#### 位置：位于机器人右键菜单内。
#### 功能说明：复制生成一个与机器人完全相同的机器人。
##### 11.10.13读取和保存关节值
#### 位置：位于机器人右键菜单内。
#### 功能说明：这里指的是“保存关节值”和“读取关节值”两个功能。
#### 保存关节值：用于保存机器人当前姿态的关节角，保存文件格式为txt。

读取关节值：从存储有机器人关节值的文件（txt）中导入机器人的关节角度值。
##### 11.10.14另存机器人
#### 位置：位于自定义机器人的右键菜单内。
#### 功能说明：自定义的机器人，即使已经插入应用到场景中，仍可以通过【修
#### 改机器人】命令对其修改。修改后的机器人，可通过该命令，将修改好的机
#### 器人重新另存出去。
##### 11.10.15 隐藏，显示，删除和重命名
#### 位置：位于机器人右键菜单内.

功能说明：这里指的是三个功能，详细说明如下：

隐藏：隐藏当前选中的机器人。单击后，机器人会从绘图区隐藏，且机器人加工管理面板中的机器人节点变灰。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image323.png)
图11.53：机器人的隐藏

显示：用于显示已隐藏的机器人。右击机器人加工管理面板中的机器人名称，选择右键菜单内的【显示】功能，机器人就会重新出现在绘图区。

删除：用于删除所选的机器人。

重命名：用于修改机器人的名称。
##### 11.10.16设置机器人属性
#### 位置：位于机器人右键菜单内。

功能说明：【机器人属性】界面分为三个标签页：基本信息，后置信息，显示设置。
### 轨迹
##### 11.11.1轨迹组（Group）

位置：位于右侧菜单栏中，点击【Group】，右键菜单，如图11.54所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image324.png)
图11.54：功能位置

1. 创建轨迹模板：创建一个可以基于参数快速生成特定路轨迹的方式；

1. 保存轨迹：将选中的单条轨迹单独保存到一个工程文件中。

1. 复制：复制轨迹组。

1. 复制轨迹到设备：复制该轨迹组到工作站中需要生成轨迹的设备。

1. 按轴复制轨迹：这里的轴指的是机器人的轴，按轴复制轨迹点即旋转/平移运动机构的一个轴到目标位置，同时复制选中的轨迹点，平移轴按距离复制，旋转轴按照弧度复制，简化了轨迹设计。

*该功能只针对Move-Absj点。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image325.png)
图11.55：功能界面

1. 按轴移动轨迹点：按照选定轴的方向来平移指定的距离。

*该功能只针对Move-Absj点。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image326.png)
图11.56：功能界面

如图11.56所示，（1）在机器人加工管理面板/调试面板上选中Move-Absj点，右击，选择菜单中的【按轴移动轨迹点】；（2）设置相关参数：选择轨迹点按照哪个轴进行移动；若轴类型为旋转轴，则“按轴移动量”的值为角度值，单位是°；若轴类型为平移轴，则“按轴移动量”的值为距离，单位为mm。

1. 修改轨迹点指令：该功能用于修改单条/多条轨迹的轨迹点指令，线速度和圆弧过渡。点指令包括Move-Line和Move-Joint。用户可选择性地修改轨迹的首点、中间点和末点。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image327.png)
图11.57：功能界面

*中间点指的是轨迹除首点和末点之外，其他的所有点。

1. 仿真轨迹：对选中的轨迹组进行仿真。

1. 后置：后置轨迹是将当前选中的单条/多条轨迹单独生成后置代码，方便根据 实际需求后置目标轨迹。

1. 注释：将暂时不参与运算的轨迹注释掉，暂时要保留、不参与仿真的轨迹，可以注释掉，注释的轨迹不参与后置、仿真和真机运行。

被注释的轨迹会变成灰色：

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image328.png)
图11.58：注释轨迹

取消注释：再次右击被注释的轨迹，可取消注释，恢复轨迹的仿真、后置效用。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image329.png)
图11.59：取消注释

1. 隐藏：将不需要显示的轨迹组隐藏掉，被隐藏的轨迹会变成灰色。

1. 显示：显示出被隐藏的轨迹组。

1. 删除：删除不需要的轨迹组。

1. 重命名：重新命名。

1. 合并至前一分组：将选中的轨迹组合并到上一个轨迹组内，类似效果就是将选中轨迹组取消掉。

*如果选中的轨迹组是第一个，启动该命令，会弹出拒绝的提示。

1. 属性：

轨迹显示：选择是否显示轨迹点和轨迹线

轨迹属性：设置轨迹的关联坐标系和TCP点。

轨迹速度设置：设置轨迹的速度，关节速度，快速移动和加工速度，进退刀速度以及切入切出速度等。

轴配置：用于直接查看当前激活的轨迹或机器人的轴配置信息，此处轴配置只用于快速查看，不能直接修改当前轨迹或机器人的轴配置。

联动求解：根据需求设置联动求解的方式。

自定义参数：支持自行添加相关参数，需要添加好参数名称和参数值，点击“确定”。

1. 自定义菜单

自行设置菜单功能栏

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image286.png)
图11.60：功能界面
##### 11.11.2轨迹

位置：位于右侧菜单栏中，点击任意轨迹的过渡点，右键菜单，如图11.60所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image330.png)
图11.61：功能面板

1. Z轴指向中心点：选中轨迹后，单机右键菜单内的“Z轴指向中心点”，会激活三维球；移动三维球，则所有轨迹点的Z轴朝向会统一指向三维球中心点的位置。达到统一调整轨迹点Z轴指向的目的。

1. 插入POS点：插入一个POS点会在工具TCP位置插入一个点，指令包括直线指令，关节指令和绝对关节指令三种。

1. 轨迹Z向投影：选中轨迹后，点击轨迹Z向投影，轨迹会向四周自动搜索零件，并在Z轴指向上向距离加工零件的最近位置进行投影。

1. 添加过渡轨迹：可以在选择轨迹之前新建一个过渡点，新建轨迹点姿态由此轨迹的第一个点和前一条轨迹最后一个点的姿态自动求解所得；

*首条轨迹不可添加过渡轨迹

1. 应用之前计算的偏差：用于配合多选轨迹菜单中的“计算两个轨迹的首点位置偏差”功能，基于求出的位置偏差，自动将轨迹基于第一个点的位置进行偏移；

1. 校准轨迹：用于对单条轨迹进行校准，拾取软件轨迹中的三个轨迹点，同时在实际对应轨迹中查看三个点坐标系并输入界面中，点击校准，即可实现校准轨迹操作；

1. 轨迹尾插入POS点：只在轨迹最后一个点后生成出刀点。

1. x轴与轴平行：可以控制生成轨迹后轨迹点的x轴和被激活的三维球的x轴相平行，其他轴尽可能不发生变化。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image332.png)
图11.62：功能效果展示

1. 运行Python脚本：自行导入编程好的Python程序，可选文件格式有txt Files / python Files两种，导入完成后，运行Python脚本。

1. 自定义特征：

通过导入Python脚本，可以实现在两个轨迹点之间自动生成一个轨迹点。同时用户还可根据自己的具体需求编写其他的Python脚本，实现不同的造点方式。

、

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image333.png)
图11.63：自定义特征效果

1. 打孔属性：对于一些表面没有孔位，但是想要在表面进行钻孔的模型，可在生成轨迹之后添加打孔属性。“往复起始位置”表示进刀和退刀的位置，“往复矢量”表示打孔深度。

1. 轨迹过盈：对于环形封闭轨迹，可将轨迹的起始位置和终点位置延长相应的距离，并且这段距离各个轨迹点之间的步长和之前保持一致。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image334.png)
图11.64：轨迹过盈点位

1. 轨迹点倾角：在焊接项目中，工业机器人的工具需和焊缝有一定角度的夹角，通过此功能可使轨迹的各个轨迹点姿态沿着加工方向进行前倾和侧倾，进而改变工具的加工姿态，满足焊接参数的要求；

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image335.png)
图11.65：轨迹点倾角

1. Z轴指向：选中轨迹后，单击Z轴指向，会激活三维球；移动三维球，则所有轨迹点的	Z轴朝向会统一指向三维球中心点的位置，达到统一调整轨迹点X轴指向的目的。

1. 添加仿真事件：可以给轨迹直接添加仿真事件，添加完成后，此条轨迹内的所有轨迹点后面均带有仿真事件。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image336.png)
图11.66：添加仿真事件

1. 三维球移动复制轨迹：选中轨迹后，右键启动该命令，会复制一份当前轨迹；后续通过三维球，即可将轨迹移动到新的位置；移动后的轨迹自动和被加工的零件重新建立关联。

需要注意的是：若机器人和导轨或变位机建立了链接，则这类轨迹被复制后，其外部轴的关节角度并没有变化。后续仿真时，会发生不可控联动效果。后续借助需要借助轨迹的右键菜单内的“批量修改外部轴关节角”命令，对复制轨迹内的外部轴关节角加以修改才可以。

1. 轨迹投影：选中轨迹后，点击轨迹投影，则轨迹会向四周自动搜索零件，并向其最近的位置进行投影，效果如下所示。

*投影都是自动进行，向距离加工零件的最近位置进行投影。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image337.jpeg)
图11.67：功能展示

1. 镜像复制轨迹：当加工的轨迹是对称结构时，可以使用该命令，快速生成对称面上的轨迹。

1. 轨迹点阵列：选中轨迹，启动该命令后，会弹出阵列个数设置，并弹出三维球，拖动三维球，即可设置阵列之间的间隔值。

1. X轴指向：选中轨迹后，单击X轴指向，会激活三维球；移动三维球，则所有轨迹点的	X轴朝向会统一指向三维球中心点的位置，达到统一调整轨迹点X轴指向的目的。

1. 统一位姿（使用当前姿态）：所有轨迹点的姿态与被编辑点的姿态相同，可以用来调整轴超限的点，优化轨迹姿态，减小了工具工作时扭动的幅度，尽量避免机器人和工具发生碰撞。

示例：以去毛刺为例

选中点1，右击，选择下拉菜单中的【统一位姿】后，在该点上弹出了三维球。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image338.png)
图11.68：功能示意图

用三维球对点的位姿进行微调，调整点1的时候，其他点的位姿也会随之而动，调整后效果如下：

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image339.png)
图11.69：功能效果图

*一般在平面上使用此功能的情况比较多。若在曲面上使用，其他轨迹点的姿态与所选择的轨迹点姿态一致，会导致加工方向（Z轴）不垂直于加工面。

1. 修改轨迹联动求解方式：联动求解方式有：常规；位置优先；自动链接；角度优先；Z轴朝上。

1. 多层多道：焊接一个零部件时，有电焊、打底焊、填充焊等焊工艺要求，特别是打底焊、填充焊还需要多层多道，并且焊接零部件的量还很大，示教起来很麻烦，为了解决这个问题，增加了该功能，该功能可以借助一个已经生成好的轨迹，以及模型自身，一次性生成指定间隔、层数的多层多道的焊接轨迹，从而使复杂的焊接轨迹的制作简单化。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image340.png)
图11.70：多层多道

1. 轨迹优化：对所选轨迹的整体调整，一方面解决轨迹中轴超限、奇异点等问题；另一方面可优化轨迹点的姿态。它默认地固定了此条轨迹所有点的Z轴，优化时是绕Z轴旋转一定的角度，角度的大小根据实际情况而定。

轨迹优化界面包括：轨迹点的个数，点的序号以及点绕Z轴旋转的角度。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image341.png)
图11.71：“轨迹优化”界面

*红点：不可达；黄点：轴超限；紫点：奇异点；粉色：碰撞检测；蓝色：突变检测

蓝线：表示的是所有轨迹点的集合。

鼠标在蓝色的水平线上移动时，轨迹点的序号也在改变。上下移动时，改变的是点的姿态，即绕Z轴旋转角度。

取消计算：用来终止计算，一般适用于轨迹点较多的轨迹。

开始计算：计算出轨迹中轴超限、不可达的点和奇异点，并以不同颜色的点显示在界面中。一次轨迹优化后，轨迹点姿态数据信息已保存，在此基础上可再次点击【开始计算】进行第二次优化。

确认调整：确认并保存当前对轨迹点姿态的调整。

关闭窗口：关闭优化窗口，直接关闭不会保存所做的任何调整。

优化方法：将蓝线拖动到黄色区域的空白区（机器人工作的最优区）。

1. 轨迹旋转：

旋转轨迹即让轨迹上的所有点旋转指定的角度，用于调整轴超限的点，或者改变轨迹姿态以满足其他要求，可选择性地决定让轨迹绕着XYZ三个方向旋转。

|  | 标准旋转 | 三维球旋转 |
| --- | --- | --- |
| 概念 | 通过对话框输入具体的旋转角度值，旋转角度根据实际情况填写，然后点击【确定】即可。 | 利用三维球来旋转整条轨迹。点击此指令后，三维球会默认弹出在轨迹的第一个点上。 |
| 区别 | 输入具体数值来进行旋转，比较精确。 | 可实时观察到轨迹点姿态和对其调整的效果，更加直观。 |
| 图示 |  |  |

1. 轨迹平移：

轨迹平移即将轨迹沿着XYZ三个坐标轴的方向平移一定距离。

|  | 标准平移 | 三维球平移 |
| --- | --- | --- |
| 概念 | 通过对话框输入具体的平移角度值，平移距离根据实际情况填写，然后点击【确定】即可。 | 利用三维球来平移整条轨迹。点击此指令后，三维球会默认弹出在轨迹的第一个点上。 |
| 区别 | 输入具体数值来进行平移，比较精确。 | 可实时观察到轨迹点姿态和对其调整的效果，更加直观。 |
| 图示 |  |  |

1. 轨迹反向：轨迹反向是指轨迹的起始点变为终点，终点变为起始点，此指令可使机器人运动路径反向。

1. Z轴固定：轨迹中所有点的三个坐标轴与第一个点的对应的三个坐标轴平行。Z轴固定可使工具转动幅度变小，从而不易发生碰撞。同样适用于调整轴超限的轨迹点。

1. Z轴旋转最小：

Z轴旋转最小是指在Z轴不变的前提下，使x、y轴的变化是最小的，这种变化都是基于第一个加工的点来说的，从图中可以看出，x、y轴的指向基本上是不变的。这是为了尽可能使6轴的旋转最小，从而防止轴超限的现象发生。

z轴旋转最小（前）          z轴旋转最小（后）

图11.72：功能展示

1. 轨迹点按距离排序：根据两个轨迹点之间的步长距离进行轨迹点位置的排序；

1. X/Y轴反向：以Z轴为中心，X轴旋转180度，Y轴旋转180度。

1. 批量修改外部轴关节角：

主要是对于含有外部轴，如变位机、导轨的轨迹，通过“三维球移动复制轨迹”后，外部轴的关节并没有变化，需要通过该命令将三维球的外部轴的关节角修改为新位置时的值，否则机器人仿真时，就会出现不可控的联动仿真。

1. 创建和重命名分组：创建分组，对单条/多条轨迹进行分组。因为实际操作中需要对工件分区域加工，添加分组更方便管理轨迹。

示例：右键单击单条/多条轨迹，对其进行分组。

1. 对前端或后端的单条/多条轨迹分组：

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image345.png)
图11.73：轨迹分组

1. 对中间的单条/多条轨迹分组，则所选轨迹之后会自动被分到下一组，如轨迹4和轨迹5：

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image346.png)
图11.74：轨迹分组

1. 移动复制轨迹：将选择的轨迹按照轨迹点坐标系的X或者Y方向，并选择轨迹所在实体，复制并移动相应的步长；

1. 复制轨迹：对选中的单条/多条轨迹进行复制，用于执行相同/相近的轨迹操作，可避免了二次生成相同轨迹的繁琐。复制的轨迹与原轨迹在位置和姿态上完全一致。

1. 复制轨迹到设备：复制该轨迹到工作站中需要生成轨迹的设备。

1. 按轴复制轨迹：这里的轴指的是机器人的轴，按轴复制轨迹点即旋转/平移运动机构的一个轴到目标位置，同时复制选中的轨迹点，平移轴按距离复制，旋转轴按照弧度复制，简化了轨迹设计。

*该功能只针对Move-Absj点。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image325.png)
图11.75：功能界面

1. 按轴移动轨迹点：按照选定轴的方向来平移指定的距离。

*该功能只针对Move-Absj点。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image326.png)
图11.76：功能界面

如图11.56所示，（1）在机器人加工管理面板/调试面板上选中Move-Absj点，右击，选择菜单中的【按轴移动轨迹点】；（2）设置相关参数：选择轨迹点按照哪个轴进行移动；若轴类型为旋转轴，则“按轴移动量”的值为角度值，单位是°；若轴类型为平移轴，则“按轴移动量”的值为距离，单位为mm。

1. 轨迹往复：机器人运行完原轨迹后，反方向再次运行该条轨迹，一般应用与精细加工时对零件反复进行加工。该功能支持设定轨迹往复次数。

如打磨工艺中需要使用【轨迹往复】来反复打磨一个面。

打孔时使用【轨迹往复】来打孔。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image347.png)
图11.77：轨迹往复

1. 插入POS点：插入一个POS点会在工具TCP位置插入一个点，指令包括直线指令，关节指令和绝对关节指令三种。

1. 生成出入刀点：在轨迹的起始点和终点分别生成一个点作为工具的入刀点和出刀点，符合实际工艺需求，可使机器人尽量避免发生碰撞。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image348.png)
图11.78：功能界面

出入刀偏移量：工具出刀点和入刀点分别距离第一个轨迹点和最后一个轨迹点的距离，单位是mm。

闭环轨迹的出入刀点：

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image349.png)
图11.79：功能展示

直线轨迹的出入刀点：

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image350.png)
图11.80：功能展示

1. 切入切出：通过该命令，可以实现刀具加工时切入和切出时的方向，按预显设定的轴向（X正反方向、Y正反方向、Z正反方向），进行直线切入切出或圆弧切入切出轨迹的添加。

偏移量的设置，需参考当前选中轨迹内轨迹点的坐标朝向，使用该功能时，选中轨迹内的轨迹点的坐标会显示出来，以供设置偏移量及决定其正负。比如：将来要生成的入刀点或出刀点，相对于当前高亮的坐标系，位于其某个轴的负方向上，则选择该轴后，偏移量应该输入负值，反之，需输入正值。

1. 进刀和过切设置：

该功能界面分为“进刀设置”和“过切设置”两部分。

进刀设置：用于生成到达原轨迹前的进刀轨迹路径。进刀量：进刀轨迹起始层到达原轨迹时需要进刀的总量，单位mm。步长：进刀轨迹间进刀的间隔量，单位mm；

过切设置：用于生成超越原轨迹的过切轨迹路径。过切量：原轨迹到达过切轨迹最底层时产生过切的总量，单位mm。步长：过切轨迹间过切的间隔量，单位mm。

进刀为在目标轨迹点前生成n组点，n=进刀量/步长。进刀点为目标轨迹点沿z轴正向移动步长距离得到的点。同理，过切点为目标轨迹点沿z轴负向移动步长距离得到的点。新加的点依次放在新的点分组里。

1. 修改轨迹点指令：

该功能用于修改单条/多条轨迹的轨迹点指令，线速度和圆弧过渡。点指令包括Move-Line和Move-Joint。用户可选择性地修改轨迹的首点、中间点和末点。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image327.png)
图11.81：功能界面

*中间点指的是轨迹除首点和末点之外，其他的所有点。

1. 轨迹仿真：

1. 仿真此轨迹：对当前选中的单条轨迹进行仿真。

1. 从此轨迹开始仿真：对当前选中的单条轨迹及其以后的轨迹进行仿真。

1. 单机构运动到点和多机构运动到点：在多机器人环境下，选中某个机器人的某个轨迹点后，想查看机器人运动到该点时的轨迹求解状况，目前有两种办法：

单机构运动到点：该轨迹点对应的机器人、机构单独运行到该点，其他机器人，机构静止不动。

多机构运行到点：当该轨迹点对应的机器人、机构运行到该点的时间段内，场景中其余的所有机器人、机构会做同步运动。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image351.jpeg)
图11.82：“单机构/多机构运动到点”对比图

备注：图中列举了机器人A，分别通过两种方式运动到B点的不同情形；单机器人场景下，分别通过这两种方式运行到点，效果一样。

1. 更多操作：

1. Z轴反向：以X轴为旋转中心，Z和Y两轴旋转180度，可对工具加工方向（Z轴）进行调整。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image352.png)
图11.83：功能效果图

1. XY轴固定：XY轴形成的平面是不动的，同时Z轴的指向不变但是Z轴可以旋转。

1. 保存轨迹：将选中的单条轨迹单独保存到一个工程文件中。

1. 后置轨迹：后置轨迹是将当前选中的单条/多条轨迹单独生成后置代码，方便根据实际需求后置目标轨迹。

1. 注释：将暂时不参与运算的轨迹注释掉，暂时要保留、不参与仿真的轨迹，可以注释掉，注释的轨迹不参与后置、仿真和真机运行。

被注释的轨迹会变成灰色：

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image328.png)
图11.84：注释轨迹

取消注释：再次右击被注释的轨迹，可取消注释，恢复轨迹的仿真、后置效用。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image329.png)
图11.85：取消注释

1. 添加工件关联：关联指的是位置和几何上的关联。通俗来说是轨迹会随着工件的位置移动而移动，并且轨迹可根据工件的改变自动更新轨迹数据，即工件尺寸变大，轨迹可自动更新无需编辑操作。一般情况下，轨迹和工件都是相互关联的。

1. 取消工件关联：【取消工件关联】用三维球移动工件，轨迹还在原来的地方，不会跟着工件移动。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image353.png)
图11.86：取消工件关联

选中轨迹，右击选择【添加工件关联】后，在弹出的对话框中选择“气缸”。轨迹和零件又会重新关联上。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image354.png)
图11.87：选择关联的工件

*有一种调特殊情况：当轨迹是自己导入，而不是在PQArt中生成的时候，轨迹和工件是不关联的。这时，选择【添加工件关联】，那么两者就会相互关联了。

1. 合并轨迹至前一个轨迹：指的是将后面的单条/多条轨迹合并到前一个轨迹。

示例：以下图所示的轨迹8和轨迹9为例。

右击轨迹9，选择【合并至前一个轨迹】

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image355.png)
图11.88：功能展示

这时可以看到，轨迹9没有了，轨迹8中的“曲线特征”等变成了“基本方式生成轨迹”。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image356.png)
图11.89：功能展示

生成的“基本方式生成轨迹”是无法修改特征的。这是因为，此时的轨迹8已经包含了两条不同的轨迹，而两条不同的轨迹无法同时修改特征。

合并轨迹后，仿真时一切如常。

1. 隐藏：隐藏当前选中的单条/多条轨迹。隐藏后，机器人加工管理面板中的轨迹会变成灰色，绘图区的轨迹会暂时隐藏不见。

1. 显示：重新显示已有隐藏的轨迹。

1. 删除：删除所选中的单条/多条轨迹。

1. 重命名：重新对轨迹进行命名。

1. 属性：

轨迹显示：选择是否显示轨迹点和轨迹线

轨迹属性：设置轨迹的关联坐标系和TCP点。

轨迹速度设置：设置轨迹的速度，关节速度，快速移动和加工速度，进退刀速度以及切入切出速度等。

轴配置：用于直接查看当前激活的轨迹或机器人的轴配置信息，此处轴配置只用于快速查看，不能直接修改当前轨迹或机器人的轴配置。

联动求解：根据需求设置联动求解的方式。

自定义参数：支持自行添加相关参数，需要添加好参数名称和参数值，点击“确定”。

1. 自定义菜单：

自行设置菜单功能栏

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image286.png)
图11.90：功能界面
##### 11.11.2轨迹点

轨迹点右键菜单中包含了轨迹点的诸多操作，包括轨迹点的复制、编辑、删除、仿真、定义变量、添加/删除仿真事件等。

1. 按轴移动轨迹点

功能位置：位于机器人加工管理面板上单条/多条轨迹的右键菜单内；调试面板上单个/多个轨迹点的右键菜单内。

注意：该功能只针对Move-Absj点。

功能介绍：按照选定轴的方向来平移指定的距离。

操作步骤：

1. 按轴复制轨迹点（单选/多选轨迹点）

位置：调试面板的轨迹点列表中任意轨迹点的右键菜单内；或机器人加工管理面板中轨迹点下MoveAbsj点的右键菜单内。

说明：此功能只适用于轨迹点指令为Move-AbsJoint的点。

这里的轴指的是机器人的轴。按轴复制轨迹点即旋转/平移运动机构的一个轴到目标位置，同时复制选中的轨迹点。平移轴按距离复制，旋转轴按照弧度复制，简化了轨迹设计。

示例：

以十轴机器人为例。

机器人在加工时需沿着红色箭头的方向滑行。图中已经生成了两个Move-Absj点。

图示：按轴复制轨迹点步骤

在机器人加工管理面板中选中两个Move-Absj点，右击，选择下拉菜单中的【按轴复制轨迹点（多选轨迹）】

图示：按轴复制轨迹点窗口

- 选择轴：复制轨迹时移动的轴(平移轴/旋转轴）；

- 差值：每份复制的轨迹点之间相隔的距离/相差的角度。如，旋转轴设置的差值为30，则复制点1与点2之间相差30°，点2与点3相差30°；

- 复制份数：复制所选轨迹点的份数。

- 点击【确认】后，十轴机器人复制的轨迹点如下图：

图示：十轴机器人复制轨迹点效果

1. 编辑点

位置：调试面板的轨迹点列表中任意轨迹点的右键菜单内。

说明：编辑点有两种不同操作，【绝对位置】和【相对位置】。

绝对位置：轨迹点在整个世界坐标系中的位置已经固定了，整个轨迹移动，该点不动。

相对位置：轨迹点的位置是相对于整条轨迹来说的，整个轨迹移动，该点随之移动。

需先对轨迹进行编辑后才能区分出绝对位置和相对位置，否则“编辑点（绝对位置）”和“编辑点（相对位置）”都会默认为相对位置的效果。

示例

以零件气缸上的两条轨迹为例。
#### 图示：气缸上两条轨迹

首先，让两条轨迹平移相同的距离后如图示：
#### 图示：轨迹平移

右击轨迹1上的点1，选择【编辑点（绝对位置）】，利用三维球将点1沿Z轴平移20mm.

右击轨迹2上的点1，选择【编辑点（相对位置）】，同样将点1沿Z轴平移20mm.
#### 图示：编辑轨迹点

接着，修改两条轨迹的平移特征：利用三维球将两条轨迹分别平移相同的距离。

可以看到，轨迹1上的点1同时平移，但轨迹2上的点1位置不变。
#### 图示：编辑轨迹点效果

1. 编辑多个点

位置：调试面板的轨迹点列表中任意轨迹点的右键菜单内。

说明：编辑多个点可同时编辑多个点的位置和姿态。接下来详细说明一下包含的各个功能点。

点击【编辑多个点】，弹出图示对话框。

图示：编辑多个点界面

- 输入受影响点数目：点击【输入】或按Enter键来确认点的数目。

- 向前：影响所选点的前几个点；向后，影响到所选点的后几个点；如果向前、向后同时勾选，则会影响到所选轨迹点的前、后点。

- 渐变：以被编辑的点为基准，被影响轨迹点的平移距离/旋转角度逐渐变小，减少值成   等差数列。

- 统一位姿：所有轨迹点的姿态与被编辑点的姿态相同(即X Y Z三个轴的方向平行）。

- 平移/旋转：受影响轨迹点与被编辑轨迹点平移相同的距离/旋转相同的角度。

- 曲线调整：通过调整模拟曲线形状来调节选中的轨迹点及其两侧指定个数点间的平滑过渡状态，从而实现对轨迹的多个点进行编辑的目的 。

示例

渐变，统一位姿，平移/旋转

点的编辑方式有四种：渐变,统一位姿，曲线调整和平移/旋转。

以气缸去毛刺为例，去毛刺时，打磨头的末端会沿着轨迹运动从而将毛刺去掉。

我们先来对比一下“渐变”、“统一位姿”和“平移/旋转”这三种方式。

在气缸上生成一条轨迹后，编辑多个轨迹点。被编辑的点均选择点7，被影响的点均设为向后的10个点，让点7的Z轴均旋转90度。

初始轨迹如下：
#### 图示：气缸初始轨迹

三种不同编辑方式：

| 编辑方式 | 图示 | 说明 |
| --- | --- | --- |
| 渐变 |  | 从点7到点17，旋转角度分别为90°， |
| 统一位姿 |  | 从点8到点17，点的X Y Z三个轴的方向与点7均平行。 |
| 平移/旋转 |  | 从点8到点17，所有点旋转的角度都与点7一样，均为90°。 |
#### * 三种方式在编辑时都利用三维球来实现。
#### 曲线调整
#### 以油盘涂胶为例来讲解曲线调整。

- 选中【曲线调整】后弹出图示的曲线调整界面。

不勾选向前向后，曲线的顶端点1即为所选点；

勾选向前，曲线上的点3即为所选点；

勾选向后，曲线上的点2即为所选点。

图示：“曲线调整”界面示意图

- 调控点：调整控制曲线形状的点。单击曲线，线上会出现三段平直线段，可利用线段两   端的调控点来拖动曲线改变其形状。拖动的原则是，蓝线全部位于界面的空白区（即机器人工作的最优区）。
#### 刻度：平移距离/旋转角度的比例。

图示：“曲线调整”界面示意图

- 调控点的增加和删除：右击曲线，通过指令可增加/删除调控点 。下图为增加了若干调控点的效果，提高了调整曲线的范围和灵活度。

图示：“曲线调整”界面示意图

- 曲线调整前需要做的两点工作为：

一，必须先用三维球将要调整的点，在要调整的方向上拖动一定的距离；

二，进入【编辑多个点】界面后，一定要向前或向后“影响的点数”。

- 曲线调整的两种常见场景

平移：这时曲线模拟的是轨迹点其两侧点组成的平滑过渡的形状；

图示：“曲线调整”之“平移”
#### 图中黑色箭头只在平移的时候出现，提示轨迹点平移的方向。。

旋转：这时曲线模拟的是所选轨迹点及两侧点各点的空间位姿。

图示：“曲线调整”之“旋转”

1. 删除点
#### 位置：调试面板的轨迹点列表中任意轨迹点的右键菜单内。

说明：删除点即删除选中的单个/多个点。

1. 删除此点前（后）所有点
#### 位置：位于调试面板的轨迹点列表中任意轨迹点的右键菜单内。
#### 说明：对轨迹点进行批量删除操作时，经常会删除某点前或某点后所有点。【删除此点前/后所有点】指令，批量删除点前和点后的所有点，减少了机器人加工管理面板树形图上的特征数量，简化删除操作，并能在机器人加工管理面板中修改删除特征。
#### 指令适用于轨迹点数量大于等于2时。

- 一旦使用这两个命令，会将该操作的特征节点悬挂显示在“机器人加工管理面板”的轨迹历史树下。后续支持选中它，右击，进而进行修改特征、删除特征、删除后续特征操作。

图示：编辑“删除多个点”操作

- 修改特征：再次批量删除剩余的轨迹点。

图示：编辑多个点-修改特征

- 删除特征：删除“删除多个点”的操作指令。

- 删除后续特征：删除本操作及其之后的所有操作。删除后，轨迹历史树下的相应特征被删除。

1. 设置为起始点
#### 位置：位于调试面板的轨迹点列表中任意轨迹点的右键菜单内。

说明：该指令是将当前选中的点设定为点1，即轨迹的起始点，用于修改机器人加工工件时的起始位置。

示例

以气缸去毛刺为例，轨迹初始状态如下：
#### 图示：气缸初始轨迹

将轨迹点11设置为起始点，效果如下，可以看到，原来的点11的序号已经变成1了。
#### 图示：“设置为起始点”效果

1. 统一位姿
#### 位置：位于调试面板的轨迹点列表中任意轨迹点的右键菜单内。
#### 说明：所有轨迹点的姿态与被编辑点的姿态相同，可以用来调整轴超限的点，优化轨迹姿态，减小了工具工作时扭动的幅度，尽量避免机器人和工具发生碰撞。

示例

以气缸去毛刺为例。

选中点1，右击，选择下拉菜单中的【统一位姿】后，在该点上弹出了三维球。
#### 图示：“统一位姿”示意图

用三维球对点的位姿进行微调。调整点1的时候，其他点的位姿也会随之而动，调整后如下：
#### 图示：“统一位姿”效果图

- 一般在平面上使用这个功能的情况比较多。如果在曲面上使用，其他轨迹点的姿态与所选择的轨迹点姿态一致，会导致加工方向（Z轴）不垂直于加工面。

1. 在此点前插入POS点
#### 位置：选中轨迹点后的右键菜单内。
#### 说明：在一条轨迹中插入POS点，便于在轴限位前使机器人重新调整姿态。
#### 在选中的轨迹点前插入一个POS点后，会在工具TCP位置插入一个点，取代该点序号，后面的序号依次后移。
#### 图示：插入POS点示意图
#### 插入POS点之后，机器人加工管理面板上添加特征“插入pos点：序号xx点”，可以对该特征进行修改。修改特征时，会在pos点位置弹出三维球，通过三维球调整pos点位置和姿态。
#### 图示：“插入POS点”特征修改

- 当点的指令为“Move-Circle”时，不能进行插入pos点操作。

1. 单机构运动到点和多机构运动到点
#### 位置：调试面板轨迹点列表中任意轨迹点的右键菜单内。
#### 说明：在多机器人环境下，选中某个机器人的某个轨迹点后，想查看机器人运动到该点时的轨迹求解状况，目前有两种办法：
#### 单机构运动到点：该轨迹点对应的机器人、机构单独运行到该点，其他机
#### 器人、机构静止不动。
#### 多机构运动到点：当该轨迹点对应的机器人、机构运行到该点的时间段内，
#### 场景中其余的所有机器人、机构会做同步运动。
#### 图示：“单机构/多机构运动到点”对比图
#### 备注：

- 图示列举了机器人A，分别通过两种方式运动到点B时的不同情形

- 特别指出：单机器人场景下，分别通过这两种方式运行到点，效果是一样的

1. 从此点开始仿真
#### 位置：调试面板轨迹点列表中任意轨迹点的右键菜单内。
#### 说明：对所选点及该点之后的所有轨迹点进行仿真。点击此指令后，即弹出仿真管理面板，形象逼真地模拟机器人的运动路径和状态。

1. 观察
#### 位置：调试面板轨迹点列表中任意轨迹点的右键菜单内。

说明：以所选点的Z轴为视线出发点，观察所选轨迹点周围的情况。
#### 图示：“观察”示意图

1. 定义偏移量变量
#### 位置：调试面板轨迹点列表中任意轨迹点的右键菜单内。
#### 说明：为轨迹点位置偏移设置变量。
#### 一般情况下，机器人所要加工的物料位置是固定的。但是有时候，比如砂轮上的物料，它们的摆放位置不固定，机器人需要调整运动路径来适应工件位置的变化，这时候就需要变量数值。
#### 选择【定义偏移量变量】后，输入实际情况中的变量值，机器人可根据数值灵活地随时调整姿态，以应对各种情况。
#### 图示：“定义偏移量变量”示意图
#### 偏移参考点：轨迹点偏移的距离和角度所参考的点。
#### dx、dy、dz变量：点平移的变量值；
#### ox 、oy 、oz变量：点旋转的变量值。
#### 不显示端口变量：是否在后置代码中显示端口变量。

1. 分割轨迹
#### 位置：调试面板轨迹点列表中任意轨迹点的右键菜单内。
#### 说明：根据需求将一条完整的轨迹分割成两段，分割处即为所选点，所选点将会归入到下一条轨迹中。分割完成后，“轨迹历史”下的所有轨迹特征都会合并为“基本生成方式生成轨迹”。

示例

以气缸去毛刺为例。

选择轨迹1（共有13个点）为所要分割的目标轨迹，在调试面板中选择轨迹1中的点6，右击选择【分割轨迹】

图示：“分割轨迹”示意图

可以看到，原来的轨迹1被分割成了两条轨迹，多了一条轨迹8。

图示：“分割轨迹”示意图

同时，轨迹1的点数变成了5，轨迹8则有8个点。

1. 添加仿真事件
#### 位置：调试面板轨迹点列表中任意轨迹点的右键菜单内。
#### 说明：添加仿真事件一般是对轨迹点添加新的指令，满足实际操作过程中的多种需求。
#### 可添加的事件包括：抓取事件、放开事件、停止事件、发送事件、等待事件、等候时间事件和自定义事件。
#### 等待时间事件是在被选中的轨迹点前输出。自定义事件由您来决定输出位置是点前还是点后。余下的事件都是在轨迹点后输出。

- 关联端口：端口即设备与外界通讯交流的出入口。仿真事件需要发出命令的设备给执行设备一个信号，信号接受需要一个端口，执行设备接受到信号后开始执行事件。

- 端口值：每个端口区别其他端口的特殊符号。

图示：“添加仿真事件”示意图

- 相同对象、相同模型，在不同轨迹中的关联端口是不同的；如果是两个不同的模型，它们的关联端口可以是相同的，端口值默认为1。

- 添加完的仿真事件会显示在机器人加工管理面板的工艺信息中，右键可对事件进行编辑和删除。

图示：仿真事件的编辑和删除

【抓取事件】

一个对象抓取另一个目标对象，抓取点的选定不固定不唯一。要在对话框中确定执行设备和关联设备。

【放开事件】

一个对象放开另一个目标对象，放开点的选定不固定不唯一，要确定好执行设备和关联设备。

【发送事件】与【等待事件】

发送与等待事件即两个物体通信，需要一个物体发送，另一个物体接受。

如A物体为发送方，B物体为接受方。当A的“发送事件”被触发时，B从A处接收到信号后立即运动，不再等待。

图示：发送事件示意图

在对话框中，名字是任意取的。发送时，类型选择为发送事件。当为接受物体时，类型一定要选择为等待事件。

示例

以机器人上下料为例，机器人抓取小滑块到目标位置后放开。

机器人在图示的位置放开小滑块后，小滑块应自动落下到工作台底部。此时，应在机器人放开轨迹的最后一个点上添加“发送事件”，在小滑块的驱动点上添加“等待事件“。机器人放开小滑块的瞬间，发送信号通知小滑块结束等待，滑落到工作台底部。

图示：机器人上下料场景图

先设置发送事件。选中机器人的最后一个放开点，右击，添加的仿真事件如下：

图示：“发送事件”示意图

填写好信息点击【确认】即可。

接下来设置等待事件。

选中小滑块的“驱动点1”后，右击选择【添加仿真事件】

图示：“等待事件”示意图

这里选择【等待事件】，在【等待的事】中选择“机器人-等待1”，这样发送和接收的事件就匹配上了。

【自定义事件】

根据需要自己输入内容（机器人可执行的语言），让机器人执行多种动作指令。添加的自定义事件可以在后置中生成代码，从而实现真机操作。

图示：“自定义事件”示意图

- 在添加自定义事件之前，需先在【工艺设置】中添加自定义事件模板。

图示：“工艺设置”位置

图示：“工艺设置”示意图

- 录入：将设置的模板名字和内容录入到右侧表格中。

- 删除行：删除表格中的一行模板。单击选中表格中的某一行，使其变为蓝色处于可操作状态后，可删除该行。

- 从文件读取：从格式为robdef的文件中读取自定义模板信息。

- 保存到文件：将当前自定义模板信息保存到格式为robdef的文件中，方便下一次读取使用。

在工艺设置中添加好自定义模板后，通过轨迹点右键菜单【添加仿真事件】，打开自定义事件界面，

从模板名字的下拉菜单中选择需要添加的自定义事件，则模板内容会自动加载显示。

图示：“自定义事件”示意图

- 输出位置：决定输出所添加的自定义事件的位置，包括点前输出和点后输出，即该事件是在所选轨迹点前被执行还是点后被执行。

【等候时间事件】让指定的对象在指定的点前停留指定的时间。

以机器人上下料为例，设置等候时间事件：

图示：小滑块场景图

小滑块需要等传送带滚动起来才能运动到传送带上，可以先让小滑块等待3秒钟。

选择【添加仿真事件】，弹出对话框。

名字填为“停留3秒”，执行设备选择“小滑块”，类型选择【等候时间事件】，时间设为3，点击【确认】即可。

图示：“等候时间事件”示意图

在驱动点3的工艺信息下面发现多了一个信息“停留3秒＿点1”

图示：“等候时间事件”特征图

继而仿真，会发现小滑块在驱动点3之前（等候时间是在选取的点前）停留了3秒才继续运动。

【停止事件】让目标对象在指定的点停止运动。

图示：“停止事件”示意图

1. 删除仿真事件
#### 位置：调试面板轨迹点列表中任意轨迹点的右键菜单内。

说明：删除在该轨迹点添加的仿真事件，在仿真通过方框勾选可选择删除哪个事件。
#### 图示：“删除仿真事件”示意图

1. 轨迹点属性
#### 位置：调试面板轨迹点列表中任意轨迹点的右键菜单内。

说明：轨迹点属性可以查看所选轨迹点的位置XYZ，和姿态Q1Q2Q3，清晰具体地了解到轨迹点的位姿。
#### 图示：“轨迹点属性”示意图

轨迹点是机器人运动路径的基本单元，若干个轨迹点组成了轨迹。

点击机器人加工管理面板中的单条轨迹后，该条轨迹的所有轨迹点都会显示在调试面板上。一般情况下，我们主要通过调试面板来编辑轨迹点。

本单元主要介绍了轨迹点的颜色含义、指令类型和一些基本操作，了解并掌握之后，有助于我们更好地规划机器人的运动路径。
### 工作单元

工作单元是包含机器人、工具、零件、状态机等设备的一个系统，既可以是完整的工作站，也可以是单独的某个模型。设置工作单元方便统一管理。

在机器人加工管理面板的结构树上，工作单元为独立的节点，所有新增的工作单元都会归入该节点下。右击某个单元，可对单元进行右键菜单中的几种操作。

示例：

选择某个机器人右键菜单中的【添加至工作单元】，弹出相应的对话框：

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image404.jpeg)
图11.91：“添加至工作单元”

点击【确定】后，面板结构树上，新创建的工作单元下会显示出所选对象。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image405.png)
图11.92：工作单元结构树

编辑工作单元：右击单个/多个工作单元，下拉菜单中列出了工作单元的可操作项目。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image406.jpeg)
图11.93：机器人单元

*添加到工作单元中的机器人依然保留其原本的特征。
## 调试面板

位置：位于软件界面右侧。

功能说明：调试面板与机器人姿态和轨迹点特征紧密联系，如图12.1所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image407.png)
图12.1：调试面板
### 机器人关节

该面板用于调试机器人的关节角，改变机器人的姿态，如图12.2所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image408.png)
图12.2：调试机器人关节角

J1 J2 J3 J4 J5 J6分别代表机器人的一轴、二轴、三轴、四轴、五轴和六轴。

其中，±170，±70，-65~70， ±150，±115，±300分别表示每个关节的旋转角度范围，通过小滑块左右移动，在这六个范围内改变六个轴的关节角度值。
### 轨迹点编辑

更改轨迹点的运动指令、速度和轨迹逼近值，并且显示出机器人在该轨迹点执行的事件，如图12.3所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image409.png)
图12.3：调试面板示意图

轨迹点的指令：包括Move-Line, Move-Joint，Move-AbsJoint和Move-Circle四种。

◎Move-Line：机器人以线性移动方式运动至目标点，当前点与目标点二点为一条直线，机器人运动状态可控，运动路径保持唯一。

◎Move-Joint：关节运动指令，表示的是机器人做关节运动，按照关节角度值来达到指定的点。机器人以最快捷的方式运动到目标点，机器人运动状态不完全可控，但运动路径保持唯一，常用于机器人在空间大范围移动。

◎MoveC：全称是Move-Circle，为圆弧运动指令，机器人通过中间点以圆弧移动方式运动目标点，当前点、中间点与目标点三点决定一段圆弧，机器人运动状态可控，运动路径保持唯一。

◎Move-AbsJoint：绝对运动指令，按照角度指令来移动。

轨迹点的速度：轨迹点（轨迹/机器人）在真机环境中的运动速度，单位为mm/s,可生成后置代码导入示教器中。

轨迹逼近：轨迹的平滑圆弧过渡。有时机器人运动到某个轨迹点时会暂停，即速度为0。该指令可以防止机器人在该点出现精确暂停，让其形成一个抛物线的轨迹，即实现圆弧过渡。

如图，机器人从P1运动到P2到P3，再到P4。
#### 图12.4：轨迹逼近

以上图为例，轨迹逼近值上限为p2p3距离的一半。

机器人运动到点2、点3时速度为0。 这时设定【轨迹逼近】的数值为8mm，那么机器人的运动路径为黑色曲线，绕过了P2 和P3。

*若要求机器人必须运动到点2或者点3，就不能用该指令。

另外，若原轨迹是从点1到点2，两点之间有障碍物，可以插入一个点3，然后使用轨迹逼近，可使机器人连续运动，如下图：

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image411.png)
图12.5：轨迹逼近应用场景

◎对当前选中的轨迹直接仿真。

点击出现仿真管理面板，执行仿真操作。同时面板上还显示出了该条轨迹的名称。

◎使机器人运动到某个点。

勾选面板中的“机器人运动到点”后，只需单击目标点即可让机器人运动到该点。

◎查看五种不同轨迹点颜色的含义。

绿色：表示该轨迹点是完全正常的；

黄色：表示轴超限，机器人的运动超过了某个关节的运动范围；

红色：表示不可达点，机器人距离目标太远，此时需要调整机器人与工件或外部工具的距离；

灰色：表示不知道该轨迹点的当前状态；

紫色：表示奇异点。

什么是奇异状态和奇异点？

奇异状态：一般指工业机器人机器手臂出现的运动故障，指的是在该状态下失去了一些运动自由。就像人的手一样，如果手臂完全伸直就不能让手再伸向手臂所指的方向。而没有伸直时，手是可以往各个方向运动的，这就是一种奇异状态。而奇异点就是造成机器人出现奇异状态的点。

如下图，机器人的2轴和3轴产生了奇异点：

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image416.png)
图12.6：机器人奇异状态
## 机器人控制
### 控制面板

此面板控制机器人的关节运动，调整其姿态，读取机器人的关节值，以及使机器人回到机械零点。

位置：位于软件界面右侧

功能说明：机器人控制面板分为机器人空间和关节空间两个部分。机械零点：机器人出厂时的初始姿态，如图13.1所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image417.png)
图13.1：控制面板界面
### 坐标系

通过此功能查看当前所选机器人的机器人末端法兰或机器人当前TCP相对于世界坐标系或用户坐标系或机器人基座标系的空间位姿。也可通过在输入框中修改坐标系的值后点击“到点”功能，控制机器人末端法兰或当前TCP的坐标系调整到对应的位姿，如图13.2所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image419.png)
图13.2：坐标系

工具坐标系：以工具坐标系的原点来确定机器人的位置。

调整步长：这里步长指的是机器人平移/旋转运动幅度的大小，从0.01到10幅度依次加大。
### 机器人空间

机器人空间：模拟示教器控制机器人，如图13.3所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image420.png)
图13.3：机器人空间

平移：利用 和控制机器人向X（前后）Y（左右）Z（上下）等方向平移；

旋转：利用 和控制机器人以 XYZ三个方向为中心旋转；

坐标表示：根据机器人品牌来确定坐标用四元数还是欧拉角来表示。

*坐标用四元数来表示的机器人有：ABB。其他品牌机器人一般用欧拉角来表示。

相对坐标系：方便的查看机器人末端FL、工具TCP ，相对不同的参考坐标系，实时显示出相对位置数值，以便作为参考依据。
### Home点

功能说明：此功能用来显示已保存的HOME点，还可以删除HOME点，如图13.4所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image423.png)
图13.4：home点界面
### 关节空间

功能说明：左右移动调整机器人的关节角度值，具体数值显示在中。

其中，±170等为六个轴的活动范围。减小或增大某个轴的关节角，数值改变间隔即为步长。如设定步长为5.00，J1的关节角度初始值为90。 点击增加关节角，则数值会变为95。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image428.png)
图13.5：机器人关节空间
### 轴配置

功能说明：用于直接查看当前激活的轨迹或机器人的轴配置信息，此处轴配置只用于快速查看，不能直接修改当前轨迹或机器人的轴配置。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image429.png)
图13.6：轴配置
## 输出

功能说明：输出面板位于软件界面右侧，在时序仿真时通过输出面板可以对仿真过程中设备执行的事件信息，并会输出异常轨迹点信息。仿真功能模拟的是机器人在实际环境中的运动路径和状态。仿真时，输出面板会显示出机器人执行的事件和命令，以及有问题的轨迹点。双击输出面板中的提示事件，机器人姿态会更改到事件被执行时的状态，如图14.1所示。

![配图](https://cdn.jsdelivr.net/gh/qsgy/pqart-kb-images@master/manual/manual-image430.png)
图14.1 输出面板示意图

同时，面板会输出有问题的轨迹点，如上图所示轴超限的轨迹点。出现这种情况后，需要对轨迹点的姿态进行调整，详细的调整方式详见轨迹编辑。
## 快捷键菜单
### 15.1视向快捷键

| 功能 | 快捷键 |
| --- | --- |
| 前视 | （1） |
| 俯视 | （2） |
| 右视 | （3） |
| 后视 | （4） |
| 底视 | （5） |
| 左视 | （6） |
| 轴测 | （0） |
| 显示全图 | （F8） |
| 局部放大 | （按住Ctrl+B，鼠标左键选中区域） |
| 显示居中 | （V+S） |
| 透视开 | （V+P） |
| 透视关 | （V+O） |
### 15.2绘制样式快捷键

| 功能 | 快捷键 |
| --- | --- |
| 新建 | （Ctrl+N） |
| 保存 | （Ctrl+S） |
| 撤销 | （Ctrl+Z） |
| 复制 | （Ctrl+C） |
| 粘贴 | （Ctrl+V） |
| 剪切 | （Ctrl+X） |
### 15.3功能快捷键

| 功能 | 快捷键 |
| --- | --- |
| 世界坐标系显示/隐藏 | （A） |
| 导入工程文件 | （Ctrl+I） |
| 激活工具三维球状态下添加MoveAbsj | （Ctrl+K） |
| 激活工具三维球状态下添加MoveJ | （Ctrl+J） |
| 激活工具三维球状态下添加MoveL | （Ctrl+L） |
