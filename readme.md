**研究主题：牲畜体表信息的三维重建**



**第一部分：环境配置**

1.1奥比中光OpenNISDK安装（Linux）

奥比中光针对ZaroP1开发板和深度摄像机提供了相关的[OpenNI2的SDK](https://abzg-oss.oss-cn-shenzhen.aliyuncs.com/files/OpenNI-Linux-Arm64-2.3.0.65.rar),针对Windows/Linux/Android不同平台提供了相关的[安装文档](https://developer.orbbec.com.cn/technical_library.html?id=30).根据官方文档将OpenNI2配置完成，注意官方文档中说Linux平台内置驱动不需要额外安装，但是需要仔细阅读`README`文件：

```
OpenNI
------
Website: http://structure.io/openni
Building Prerequisites(前置依赖)
======================
Linux
-----
- GCC 4.x
    From: http://gcc.gnu.org/releases.html
    Or via apt:
    sudo apt-get install g++
- Python 2.6+/3.x
    From: http://www.python.org/download/
    Or via apt:
    sudo apt-get install python
- LibUSB 1.0.x
    From: http://sourceforge.net/projects/libusb/files/libusb-1.0/
    Or via apt:
    sudo apt-get install libusb-1.0-0-dev
- LibUDEV
    sudo apt-get install libudev-dev
- JDK 6.0
    From: http://www.oracle.com/technetwork/java/javase/downloads/jdk-6u32-downloads-1594644.html
    Or via apt:
    sudo apt-get install openjdk-6-jdk
- FreeGLUT3
    From: http://freeglut.sourceforge.net/index.php#download
    Or via apt:
    sudo apt-get install freeglut3-dev
- Doxygen
    From: http://www.stack.nl/~dimitri/doxygen/download.html#latestsrc
    Or via apt:
    sudo apt-get install doxygen
- GraphViz
    From: http://www.graphviz.org/Download_linux_ubuntu.php
    Or via apt:
    sudo apt-get install graphviz
```

将以上的依赖安装完成之后，运行其中示例代码还需要安装对应的USB驱动，驱动安装方法如下此方法将同目录下的USB驱动文件拷贝到系统目录中，并自动生成环境文件指明OpenNI的路径此方法将同目录下的USB驱动文件拷贝到系统目录中，并自动生成环境文件指明OpenNI的路径,进入安装包OpenNI目录中: 最后，在安装文件中找到`NiViewer`运行文件，若文件不能运行，查看`chmod`权限。经过以上的配置过程，OpenNI的环境就配置完成了。