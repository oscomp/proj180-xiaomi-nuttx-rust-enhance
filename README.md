# proj180-xiaomi-nuttx-rust-enhance
基于小米Vela平台的NuttX RTOS Rust增强
## 基于Vela平台的NuttX RTOS Rust增强

### 赛题要点/解析

#### 项目介绍

##### 平台介绍

**关于Vela**：[Vela](https://iot.mi.com/vela)是小米公司基于开源实时操作系统NuttX打造的物联网嵌入式软件平台，Vela在各种物联网硬件平台上提供统一的软件服务，支持丰富的组件和易用的框架，用于打通碎片化的物联网应用场景。

**关于NuttX**：[NuttX](https://nuttx.apache.org/docs/latest/)是一个在IoT、分布式嵌入式系统、无人机系统中广泛使用的RTOS，第一个版本由 Gregory Nutt 于 2007 年发布。NuttX 可以支持 8 位到64位的处理器，支持risc-v，arm，mips，x86等主流芯片平台，按照POSIX和 ANSI 标准进行设计，支持MMU和MPU，支持多线程和进程。2019年NuttX在小米的推动下正式进入Apache基金会，小米多位资深工程师参与了NuttX社区（https://github.com/apache/incubator-nuttx）的开发和架构设计。经过多年的不懈努力，NuttX功能丰富，性能稳定，商业化成熟度高，在各种物联网产品上得到了广泛的应用。

##### 项目意义

Rust是一门系统编程语言 ，专注于安全 ，尤其是并发安全，支持函数式和命令式以及泛型等编程范式的多范式语言。 Rust在语法上和C++类似 ，但是在保证性能的同时会提供更好的内存安全机制。当前，Rust语言已经逐步成为Linux内核的基础开发语言之一，后续将在Linux内核的开发中发挥重要作用，并会在后续的系统软件的开发中起到重要作用。

以Vela平台和NuttX实时操作系统为软件平台基础，结合大赛所提供的K210硬件平台（NuttX RTOS已经完整支持K210板卡，仿照Linux内核的实现方式，对NuttX操作系统进行增强，扩展各种Rust支持。

 

#### 功能点

注：所有功能点应能在K210板卡上运行并演示

##### 功能点要求

• 仿照Linux内核的实现，完成NuttX整体Rust支持框架包括编译框架

• 编写示例的Rust应用程序，可以在NuttX中进行加载和执行

• 编写示例驱动，可以采用模块方式加载内核驱动到NuttX内核并运行

##### 扩展功能

• 扩展Rust的支持，给出参考实现框架

• 利用Rust重写NuttX中的某个子系统框架

### 项目导师

• 接口人：秦蔚，qinwei1@xiaomi.com

• 小米公司Vela研发团队（含NuttX社区主要代码提交人）

#### 难度

中等~高

#### 文档

• [https://nuttx.apache.org/docs/latest/](https://github.com/acoinfo/sylixos_oscomp_2021/tree/master/Dual-OS-OpenAMP) ：NuttX的最新文档，可以直接下载并按照要求配置和使用K210板卡

• https://github.com/apache/incubator-nuttx/tree/master/boards/risc-v/k210/maix-bit ：NuttX文档中对K210板卡的配置和使用说明

• https://security.googleblog.com/2021/04/rust-in-linux-kernel.html

#### 参考代码

• https://github.com/apache/incubator-nuttx/ ：目前NuttX针对K210板卡具备完整支持，参赛者可在此基础上进行后续开发

• https://github.com/Rust-for-Linux/linux ：Linux内核的Rust支持

#### 预期目标

注意：下面的内容是建议内容，不要求必须全部完成。选择本项目的同学也可与导师联系，提出自己的新想法，如导师认可，可加入预期目标

##### 第一题

NuttX整体rust支持框架包括编译框架，可以加载和执行模块和应用;

##### 第二题

利用Rust重写NuttX中的某个子系统框架，并能正常使用和运行

##### 第三题

相关工作成果可以提交到Rust或NuttX开源社区并通过评审

### 对选择该赛题的支持

• 针对NuttX实时操作系统和Vela平台业界最专业权威的技术支持和指导

• 我们希望参赛团队根据自己的理解和思路，完成相关的代码架构设计，我们可以进行代码架构的评估和建议和以及针对NuttX修改思路上的指导
