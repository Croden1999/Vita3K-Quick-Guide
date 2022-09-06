# 更新补丁安装
支持更新补丁的格式：
- PKG
- ZIP
- VPK（如带MaiDump补丁的vpk）

你可以右键应用程序，选择信息，就可以浏览应用程序的版本。

## PKG
可以在NPS网站中下载[PSV_UPDATES.tsv](https://nopaystation.com/tsv/PSV_UPDATES.tsv)文件用Excel打开，搜索你需要找的游戏名称的【标题ID】，找到对应【标题ID】pkg的URL地址，复制到浏览器或者在其他下载软件中下载pkg，再到Vita3K上安装pkg，选择与同【标题ID】work.bin/zrif密钥，显示更新版本安装完成运行即可。

※注意：仅pkg或者zip（nonpdrm）游戏可更新版本，mai游戏不通用。

## ZIP
可以在NPS Browser下载游戏的更新补丁，下载完将`patch\【标题ID】`文件夹里的压缩为zip，再到Vita3K上安装zip，显示更新版本安装完成运行游戏即可。

※注意：仅pkg或者zip（nonpdrm）游戏可更新版本，mai游戏不通用。

## VPK
一些人分享的MaiDump vpk的游戏里面覆盖应用程序补丁，例如文件名：0233_ASIA_PCSH00250_DEADORALIVEXTREME3VENUS_0115.vpk，后面这个0115就是应用程序的版本，即应用程序是1.15版本，安装方式请按照[应用程序/游戏安装](http://croden1999.github.io/Vita3K-quick-guide/README_APP#mai-vpk)操作。

## 语言补丁和MOD补丁导入
解压你所下载的补丁（如repatch或者语言补丁文件内容），将其放置覆盖到游戏文件夹里（路径大致为`ux0\app\【标题ID】`），覆盖补丁文件后打开Vita3K运行游戏即可。
