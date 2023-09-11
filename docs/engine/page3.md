## 渲染 Rendering

## 动画系统
## 物理系统
## 音效
## GamePlay
## 工具链
## 网络
## 面对数据编程与任务系统

<figure markdown>
  ![Image title](https://dummyimage.com/600x400/){ width="300" }
  <figcaption>Image caption</figcaption>
</figure>

---
引擎结构：

游戏 地图 APP

API层：java API，c++ API

平台无关层：3D文件加载和解析，场景管理，动画管理，渲染管理(渲染管理的设计目标：

1、屏蔽平台相关的图形API差异

2、内置常用的渲染管线：Forward，Deferred， Cluster Forward

3、灵活可选项：是否增加阴影Pass，是否增加反射Pass，是否需要后处理Pass；是否增加UI Pass

4、支持用户可配置管线，可定义规格（例如Unity最新版本可根据脚本来配置想要的渲染管线）

Render Graph的3个阶段：

1、setup阶段【将整个渲染流程拆分成pass；分为Compute Pass 和 Render Pass；约定Render Pass的执行顺序。声明输入输出的资源。延迟创建相关资源】

2、compile阶段【1、裁剪不需要的pass；2、计算resource的生命周期：资源的引用计数，异步计算的同步时间点；3、按需创建使用的内存】

3、excute阶段【1、调用真正的图形API: eg. OpenGL ES API；2、获取GPU需要的格式存放的数据，传递给GPU】

)，

loop管理（设计目标：把所有模块都串起来，ECS update更新所有系统，render frame绘制指令生成），拓展插件，脚本系统

平台相关层：图形设备管理，OpenGL后端，Vulkan后端，metal后端

android ios playstation windows web

引擎效率优化：

单一线程 -> 线程池：App 主线程， 引擎线程，ECS线程，IO线程

局部刷新

视锥剔除

如何实现视锥剔除：

1、确定视锥范围：近平面远平面

2、确定物体的包围盒

3、利用SSE指令加速计算物体包围盒跟视锥的交集


