## 基础

#### 路径

软件本体、版本：C:\Program Files\Blender Foundation\Blender 4.4\

项目：D:\Blender_study\Blender_Projects

#### 快捷键与工具、修改器

Shift + 中键                平面移动

Shift + A                     菜单

G（ + X /Y /Z )              移动物体

S（ + X /Y /Z )               缩放

R（ + X /Y /Z )               旋转

ps物体模式下变换记得应用Ctrl + A

Alt（ + G /S /R )            撤销 移动/缩放/旋转

Alt + 双击                       编辑模式下可以全选纵/横向的点（注意在线模式下，+Shift才可选竖线横排的线）

Alt + Z                            切换透视模式

H（ + Alt /Shift )           隐藏 显示全部/隐藏未选中的物体

Shift + D                        复制并移动

137 9  5  0  .   ~             xyz 取反 正交切换 摄像头 快捷放大 快捷目录

Ctrl + 空格                     最大化当前功能面板

Shift + 右键                    移动游标

Shift + 左键                    最后选中的物体（多选时）

Shift + C                         游标回归原点

Shift + N                        调换正反面

Ctrl                                 吸附网格（编辑模式框选时连接选中的点； 标注模式下+左键为擦除； 测量模式为吸附）

Ctrl + L                           关联

Ctrl + I                            反选

Ctrl + +（数字键盘+）  扩大选区

Ctrl + 右键                      连续挤出

L                                      编辑模式下会选中与之相连的所有点（需要鼠标悬浮在物体上，三角面需要点两次）

X                                      编辑模式下控制点线面的删除融并

![0f3fb334-4d83-4516-bc9d-587cfe8a253d](file:///C:/Users/yeyuh/Pictures/Typedown/0f3fb334-4d83-4516-bc9d-587cfe8a253d.png)

![3419ccff-a9dc-49cc-a2ca-902ae49978c6](file:///C:/Users/yeyuh/Pictures/Typedown/3419ccff-a9dc-49cc-a2ca-902ae49978c6.png)



#### 流程

建模

布光

材质

渲染



#### 面板

选择：随机选择

透视模式：四个球左边

显示面朝向：透视模式左边。蓝正红反

显示点法线/拆分法线/法线：透视模式左边。法向模块

鼠标移至四角拖动可分裂或合并功能模块（右键）

选项 变换 仅影响物体锚点或其他



![007f0d27-aa81-4bc3-8d88-001a3801a3cf](file:///C:/Users/yeyuh/Pictures/Typedown/007f0d27-aa81-4bc3-8d88-001a3801a3cf.png)



#### 建模基础

###### 点线面选择与控制

![e71d97f5-eb37-4872-badb-924b86d4505b](file:///C:/Users/yeyuh/Pictures/Typedown/e71d97f5-eb37-4872-badb-924b86d4505b.png)



###### 十大建模技巧

E挤出：按右键取消仍会保留挤出的点线面，完全撤销按Ctrl + Z；多个面默认按平均法向挤出

I向内挤出：右键取消 不会 会保留挤出的点线面

Ctrl + B倒角：滚轮改变面数

Ctrl + R环切：滚轮改变环切数量，右键取消自由切割，默认平均切割

M合并：

V断开：

右键：细分

F填充：点击上面的点线面按钮可以栅格填充

K切刀：右键退出

Ctrl + J：合并选中物体

Ctrl + E：桥接

P分离：

![fd6f38cc-8b77-4c2c-8b09-06c7eb0e8df3](file:///C:/Users/yeyuh/Pictures/Typedown/fd6f38cc-8b77-4c2c-8b09-06c7eb0e8df3.png)



## MMD

#### 流程

插件：mmd tool

修改输出帧率

导入pmx 3D模型

<img title="" src="file:///C:/Users/yeyuh/Pictures/Typedown/f4057433-4923-4ebf-98c0-a6a7bd588ed9.png" alt="f4057433-4923-4ebf-98c0-a6a7bd588ed9" style="zoom:50%;">

以下流程解决动作无表情：

        选择骨骼

        MMD插件点"变形工具"  "顶点"

        点“ v ”

        选择绑定变形

        在之后绑定运动后，同时也要为“.placeholder”导入运动

选择骨骼

然后导入运动

“渲染动画”后可以导出



#### ps

1.模型发紫可能为贴图丢失，可在MMD插件模型调试中点击检测贴图来检测缺失部位，然后在mesh的材质模块 表(曲)面  Toon Tex中手动修改贴图



## 原神模型导入

#### 流程

使用cat插件

N键打开侧栏

导入模型，点击骨骼进入编辑模式修改脚部骨骼防止脚部穿模

点击MMD模块 点击“翻译”并覆盖所有（似乎问题不大）

！！~~连接网格~~——合并——按材质分开——++合并——转换给Blender（独立化可以看到脸红？）

~~Combine Material~~（优化材质数量，别点）（Join all mesh是否需要？）

导入后在rig中创建Unity通用骨骼，如要物理模拟，请在这个操作之前完成



#### unity的插件

不过blender 直接导入unity的插件

http://link.zhihu.com/?target=https%3A//stereoarts.jp/MMD4Mecanim_Beta_20200105.zip)
