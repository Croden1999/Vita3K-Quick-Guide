# Vita3K快速指南
### 前言
此快速指南基于[Vita3K快速入门](https://vita3k.org/quickstart)的教程编写，面向于对Vita3K刚接触和长时间使用模拟器的玩家用户，该指南会帮助对玩家用户需要了解安装和导入内容等操作，并使用PS Vita搭配Vita3K模拟器来提取安装，游玩应用及游戏。

### 免责声明
Vita3K不容忍盗版，此快速指南不提供任何游戏以及其他PS Vita相关软件的内容，您需要使用[NoNpDrm](https://github.com/TheOfficialFloW/NoNpDrm)或[FAGDec](https://github.com/CelesteBlue-dev/PSVita-RE-tools/tree/master/FAGDec/build)在您的PS Vita提取应用程序/游戏/更新补丁/追加内容DLC。当然，您可以在[VitaDB](https://vitadb.rinnegatamante.it)中获取自制程序。

## 支持的操作系统
- Windows（需要安装[Microsoft Visual C++ 2015-2022 Redistributable x64运行库](https://aka.ms/vs/17/release/vc_redist.x64.exe)）
- Linux（如Arch Linux、Ubuntu、Steam OS等）
- macOS
- Android

## 获取Vita3K
- 当前最新版本 [![Version](https://img.shields.io/github/v/release/Vita3K/Vita3K-builds?include_prereleases)](https://github.com/Vita3K/Vita3K/commits/master) | [历史版本](https://github.com/Vita3K/Vita3K-builds/releases) | [Android历史版本](https://github.com/Vita3K/Vita3K-Android/releases) | [更早版本（非全收录）](https://www.123684.com/s/izofjv-loog3) 

平台 | Vita3K官方 | gh-proxy代理 | kgithub代理 
--- | --- | --- | --- 
Android | [下载](https://github.com/Vita3K/Vita3K/releases/download/continuous/android-latest.apk) | [下载](https://gh-proxy.com/github.com/Vita3K/Vita3K/releases/download/continuous/android-latest.apk) | [下载](https://kkgithub.com/Vita3K/Vita3K/releases/download/continuous/android-latest.apk)
macOS | [下载](https://github.com/Vita3K/Vita3K/releases/download/continuous/macos-latest.dmg) | [下载](https://gh-proxy.com/github.com/Vita3K/Vita3K/releases/download/continuous/macos-latest.dmg) | [下载](https://kkgithub.com/Vita3K/Vita3K/releases/download/continuous/macos-latest.dmg)
Linux-arm64 (AppImage) | [下载](https://github.com/Vita3K/Vita3K/releases/download/continuous/Vita3K-aarch64.AppImage) | [下载](https://gh-proxy.com/github.com/Vita3K/Vita3K/releases/download/continuous/Vita3K-aarch64.AppImage) | [下载](https://kkgithub.com/Vita3K/Vita3K/releases/download/continuous/Vita3K-aarch64.AppImage)
Linux-arm64 (zip) | [下载](https://github.com/Vita3K/Vita3K/releases/download/continuous/ubuntu-aarch64-latest.zip) | [下载](https://gh-proxy.com/github.com/Vita3K/Vita3K/releases/download/continuous/ubuntu-aarch64-latest.zip) | [下载](https://kkgithub.com/Vita3K/Vita3K/releases/download/continuous/ubuntu-aarch64-latest.zip)
Linux-x86_64 (AppImage) | [下载](https://github.com/Vita3K/Vita3K/releases/download/continuous/Vita3K-x86_64.AppImage) | [下载](https://gh-proxy.com/github.com/Vita3K/Vita3K/releases/download/continuous/Vita3K-x86_64.AppImage) | [下载](https://kkgithub.com/Vita3K/Vita3K/releases/download/continuous/Vita3K-x86_64.AppImage)
Linux-x86_64 (zip) | [下载](https://github.com/Vita3K/Vita3K/releases/download/continuous/ubuntu-latest.zip) | [下载](https://gh-proxy.com/github.com/Vita3K/Vita3K/releases/download/continuous/ubuntu-latest.zip) | [下载](https://kkgithub.com/Vita3K/Vita3K/releases/download/continuous/ubuntu-latest.zip)
Windows-arm64 | [下载](https://github.com/Vita3K/Vita3K/releases/download/continuous/windows-arm64-latest.zip) | [下载](https://gh-proxy.com/github.com/Vita3K/Vita3K/releases/download/continuous/windows-arm64-latest.zip) | [下载](https://kkgithub.com/Vita3K/Vita3K/releases/download/continuous/windows-arm64-latest.zip)
Windows-x64 | [下载](https://github.com/Vita3K/Vita3K/releases/download/continuous/windows-latest.zip) | [下载](https://gh-proxy.com/github.com/Vita3K/Vita3K/releases/download/continuous/windows-latest.zip) | [下载](https://kkgithub.com/Vita3K/Vita3K/releases/download/continuous/windows-latest.zip)

## 配置要求
### PC

\ | 最低要求 | 推荐要求 
--- | --- | --- 
CPU | 任何x86_64/arm64 | 具有AVX指令集的x86_64/任何arm64
GPU | 支持OpenGL 4.4 | 支持Vulkan以及着色器互锁 
运行内存 | 4GB | 8GB+ 

- 如果您的配置低于最低要求，请更换PC硬件配置或者新设备


### Android

\ | 最低要求 | 推荐要求 
--- | --- | --- 
OS | Android 9 | Android 10+
CPU | arm64-v8a | arm64-v8a 
GPU | 支持OpenGL ES 3.2 | 支持Vulkan 
运行内存 | 4/6GB | 8GB+ 

- 如果您的配置低于最低要求，请更换新设备
- 如果您的设备只是硬件符合，系统软件版本过低可尝试更新（可能需要解锁设备bootloader，且使用第三方sideload），否则仍建议更换新设备

## Pref路径
各平台默认存放路径如下：
- Windows: `C:/Users/[username]/Appdata/Roaming/Vita3K/Vita3K`
- Linux: `~/.local/share/Vita3K/Vita3K`
- macOS: `~/Library/Application Support/Vita3K`
- Android: `/storage/emulated/0/Android/data/org.vita3k.emulator/files/vita`

## 教程
- [指南起点](http://croden1999.github.io/Vita3K-Quick-Guide/Start)

## Vita3K官方网站以及项目
- [官网](https://vita3k.org)
- [Vita3K项目库列表](https://github.com/Vita3K) & [Vita3K主项目库](https://github.com/Vita3K/Vita3K) 
- [商业游戏兼容性列表](https://vita3k.org/compatibility) & [商业游戏兼容性数据库](https://github.com/Vita3K/compatibility/issues)
- [自制程序兼容性列表](https://vita3k.org/compatibility-homebrew) & [自制程序兼容性数据库](https://github.com/Vita3K/homebrew-compatibility/issues)

## 交流
- [Vita3K Discord服务器（推荐）](https://discord.gg/MaWhJVH)
- [Vita3K Reddit社区](https://www.reddit.com/r/vita3k)
- [中文社区百度贴吧Vita3K吧](https://tieba.baidu.com/f?kw=vita3k&fr=index)
- [Vita3K爱好者QQ群 - 736751007](https://jq.qq.com/?_wv=1027&k=cg1vogjK)

## 捐赠
使用[Ko-fi](https://ko-fi.com/vita3k)为Vita3K项目组捐赠。

## 致谢
特别感谢开发团队和所有做出贡献的人员。
- 感谢提供建议或以其他方式使Vita3K项目成为可能的人，例如**Davee、korruptor、Rinnegatamante、ScHlAuChi、Simon Kilroy、TheFlow、xerpi、xyz、Yifan Lu**等。
- [Developers of Vita3K team / Vita3K小组开发人员](https://github.com/Vita3K)，开发人员包括**petmac、frangarcj、VelocityRa、1whatleytay、EXtremeExploit、HolyMcDiver、HorrorTroll、IllusionMan1212、KorewaWatchful、scribam、sunho、wfscans、Macdu、bookmist、pent0和Zangetsu38**。
- [And all contributors to the Vita3K emulator project / 以及所有Vita3K模拟器项目贡献者们](https://github.com/Vita3K/Vita3K/graphs/contributors)
- 感谢由**UnearthlyGoose**为Android虚拟按键设计overlay覆盖层。
