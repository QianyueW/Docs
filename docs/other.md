# 待整理信息

## Git常用命令
Git log --reverse --oneline
Git log --graph --oneline
Git checkout <commitid>
Git checkout master

# ADB工具
adb shell dumpsys meminfo + 你的demo进程的包名

# Digital Content Creation Tools & TA related
https://renderguide.com/daz3d-filament-tutorial/ TA快乐老家可用来学Blender
https://www.khronos.org/api/index_2017/ktx
https://registry.khronos.org/KTX/specs/2.0/ktxspec.v2.html

# profling tools性能调试工具：
• Intel's VTune,
• IBM's Quantify and Purify (part of the PurifyPlus tool suite),
• Insure++ by Parasoft, and
• Valgrind by Julian Seward and the Valgrind development team.

# 相关好文
https://www.cnblogs.com/dins/p/tu-pian-de-jie-ya-suo-xuan-ran.html
https://zhuanlan.zhihu.com/p/357265599

# 工作小札

- 虹彩特性合入当前的引擎框架

- 运动模糊后处理特性的开发

- 其他-OIT透明渐变方案，灯光排除功能实现，动画系统问题定位。。
  
### 如何优化内存使用情况
一、从模型资源入手
1. 降低模型面数
2. 实例化
> 用renderdocs来检查gltf中是否存在重复的几何数据，如有可以使用实例化的技术来降低内存的使用。实例化是一种技术，在场景中渲染同一对象（网格）的多个副本，但它们不是将每个副本存储为单独的对象，而是将它们都存储为单个实例。
3. 贴图转ktx2
4. 降低贴图分辨率，尽可能选择小的贴图
5. 拆分复杂贴图，复杂的贴图要拆分来评估其大小
6. 减少不必要的贴图使用，纯色的话就没有必要使用贴图
二、从引擎内存管理系统入手：？？？

### 如何优化CPU的占用情况：
1. 

### 如何优化锯齿的问题：
1. 