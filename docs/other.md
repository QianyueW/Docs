# 待整理信息

## Git常用命令
Git log --reverse --oneline
Git log --graph --oneline
Git checkout <commitid>
Git checkout master

## ADB工具
adb shell dumpsys meminfo + 你的demo进程的包名

## Digital Content Creation Tools & TA related
https://renderguide.com/daz3d-filament-tutorial/ TA快乐老家可用来学Blender
https://www.khronos.org/api/index_2017/ktx
https://registry.khronos.org/KTX/specs/2.0/ktxspec.v2.html

## profling tools性能调试工具：
• Intel's VTune,
• IBM's Quantify and Purify (part of the PurifyPlus tool suite),
• Insure++ by Parasoft, and
• Valgrind by Julian Seward and the Valgrind development team.

## 相关好文
https://www.cnblogs.com/dins/p/tu-pian-de-jie-ya-suo-xuan-ran.html
https://zhuanlan.zhihu.com/p/357265599

## 工作小札

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



### Other
 - https://www.cnblogs.com/skiwnchiwns/p/10121763.html
 - https://mengzephyr.com/
 - http://geometry.cs.ucl.ac.uk/index.php
 - https://enigma-li.github.io/
 - https://www.youtube.com/@cggcseminar6533
 - http://kunzhou.net/
 - https://zhuanlan.zhihu.com/p/435927070
 - https://leetcode.cn/circle/article/mggm6Q/
 - https://en.cppreference.com/w/
 - https://github.com/FlaxEngine/FlaxEngine

https://doc.magnum.graphics/magnum/examples-motionblur.html

【碎片信息】

webGPU：https://www.youtube.com/watch?v=oWwtCDv3Pgg

Unity 2023: https://www.youtube.com/watch?v=kUDUM3BtXtU

Intel: https://www.intel.com/content/www/us/en/developer/topic-technology/gamedev/overview.html

https://game.intel.com/story/intel-arc-graphics-game-dev-all-access-2023-ray-tracing/

《3D数学基础：图形和游戏开发》—— 图形学相关的数学内容，可以用来打底子或是复习

《Fundamentals of Computer Graphics》, Forth Edition —— 虎书，图形学入门经典材料

《计算机图形学（第四版）》

《introduction to 3D Game Programming with DiecrtX 12》—— 某乎安利，用于学习常用的图形架构

《Real-Time-Rendering》, Forth Edition —— 实时渲染领域的圣经，可以搭配Games202和毛星云大佬提炼的该书籍的学习笔记一起食用

《Practical Rendering & Computation with Direct3D 11》—— 实时渲染实战

《Physically Based Rendering》, Third Edition —— 离线渲染领域的圣经，可以搭配Games201一起食用

《COMPUTER GRAPHICS: PRINCIPLES AND PRACTICE》, 3RD EDITION —— 课外读物

《WebGL编程指南》—— 通俗易懂搞懂图形渲染管线

《C++ Primer》—— C++从入门到入土

opengl红宝石书，可以搭配配套示例代码食用 GitHub - openglredbook/examples: Examples for the OpenGL Red Book

《OpenGL学习指南》第9版

《OpenGL programming guide》

《OpenGL编程权威指南》

《Vulkan学习指南》《Vulkan应用开发指南》

The Book of Shaders —— 着色器编程指南

《游戏引擎架构》——叶劲峰译

《GPU Gems 1-3》

《GPU Pro 1-7》

《GPU Zen》

实时渲染高级特性开发：https://zhuanlan.zhihu.com/p/151301323

渲染顺序：https://sunra.top/2022/07/24/unity-render-pipeline-12/

￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥

相关从业人员：【除了可以学习他们的CG知识分享，还可以思考他们增加互联网影响力的方式】

￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥￥

https://www.zhihu.com/people/tc130-52/following/columns

https://sunra.top/2022/07/24/unity-render-pipeline-12/

https://lijiankuan.github.io/

https://www.zhihu.com/people/pastel_de_nata

https://gwb.tencent.com/community/user/1037694

http://www.ownself.org/blog/more

