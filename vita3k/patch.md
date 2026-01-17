# 更新补丁安装
支持更新补丁的格式：
- pkg
- zip (nonpdrm)

## pkg
1. 打开Vita3K，在顶部菜单栏选择`文件`->`安装pkg`；
2. 选择`*.pkg`文件，选择`输入zrif密钥`或`导入work.bin/rif`文件，等待更新补丁安装完成。

## zip
因为文件是加密的原因（包含sce_pfs、package），Vita3K存在两种检测work.bin授权文件的方式。
1. 存放路径ux0/license内存在授权文件:
压缩更新补丁为zip，再到Vita3K上安装zip，等待更新补丁安装完成即可。

2. 压缩包sce_sys/package内存在授权文件:
需要先获取原[标题ID]应用程序的work.bin文件，并放置在`sce_sys/package`文件夹中，将其压缩为zip，再到Vita3K上安装zip，等待更新补丁安装完成即可。一般情况下按第一种方式安装，除非没有安装过work.bin授权文件才适合当前方式。

## 相关的安装教程
- [追加内容DLC安装](http://croden1999.github.io/Vita3K-Quick-Guide/vita3k/addcont)
- [应用程序/游戏安装](http://croden1999.github.io/Vita3K-Quick-Guide/vita3k/app)
