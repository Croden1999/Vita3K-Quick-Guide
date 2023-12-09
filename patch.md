# 补丁安装
支持更新补丁的格式：
- pkg
- zip

## pkg
在NPS网站中下载[PSV_UPDATES.tsv](https://nopaystation.com/tsv/PSV_UPDATES.tsv)文件，使用Excel打开文件，搜索需要找的游戏名称的[标题ID]，找到对应【标题ID]pkg的URL地址，复制到浏览器或者在其他下载软件中下载pkg，再到Vita3K上安装pkg，选择与同[标题ID]work.bin文件或者输入zrif密钥，等待安装完成更新补丁后即可。

## zip
分两种情况：
- nonpdrm（加密）
- decrypt（解密）

### nonpdrm
因为文件是加密的原因（包含sce_pfs、package）需要先获取原[标题ID]应用程序的work.bin文件，并放置在`sce_sys/package`文件夹中，将其压缩为zip，再到Vita3K上安装zip，等待安装完成更新补丁后即可。

### decrypt
解密的文件安装较为方便，需要先在PSVita使用FAGDec或MaiDumpTool提取解密补丁，提取位置在ux0:mai文件夹内，提取补丁名为[标题ID_patch]，将其压缩为zip，将此压缩包传到您的设备上，再到Vita3K上安装zip，等待安装完成更新补丁后即可。

## 相关的安装教程
- [追加内容DLC安装](http://croden1999.github.io/Vita3K-quick-guide/addcont)
- [应用程序/游戏安装](http://croden1999.github.io/Vita3K-quick-guide/app)
