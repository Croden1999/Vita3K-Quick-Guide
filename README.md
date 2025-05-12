# Vita3K快速指南
简体中文 / [繁體中文（待更新）](http://croden1999.github.io/Vita3K-Quick-Guide/README-CH)

### 前言
此快速指南基于[Vita3K快速入门](https://vita3k.org/quickstart)的教程，此快速指南会帮助刚接触Vita3K的新人们了解使用，使用PS Vita搭配Vita3K模拟器来提取并安装，游玩应用及游戏。

### 免责声明
Vita3K不容忍盗版，此快速指南不提供任何游戏以及其他PS Vita相关软件的内容，您需要使用[NoNpDrm](https://github.com/TheOfficialFloW/NoNpDrm)或[FAGDec](https://github.com/CelesteBlue-dev/PSVita-RE-tools/tree/master/FAGDec/build)在您的PS Vita提取应用程序/游戏/更新补丁/追加内容DLC。当然，您可以在[VitaDB](https://vitadb.rinnegatamante.it)中获取自制程序。

## 支持的操作系统
- Windows x64（需要安装[Microsoft Visual C++ 2015-2022 Redistributable x64运行库](https://aka.ms/vs/17/release/vc_redist.x64.exe)）
- Linux（如Ubuntu、Steam OS等）
- macOS
- Android

## 下载Vita3K
当前版本及更新记录
- master [![Version](https://img.shields.io/github/v/release/Vita3K/Vita3K-builds?include_prereleases)](https://github.com/Vita3K/Vita3K/commits/master)
- Android [![Version](https://img.shields.io/github/v/release/Vita3K/Vita3K-Android?include_prereleases)](https://github.com/Vita3K/Vita3K-Android/commits/android/)

### Vita3K官方
[Windows x64](https://github.com/Vita3K/Vita3K/releases/download/continuous/windows-latest.zip) | 
[Linux (AppImage)](https://github.com/Vita3K/Vita3K/releases/download/continuous/Vita3K-x86_64.AppImage) | 
[Linux (zip)](https://github.com/Vita3K/Vita3K/releases/download/continuous/ubuntu-latest.zip) | 
[macOS](https://github.com/Vita3K/Vita3K/releases/download/continuous/macos-latest.dmg) |
[Android](https://github.com/Vita3K/Vita3K-Android/releases/download/v12/vita3k-android-release-12.apk)

### gh-proxy代理
[Windows x64](https://gh-proxy.com/github.com/Vita3K/Vita3K/releases/download/continuous/windows-latest.zip)  | 
[Linux (AppImage)](https://gh-proxy.com/github.com/Vita3K/Vita3K/releases/download/continuous/Vita3K-x86_64.AppImage)  | 
[Linux (zip)](https://gh-proxy.com/github.com/Vita3K/Vita3K/releases/download/continuous/ubuntu-latest.zip) | 
[macOS](https://gh-proxy.com/github.com/Vita3K/Vita3K/releases/download/continuous/macos-latest.dmg) | 
[Android](https://gh-proxy.com/github.com/Vita3K/Vita3K-Android/releases/download/v12/vita3k-android-release-12.apk)

### kkgithub代理
[Windows x64](https://kkgithub.com/Vita3K/Vita3K/releases/download/continuous/windows-latest.zip)  | 
[Linux (AppImage)](https://kkgithub.com/Vita3K/Vita3K/releases/download/continuous/Vita3K-x86_64.AppImage)  | 
[Linux (zip)](https://kkgithub.com/Vita3K/Vita3K/releases/download/continuous/ubuntu-latest.zip) | 
[macOS](https://kkgithub.com/Vita3K/Vita3K/releases/download/continuous/macos-latest.dmg) | 
[Android](https://kkgithub.com/Vita3K/Vita3K-Android/releases/download/v12/vita3k-android-release-12.apk)

### Vita3K历史版本
[Vita3K构建存储库](https://github.com/Vita3K/Vita3K-builds/releases) | 
[Vita3K-Android构建存储库](https://github.com/Vita3K/Vita3K-Android/releases)

## 配置要求
### PC

\ | 最低要求 | 推荐要求 
--- | --- | --- 
CPU | 支持AVX指令集 | 支持AVX指令集 
GPU | 支持OpenGL 4.4 | 支持OpenGL 4.4或更高版本 / Vulkan
显卡着色器互锁 | × | ✓ 
运行内存 | 4GB | 8GB或者更高 

- 如果您的配置低于最低要求，请更换PC硬件配置或者新设备。

### Android
最低要求：
1. ARM64设备
2. OpenGL ES 3.2（实验性）或Vulkan 1.0
3. Android 8及以上（注意：如果您的设备支持OpenGL ES 3.2或Vulkan，则为Android 8或更高版本），但建议最低Android 11或更高版本，以获取更好的游玩体验

- 如果您的配置低于最低要求，请更换新设备。

## Default Perf Path
各平台默认存放路径如下：
- Windows: `C:/Users/[username]/Appdata/Roaming/Vita3K/Vita3K`
- Linux: `~/.local/share/Vita3K/Vita3K`
- macOS: `~/Library/Application Support/Vita3K`
- Android: `/storage/emulated/0/Android/data/org.vita3k.emulator/files/vita`

## 教程
- [PSVita to Vita3K](http://croden1999.github.io/Vita3K-Quick-Guide/psvita-to-vita3k)
- [单独使用Vita3K](http://croden1999.github.io/Vita3K-Quick-Guide/vita3k)

## Vita3K官方网站以及项目
- [Vita3K官网](https://vita3k.org) & [Vita3K快速入门](https://vita3k.org/quickstart)
- [Vita3K项目](https://github.com/Vita3K) & [Vita3K repo](https://github.com/Vita3K/Vita3K) & [Vita3K-Android repo](https://github.com/Vita3K/Vita3K-Android)
- [Vita3K商业游戏兼容性列表](https://vita3k.org/compatibility) & [Vita3K商业游戏兼容性数据库](https://github.com/Vita3K/compatibility/issues)
- [Vita3K自制程序兼容性列表](https://vita3k.org/compatibility-homebrew) & [Vita3K自制程序兼容性数据库](https://github.com/Vita3K/homebrew-compatibility/issues)

## Communication
- [Vita3K Discord服务器（推荐）](https://discord.gg/MaWhJVH)
- [Vita3K Reddit社区](https://www.reddit.com/r/vita3k)
- [中文社区百度贴吧Vita3K吧](https://tieba.baidu.com/f?kw=vita3k&fr=index)
- [Vita3K爱好者QQ群 - 736751007](https://jq.qq.com/?_wv=1027&k=cg1vogjK)

## Donation
可以使用[Ko-fi](https://ko-fi.com/vita3k)为Vita3K项目组捐赠。

## Special Thanks
特别感谢开发团队和所有做出贡献的人员。
- 感谢提供建议或以其他方式使Vita3K项目成为可能的人，例如Davee、korruptor、Rinnegatamante、ScHlAuChi、Simon Kilroy、TheFlow、xerpi、xyz、Yifan Lu等。
- [Developers of Vita3K team / Vita3K小组开发人员](https://github.com/Vita3K)，开发人员包括petmac、frangarcj、VelocityRa、1whatleytay、EXtremeExploit、HolyMcDiver、HorrorTroll、IllusionMan1212、KorewaWatchful、scribam、sunho、wfscans、Macdu、bookmist、pent0和Zangetsu38。
- [And all contributors to the Vita3K emulator project / 以及所有Vita3K模拟器项目贡献者们](https://github.com/Vita3K/Vita3K/graphs/contributors)