http://www.ownself.org/blog/archives

https://holko.pl/about/

https://www.lfzxb.top/link/

https://www.cnblogs.com/cheermyang/p/6383266.html

https://github.com/keijiro

https://radiumsoftware.tumblr.com/archive

https://amplify.pt/

http://nothkedev.blogspot.com/2018/10/correct-motion-blur-for-fast-rotating.html

【学界论文】

https://onlinelibrary.wiley.com/doi/10.1111/j.1467-8659.2010.01840.x【】

UE

GTA游戏展示：https://www.rockstargames.com/zh/gta-v?info=trailer

UE光照技术：https://www.lunas.pro/news/lumen-ray-tracing.html

【Lumen自动全局光照和反射系统】Lumen is a fully dynamic global illumination and reflections system designed for next generation consoles that operates by default in Unreal Engine 5.

【RayTracing光线追踪】

unity后处理效果：

【如何检索一个后处理效果的实现方式？？Google (XXX图片检索 + XXXunity和UE code/源码 + XXX相关论文)】

【B/Y 检索unity和UE提供怎么样的XXX，以及是否有其他实现的教程】

【GitHub检索相关代码】

Unity Learn教程Introduction to Post Processing Stack中文讲解

课程资源链接：https://pan.baidu.com/s/1QOs8zWIRiGbd5w5t4UVM9Q 提取码:603i

讲师：BeaverJoe

https://www.bilibili.com/video/BV1SK4y187jj/?t=0h35m35s&vd_source=4e9b1èc157aec6187è1b36ā4310ed

https://www.bilibili.com/video/BV1B3411E7Gu/?spm_id_from=333.788&vd_source=4e9b1èc157aec6187è1b36ā4310ed

https://www.bilibili.com/video/BV1964y197t8/?spm_id_from=333.788.recommend_more_video.2&vd_source=4e9b1èc157aec6187è1b36ā4310ed

https://www.bilibili.com/video/BV1Gs4y1j7Yf/?spm_id_from=333.788.recommend_more_video.6&vd_source=4e9b1èc157aec6187è1b36ā4310ed

https://vga.zol.com.cn/228/2281769.html

https://www.lfzxb.top/unity-shader-post-processing/#%E8%BF%90%E%8A%A8%E6%A8%Ā%E7%B3%8A

https://www.irimsky.top/archives/301/https://www.blurredcode.com/2022/05/9f1444db/#%e7%94%bb%e9%9d%á%e%8f%98%e6%a8%ā%e7%b3%8a

https://ubm-twvideo01.s3.amazonaws.com/ō/vault/gdc2016/Presentations/Pedersen_LasseJonFuglsang_TemporalReprojectionAntiAliasing.pdf

静态模糊算法合集：https://zhuanlan.zhihu.com/p/125744132

https://github.com/QianMo/X-PostProcessing-Library

https://www.intel.com/content/www/us/en/developer/articles/technical/an-investigation-of-fast-real-time-gpu-based-image-blur-algorithms.html

https://developer.nvidia.com/gpugems/gpugems3/part-iv-image-effects/chapter-27-motion-blur-post-processing-effect

https://learnopengl.com/Advanced-Lighting/Bloom

https://portal.productboard.com/unity/1-unity-platform-rendering-visual-effects/tabs/3-universal-pipeline

https://docs.unity3d.com/Manual/PostProcessingOverview.html

https://github.com/Unity-Technologies/PostProcessing/blob/v2/Documentation~/Motion-Blur.md

https://www.youtube.com/watch?v=RlvvmiGtPQE

PS 后处理效果实现:

https://www.cnblogs.com/mtcnn/p/9412094.html

https://blog.csdn.net/kezunhai/category_2747081.html

写shader的骚操作：

https://www.bilibili.com/video/BV16à11e7Ly/?spm_id_from=333.788.recommend_more_video.-1&vd_source=4e9b1èc157aec6187è1b36ā4310ed

https://juejin.cn/user/1292681404482840/posts

https://github.com/WYM/cocos-creator-shaders

https://www.codinblack.com/blur-shader-using-shader-graph-in-unity3d/

