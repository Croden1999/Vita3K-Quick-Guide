# Vita3K快速指南

### 前言
此快速指南基于[Vita3K快速入门](https://vita3k.org/quickstart)的教程，此快速指南会帮助刚接触Vita3K的新人们了解使用，不需要借助PS Vita，直接使用Vita3K模拟器就可以操作，并安装和游玩游戏。

### 免责声明
Vita3K不纵容盗版，此快速指南不提供任何游戏资源，您需要自己搜索并获取。

## 支持的操作系统
- Windows x64（需要安装[Microsoft Visual C++ 2015-2022 Redistributable x64运行库](https://aka.ms/vs/17/release/vc_redist.x64.exe)）
- Linux（如Ubuntu、Steam OS等）
- macOS
- Android（等待周日2月12日发布）

## 配置要求
### PC

\ | 最低要求 | 推荐要求 
--- | --- | --- 
CPU | 支持AVX指令集 | 支持AVX指令集 
GPU | 支持OpenGL 4.4 | 支持OpenGL 4.4或更高版本 
显卡着色器互锁 | × | ✓ 
运行内存 | 4GB | 8GB或者更高 


- 如果您的配置低于最低要求，请更换PC硬件配置或者新设备。

### Android
最低要求：
1. ARM64位设备
2. Vulkan 1.0版本
3. 安卓7及以上的版本（如果设备支持Vulkan 1.0，至少能在安卓7运行）

推荐要求：
1. 待更新（如果你的设备是最低要求，除了自制程序和2D游戏，其他不要指望能运行）
2. 安卓版本至少几个月内不会开源，意味没有其他人能构建以及修改它。
3. 安卓版本支持Adreno设备的自定义GPU驱动（特指高通处理器）。如果你的设备有Adreno 6xx系列GPU，建议使用Turnip驱动程序以获得较大的速度提升。Vita3K与adpkg驱动兼容。

- 如果您的配置低于最低要求，请更换新设备。

## 默认存放路径
- Windows: C:/Users/[user_name]/Appdata/Roaming/Vita3K/Vita3K
- Linux: ~/.local/share/Vita3K/Vita3K
- macOS: ~/Library/Application Support/Vita3K
- Android: /storage/emulated/0/Android/data/...

## 教程
### 主要
- [使用Vita3K](http://croden1999.github.io/Vita3K-quick-guide/README_USE_VITA3K)  
- [追加内容DLC安装](http://croden1999.github.io/Vita3K-quick-guide/README_ADDCONT)
- [应用程序/游戏安装](http://croden1999.github.io/Vita3K-quick-guide/README_APP)
- [补丁安装](http://croden1999.github.io/Vita3K-quick-guide/README_PATCH)

### 其他
- [保存数据导入/导出](http://croden1999.github.io/Vita3K-quick-guide/README_SAVEDATA)
- [主题安装](http://croden1999.github.io/Vita3K-quick-guide/README_THEME)
- [奖杯修改](http://croden1999.github.io/Vita3K-quick-guide/README_TROPHY)

## Vita3K官方网站以及项目
- [Vita3K官网](https://vita3k.org)
- [Vita3K模拟器项目](https://github.com/Vita3K/Vita3K)
- [Vita3K快速入门](https://vita3k.org/quickstart)
- [Vita3K商业游戏兼容性列表](https://vita3k.org/compatibility) & [Vita3K商业游戏兼容性数据库](https://github.com/Vita3K/compatibility/issues)
- [Vita3K自制程序兼容性列表](https://vita3k.org/compatibility-homebrew) & [Vita3K自制程序兼容性数据库](https://github.com/Vita3K/homebrew-compatibility/issues)

## Social
- [Vita3K Discord服务器（推荐）](https://discord.gg/MaWhJVH)
- [Vita3K Freenode IRC群聊](https://webchat.freenode.net/?channels=%23vita3k)
- [Vita3K Reddit社区](https://www.reddit.com/r/vita3k)
- [Vita3K模拟器QQ交流群](https://jq.qq.com/?_wv=1027&k=cg1vogjK)
- [百度贴吧Vita3K吧](https://tieba.baidu.com/f?kw=vita3k&fr=index)

## Donations
为Vita3K项目使用[Patreon](https://www.patreon.com/Vita3K)捐赠。

## Special Thanks
- [Developers of Vita3K team](https://github.com/Vita3K)
- [And contributors to the Vita3K emulator project](https://github.com/Vita3K/Vita3K/graphs/contributors)
