# 追加内容安装
分为三种类型：
1. [pkg](http:///croden1999.github.io/Vita3K-quick-guide/README_ADDCONT#pkg)（加密）
2. [zip](http://croden1999.github.io/Vita3K-quick-guide/README_ADDCONT#zip)（如nonpdrm）
3. [decrypt](http://croden1999.github.io/Vita3K-quick-guide/README_ADDCONT#decrypt)（解密，例如readdcont的DLC(s)、mai游戏附带的DLC(s)文件夹等解密的追加内容dlc文件）

你可以在Vita3K主页面的 【NPXS10026】 内容管理 应用程序，点击应用程序，找到对应游戏所安装的DLC信息。

## pkg
关于获取zrif或者work.bin文件，zrif和work.bin可以在[NoPayStation](https://nopaystation.com)上搜索内容获取，或者在 NPS Browser 软件搜索内容右键复制zrif，然后打开Vita3K模拟器，在顶部选项栏`文件`——>`安装pkg`，`选择pkg文件`，`输入zrif密钥`或者`导入work.bin`文件，等待安装完成后即可，可在Vita3K内容管理查看已安装的DLC。

## zip
### PC
可以在 NPS Browser 下载DLC后在NoPayStation\addcont里找到【标题ID】的文件夹并打包zip，之后打开Vita3K模拟器，在顶部选项栏`文件`——>`安装zip、vpk`，点击`选择文件/选择目录`，`选择zip文件/目录`，等待安装完成即可，可在Vita3K内容管理查看已安装的DLC。

### Android（需要PC）
可以在 NPS Browser 下载DLC后在NoPayStation\addcont里找到【标题ID】的文件夹并打包zip，将您的设备连接至PC，传输至根目录或者download文件夹即可，打开Vita3K模拟器，在顶部选项栏`文件`——>`安装zip、vpk`，选择zip文件，等待安装完成即可，可在Vita3K内容管理查看已安装的DLC。

注：Android没有`选择目录`选项。

## decrypt
### PC
第一种，例如他人提供的readdcont/其他的解密DLC(s)就可使用，打开Vita3K模拟器，在顶部选项栏`文件`→`打开存放路径`，将下载的dlc压缩包覆盖至`ux0/addcont/[标题ID]`文件夹内，可在Vita3K内容管理检查DLC是否放置正确。

第二种，readdcont的dlc也可以打包为zip安装，前提是必须有param.sfo文件，否则可能无法正常安装。打开Vita3K模拟器，在顶部选项栏`文件`→`安装zip、vpk`，点击`选择文件/选择目录`，`选择zip文件/目录`，等待安装完成即可，可在Vita3K内容管理查看已安装的DLC。

### Android
安卓11+由于存储策略限制无法直接导入文件至Android/data文件夹，仅能使用PC传输；除非使用mt管理器等软件data文件夹。
例如他人提供的readdcont/其他的解密DLC(s)就可使用，将下载的dlc压缩包解压覆盖至`/storage/emulated/0/Android/data/org.vita3k.emulator/files/vita/ux0/addcont/[标题ID]`文件夹内，可在Vita3K内容管理检查DLC是否放置正确。

## 相关的安装教程
- [应用程序/游戏安装](http://croden1999.github.io/Vita3K-quick-guide/README_APP)
- [补丁安装](http://croden1999.github.io/Vita3K-quick-guide/README_PATCH)
