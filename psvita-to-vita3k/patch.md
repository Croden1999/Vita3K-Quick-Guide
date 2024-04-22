# 更新补丁安装
支持更新补丁的格式：
- pkg
- zip

## pkg
1. 打开Vita3K，在顶部菜单栏选择`文件`->`安装pkg`；
2. 选择`*.pkg`文件，选择`输入zrif密钥`或`导入work.bin/rif`文件，等待更新补丁安装完成。

## zip
分两种情况：
- nonpdrm（加密）
- decrypt（解密）

### nonpdrm
因为文件是加密的原因（包含sce_pfs、package）需要先获取原[标题ID]应用程序的work.bin文件，并放置在`sce_sys/package`文件夹中，将其压缩为zip，再到Vita3K上安装zip，等待更新补丁安装完成。

### decrypt
解密的文件安装较为方便，需要先在PSVita使用maidumptool提取解密补丁，提取位置在ux0:mai文件夹内，提取补丁名为[标题ID_patch]，将其压缩为zip，将此压缩包传到您的设备上，再到Vita3K上安装zip，等待更新补丁安装完成。

## 相关的安装教程
- [追加内容DLC安装](http://croden1999.github.io/Vita3K-Quick-Guide/vita3k/addcont)
- [应用程序/游戏安装](http://croden1999.github.io/Vita3K-Quick-Guide/vita3k/app)
