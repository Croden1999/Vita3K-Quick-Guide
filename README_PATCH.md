# 补丁安装
支持更新补丁的格式：
- [pkg](https://croden1999.github.io/Vita3K-quick-guide/README_PATCH#pkg)
- [zip](https://croden1999.github.io/Vita3K-quick-guide/README_PATCH#zip)
- [vpk](https://croden1999.github.io/Vita3K-quick-guide/README_PATCH#vpk)（如带MaiDump补丁的vpk）

你可以右键应用程序，选择信息，就可以浏览应用程序的版本。

## pkg
在NPS网站中下载[PSV_UPDATES.tsv](https://nopaystation.com/tsv/PSV_UPDATES.tsv)文件，使用Excel打开文件，搜索需要找的游戏名称的【标题ID】，找到对应【标题ID】pkg的URL地址，复制到浏览器或者在其他下载软件中下载pkg，再到Vita3K上安装pkg，选择与同[标题ID]work.bin文件或者输入zrif密钥，显示更新版本安装完成运行即可。

※注意：仅pkg或者zip（nonpdrm）可更新版本，mai不通用。

## zip
### PC
在NPS Browser下载游戏的更新补丁，下载完将`patch/[标题ID]`文件夹里的压缩为zip，再到Vita3K上安装zip，显示更新版本安装完成运行游戏即可。

### Android（需要PC）
在NPS Browser下载游戏的更新补丁，下载完将`patch/标题ID]`文件夹里的压缩为zip，将您的设备连接至PC，传输zip文件至根目录或者download文件夹即可，再到Vita3K上安装zip，显示更新版本安装完成运行游戏即可。

※注意：仅pkg或者zip（nonpdrm）可更新版本，mai不通用。

## vpk
一些人分享的MaiDump vpk的游戏里面覆盖应用程序补丁，例如文件名：0233_ASIA_PCSH00250_DEADORALIVEXTREME3VENUS_0115.vpk，后面这个0115就是应用程序的版本，即应用程序是1.15版本，安装方式请按照[应用程序/游戏安装](http://croden1999.github.io/Vita3K-quick-guide/README_APP#vpk)中vpk步骤操作。

## 语言补丁/mod补丁导入
### PC
打开Vita3K，右击应用程序图标选择打开文件夹，解压你所下载的补丁（如repatch或者语言补丁文件内容），将其放置覆盖到游戏文件夹里（路径为`ux0/app/[标题ID]`），覆盖补丁文件后运行游戏即可。

- 如果是readdcont，请按照[追加内容DLC安装](http://croden1999.github.io/Vita3K-quick-guide/README_ADDCONT#decrypt)操作。

### Android
安卓7至安卓10的data文件夹不受任何权限限制，可以直接将语言/mod补丁(repatch)覆盖到`/storage/emulated/0/Android/data/org.vita3k.emulator/files/vita/ux0/app/[标题ID]`文件夹内，再打开Vita3K运行游戏检查效果。

安卓11+由于存储策略限制无法直接导入文件至Android/data文件夹，仅能使用PC传输；除非使用mt管理器等软件对data文件夹授权，才能将语言/mod补丁（repatch）覆盖到`/storage/emulated/0/Android/data/org.vita3k.emulator/files/vita/ux0/app/[标题ID]`文件夹内。

- 如果是readdcont，请按照[追加内容DLC安装](http://croden1999.github.io/Vita3K-quick-guide/README_ADDCONT#decrypt)操作。

## 相关的安装教程
- [追加内容DLC安装](http://croden1999.github.io/Vita3K-quick-guide/README_ADDCONT)
- [应用程序/游戏安装](http://croden1999.github.io/Vita3K-quick-guide/README_APP)
