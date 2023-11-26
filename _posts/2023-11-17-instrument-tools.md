---
title: "插桩工具整理"
excerpt: "插桩工具整理"
author: dsj
---

## Gcov

GNU工具链的一部分，用于代码覆盖率分析。它能够生成关于每个源代码行执行次数的统计信息

**插装技术类型**: 静态源代码

**下载地址**: 安装GCC即可

**适用平台**: Windows, Linux, macOS, and Unix等

## Syzygy

Syzygy 项目由一套工具组成，用于检测COFF对象文件和 PE二进制文件的工具套件。各种检测模式可用于计算代码覆盖率结果、分析源代码、应用配置文件指导的基本块优化、块（函数）级配置文件引导的重新排序，以及查找内存错误。

**插装技术类型**: 静态源代码

**下载地址**: 安装GCC即可

**适用平台**: Windows, Linux, macOS, and Unix等

## AddressSanitizer (ASAN)

AddressSanitizer（又名 ASan）是一款用于 C/C++ 的内存错误检测器。它能发现释放后使用（悬空指针取消引用）、堆缓冲区溢出、堆缓冲区溢出、全局缓冲区溢出、在返回后使用、在作用域后使用、初始化顺序错误、内存泄漏。

**插装技术类型**: 动态二进制

**下载地址**: 安装GCC或Clang

**适用平台**:  Linux, Darwin (OS X 和 iOS 模拟器), FreeBSD和Android

## Valgrind

Valgrind 是一个用于构建动态分析工具的插桩框架。Valgrind 工具可以自动检测许多内存管理和线程错误，并对程序进行详细剖析。

**插装技术类型**: 动态二进制

**下载地址**: [https://valgrind.org/downloads/current.html](https://valgrind.org/downloads/current.html)

**适用平台**: Linux、Android等

## DyanamoRIO

Syzygy 项目由一套工具组成，用于检测COFF对象文件和 PE二进制文件的工具套件。各种检测模式可用于计算代码覆盖率结果、分析源代码、应用配置文件指导的基本块优化、块（函数）级配置文件引导的重新排序，以及查找内存错误。

**插装技术类型**: 动态二进制

**下载地址**: [https://github.com/DynamoRIO/dynamorio](https://github.com/DynamoRIO/dynamorio)

**适用平台**: Windows, Linux, macOS, and Android

## Intel Pin

Pin可用于创建动态程序分析工具。使用 Pin 创建的工具称为 Pintools，可用于对应用程序进行程序分析。作为一种动态二进制插桩工具，插桩分析是在运行时对编译后的二进制文件进行的。因此，它无需重新编译源代码，可支持对动态生成代码的程序进行检测。

Pin 提供了丰富的应用程序接口，抽象出底层指令集的特异性，并允许将寄存器内容等上下文信息作为参数传递给注入代码。Pin 会自动保存和恢复被注入代码覆盖的寄存器，以便应用程序继续运行。此外，还可对符号和调试信息进行有限访问。 

**插装技术类型**: 动态二进制

**下载地址**: [https://www.intel.com/content/www/us/en/developer/articles/tool/pin-a-binary-instrumentation-tool-downloads.html](https://www.intel.com/content/www/us/en/developer/articles/tool/pin-a-binary-instrumentation-tool-downloads.html)

**适用平台**: Linux, Windows 和 macOS 

## Frida

Frida是原生应用程序的Greasemonkey，或者用更专业的术语来说，它是一个动态代码工具包。它能让你在原生应用程序中注入 JavaScript 片段或你自己的库。Frida 还为您提供了一些基于 Frida API 的简单工具。这些工具可以按原样使用，也可以根据需要进行调整，还可以作为如何使用 API 的示例。Frida广泛应用于移动应用和桌面应用的安全研究、逆向工程以及应用程序调试等。

**插装技术类型**: 动态二进制

**下载地址**: [https://github.com/frida/frida](https://github.com/frida/frida)

**适用平台**: Windows、macOS、GNU/Linux、iOS、watchOS、tvOS、Android、FreeBSD 和 QNX 

## JaCoCo

Syzygy 项目由一套工具组成，用于检测COFF对象文件和 PE二进制文件的工具套件。各种检测模式可用于计算代码覆盖率结果、分析源代码、应用配置文件指导的基本块优化、块（函数）级配置文件引导的重新排序，以及查找内存错误。

**插装技术类型**: 字节码

**下载地址**: [https://www.jacoco.org/jacoco/](https://www.jacoco.org/jacoco/)

**适用平台**: 

## Coverage.py

Coverage.py 是一款用于测量 Python 程序代码覆盖率的工具。它监控程序，记录代码的哪些部分已被执行，然后分析源代码，找出可能已被执行但未被执行的代码。 

**插装技术类型**: 源代码

**下载地址**: [https://coverage.readthedocs.io/en/7.3.2/](https://coverage.readthedocs.io/en/7.3.2/)

**适用平台**: