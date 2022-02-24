# DLC(s)追加内容安装教程
分为三种类型：
1. PKG（加密）
2. ZIP
3. 解密（如readdcont的DLC(s)、Mai游戏附带的DLC(s)文件夹等）

你可以在Vita3K主页面的 【NPXS10026】 内容管理 应用程序，点击Application（应用程序），找到对应游戏所安装的DLC信息。

## PKG
打开Vita3K模拟器，在菜单栏点击文件->安装pkg选项，选择pkg文件，输入zrif密钥或者导入work.bin文件，等待安装完成后即可。

关于获取zrif或者work.bin文件，zrif和work.bin可以在[NoPayStation](https://nopaystation.com)上搜索内容获取，或者在 NPS Browser 软件搜索内容右键复制zrif都是可以的。

## ZIP
可以在 NPS Browser 下载DLC(s)后在NoPayStation\addcont里找到【标题ID】的文件夹并打包zip，打包方式与vpk打包一致，之后打开Vita3K模拟器，在菜单栏点击文件->安装zip、vpk选项，点击Select File（选择），选择zip文件，等待安装完成后即可。如果是安装多个内容建议在安装zip/vpk选择文件夹可以进行多个安装。

## 解密
1. 第一种，例如他人提供的readdcont/其他的解密DLC(s)就可使用，打开Vita3K模拟器，点击顶部文件->打开存放路径，将你下载的解密dlc放置在ux0\addcont即可，正确路径是ux0\addcont\【标题ID】，可在Vita3K内容管理检查DLC(s)是否放置正确。
2. 第二种，也可以打包为zip安装，前提是必须有param.sfo文件，否则可能无法正常安装。

## MAI
为加载方式5的游戏附带有DLC(s)追加内容的dlcs文件夹，在ux0\app\(应用程序ID)文件夹里找到，将dlcs文件夹移动到ux0\addcont文件夹下，并重命名与【应用程序标题ID】一致，并使用MaiDumpTool将加载方式切换为0或4，可在Vita3K内容管理检查DLC(s)是否放置正确。