[Universal Scene Description] https://www.bing.com/search?q=usd+format+3d&qs=UT&pq=usd+forma&sk=CT1&sc=10-9&cvid=Ǎ54F1C3ED34429B9445C4C1DAEFB116&FORM=QBRE&sp=2&lq=0

https://github.com/ocornut/imgui

https://github.com/miloyip/game-programmer

https://www.cnblogs.com/miloyip/

https://zhuanlan.zhihu.com/p/449623131

--------------------------------------------------------------------------------------------------------------------------------

【刷题题单】

力扣全tag

https://github.com/SharingSource/LogicStack-LeetCode/wiki/%E%9B%BE%E8%AE%BA-DFS

https://www.programmercarl.com/%È%BA%8C%E%8F%89%E6%A0%91%E6%80%BB%E7%BB%93%E7%AF%87.html

https://www.desgard.com/algo/docs/part3/ch02/1-segment-tree-rmq/

【学习视频】

c++ chreno 教程

c++ codecamp 教程

B站黑马程序员教程

ilearning课程1,2,3

【学习资料】

《C++软件工程能力》《C++ Primer》

---------------------------------------------------------------------------------------------------------------------------------

待学习清单：

 图形学及渲染理论基础：GAMES101, GAMES其他学习资料；OpenGL等图形API的学习及glTF格式理解；可以开发各种shader in GLSL/CG...

 软件开发基础：C++编程能力和工程能力；Java编程能力和安卓开发能力；git等常用工具的使用

 ---
- https://blog.selfshadow.com/publications/s2012-shading-course/
- https://media.disneyanimation.com/uploads/production/publication_asset/48/asset/s2012_pbs_disney_brdf_notes_v3.pdf
- https://www.zhihu.com/column/c_1419375161635819520
- https://renderguide.com/daz3d-filament-tutorial/ TA快乐老家可用来学Blender
- https://www.khronos.org/api/index_2017/ktx
- https://registry.khronos.org/KTX/specs/2.0/ktxspec.v2.html


c++推荐书籍：

[36] Scott Meyers. Effective C++: 55 Specific Ways to Improve Your Programs and Designs,

Third Edition. Reading, MA: Addison-Wesley, 2005.

[37] Scott Meyers. More Effective C++: 35 New Ways to Improve Your Programs and Designs.

Reading, MA: Addison-Wesley, 1996.

[38]Bjarne Stroustrup. The C++ Programming Language, Special Edition (Third Edition).

Reading, MA: Addison-Wesley, 2000.


📚 RT RESOURCES (in order of complexity)

 Ray Tracing in One Weekend series ► https://raytracing.github.io

 Scratch a Pixel ► https://scratchapixel.com

🔴 Physically Based Rendering: From Theory to Implementation ► https://amzn.to/3y2bGK7

https://github.com/facebook/igl

**rust编程语言**

Omniverse Runs on RTX

webGPU+RT: https://zhuanlan.zhihu.com/p/151023667

https://www.stubbornhuang.com/1256/

renderdoc可以查看gltf是否有重复实例化的信息，比如汽车轮毂

其他推荐工具：https://developer.nvidia.com/nvidia-perfkit User Guide

AI MIDDLEWARE SDK: Kynapse, Gameware Navigation



https://www.youtube.com/watch?v=GK7ntA7ávk&list=PLGvfHSgImk4ae9O7hLks6AJQTnQ3IIpDi

https://www.youtube.com/watch?v=mUeNqLcx4eI

https://www.youtube.com/watch?v=teg23SJlyl8

https://www.youtube.com/watch?v=HtH1GMnZpgo&list=PLAOytOz0HZbLaWhVrGEge_6dNCAzGFYH

https://www.youtube.com/watch?v=70q9jtjWP4o

https://www.youtube.com/watch?v=hRL56gXqj-4&list=PLÚnPsAdxKWQYxkmQ3TdbLsyc1l2j25XM

https://www.youtube.com/watch?v=DKrdLKetBZE

https://www.youtube.com/watch?v=Gf5mMWHWNYc

