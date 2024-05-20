# naiveproxy for Windows 7 and Windows 8.1

## 写在前面的话
* 这是Windows 7和Windows 8.1能正常使用的naiveproxy，源码来自naiveproxy项目官方。支持的操作系统Windows 7~Windows 10，但Windows 10有官方的预编译包可以直接使用。

* 作为计算机信息技术行业的一员，这两年到国外翻阅资料的条件越来越苛刻，TLS相关技术显得越来越紧要。

* 窘迫的是面对老旧的Windows系统，它们并非是主力设备，但目前运行在老硬件上，工作良好但也需要可靠的工具，目前也不能淘汰。所以在2023年的某个时间里，我给我自用的老系统编译了naiveproxy。

* Naiveproxy的作者在项目的Issues中明确表示不支持Windows 8.1及以下的系统，认为它们过时且不安全，但Windows 7、Windows 8.1的使用者还是很多，他们也想要naiveproxy，我就是其中的一员，这很矛盾。

* Naiveproxy的作者在Issues里删除了我回复其他想要Windows 7支持的人的二进制包，被标记成spam后删除，尽管我提示其他人如果不放心可先在Virustotal上安全扫描。我理解项目作者的洁癖，作为naiveproxy的上帝他不希望有人在自己的项目里做违背自己意愿的事，这是他的后花园，这也是他的权力。

* 我无意冒犯naiveproxy的作者，我只想帮助那些看起来像曾经自己的人，他们确实想要在Windows 7上使用，或配合其他GUI工具使用，例如NekoRay。

* 但有一群人真的需要这个可爱的工具。

## 项目简介
* 我[发布](https://github.com/PastelArtist/naiveproxy-for-Windows-7-and-Windows-8.1/releases)了预编译的64位包，源码来自naiveproxy官方[109.0.5414.74](https://github.com/klzgrad/naiveproxy/tree/109.0.5414.74)分支，这是Windows 7、Windows 8.1能支持的最高版本。

* 根据官方项目的[Wiki](https://github.com/klzgrad/naiveproxy/wiki/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87#%E8%87%AA%E8%A1%8C%E7%BC%96%E8%AF%91)我在Windows 10 LTSC 2019上编译，下面是相关章节引用：

>  ## 自行编译
> 
> 如果你不喜欢下载二进制文件，你可以自行编译NaïveProxy。
> 
> 要求:
> 
> * Ubuntu (apt-get install): git, python2, ninja-build (>= 1.7), pkg-config, libnss3-dev, curl, unzip, >  ccache (optional)
> * MacOS (brew install): git, ninja, ccache (optional)
> * Windows ([choco install](https://chocolatey.org/)): git, python2, ninja, visualstudio2017community. See [Chromium's page](https://chromium.googlesource.com/chromium/src/+/master/docs/windows_build_instructions.md#Visual-Studio) for detail on Visual Studio setup requirements.
> 
> 编译 (输出至 to `./out/Release/naive`):
> 
> ```
> $ git clone --depth 1 https://github.com/klzgrad/naiveproxy.git
> $ cd naiveproxy/src
> $ ./get-clang.sh
> $ ./build.sh
> ```
> 
> 改脚本会使用`curl`从Google服务器下载所需要的工具。你可能需要为curl设置一个代理环境变量，例如：`export ALL_PROXY=socks5h:/127.0.0.1:1080`。

* 同样的如果你不喜欢项目编译的包，欢迎自行编译，比心。
