## 基础架构 5 + 1：越低层的能力越稳定很少改动，越上层的能力越多变
#### 工具层 Tool Layer
1． Level editor 引擎自有IDE
Ø Logic editor
Ø Shader editor
Ø UI editor
Ø Animation editor
2． 用于处理Digital content creation的Asset conditioning pipeline（实际上就是各种导入导出器，让我们的引擎可以使用各种工具生产的3D资源）
#### 功能层 Function Layer：
1. Dive into Ticks: tickLogic + tickRender
2. Multi-threading: fixed thread à thread fork à Job system 如何组织任务线程，最大程度利用多核CPU的资源
资源层 Resource Layer: 实时的资产管理器Runtime Assets Manager
1. 处理resource à assets的转化，实际上就把所有的资源数据转化为引擎可以直接识别的和使用的格式。例如有些以DirectX作为渲染后端的引擎就需要使用DirectXTex texture processing library把jpg等图片转换成引擎可以识别的dds纹理格式，在Lume中我们是把所有的图像资源转化为KTX (Khronos Texture)的格式，从而可以被OpenGL和Vulkan渲染后端所识别并使用；同时，记录数据之间的关联的文件如xml等也是资源的一部分（包含GUID，全局唯一编号），在Lume引擎中我们是直接使用了glTF的文件格式来记录资源之间的联系，像是某一个部分贴什么贴图。
2. 管理资产的引用by handle system（句柄系统）
3. 管理资源的生命周期
#### 核心层 Core Layer：代码安全性和效率性要求很高，一般很少改动
1. Math Library 高效很重要
2. Data structure and containers
3. Memory Management
#### 平台层 Platform Layer：保证在各种不同的平台上该系统仍能兼容运行
不同的操作系统（Android，Mac，iOS，Windows）
不同的图形API接口（OpenGL，Vulkan，DirectX11\12, Metal）
甚至是不同的CPU架构。。
#### Middleware and 3rd party libraries

Trick is tick!s