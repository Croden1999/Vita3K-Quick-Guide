# 追加内容安装
分为三种类型：
1. [pkg](http:///croden1999.github.io/Vita3K-Quick-Guide/addcont#pkg)（加密）
2. [zip](http://croden1999.github.io/Vita3K-Quick-Guide/addcont#zip)（如nonpdrm）
3. [decrypt](http://croden1999.github.io/Vita3K-Quick-Guide/addcont#decrypt)（解密，例如readdcont的DLC(s)、mai游戏附带的DLC(s)文件夹等解密的追加内容dlc文件）

你可以在Vita3K主页面的 【NPXS10026】 内容管理 应用程序，点击应用程序，找到对应游戏所安装的DLC信息。

## pkg
1. 打开Vita3K，在顶部菜单栏选择`文件`->`安装pkg`；
2. 选择`*.pkg`文件，选择`输入zrif密钥`或`导入work.bin`文件，等待安装完成后即可；
3. 可在Vita3K内容管理查看已安装的DLC，或在游戏中浏览已安装的DLC内容。

## zip
分两种情况：
- PSVita（已安装的DLC无法直接在Vita3K使用，需要在PSVita使用maidumptool提取解密的DLC）
- NPS
  
### PC
1. 打开Vita3K，在顶部菜单栏选择`文件`->`安装zip、vpk`；
2. `选择文件`或`选择目录`，选择`*.zip文件`或`目录`，等待安装完成即可;
3. 可在Vita3K内容管理查看已安装的DLC，或在游戏中浏览已安装的DLC内容。

### Android
1. 打开Vita3K，在顶部菜单栏选择`文件`->`安装zip、vpk`;
2. `选择文件`，选择`*.zip`文件，等待安装完成即可;
3. 可在Vita3K内容管理查看已安装的DLC，或在游戏中浏览已安装的DLC内容。

⚠注意：Android没有`选择目录`选项。

## decrypt
### PC
第一种，例如他人提供的readdcont/其他的解密DLC(s)就可使用。

1. 打开Vita3K，在顶部菜单栏选择`文件`->`打开存放路径`；
2. 将下载的dlc压缩包解压覆盖至`ux0/addcont/[标题ID]`文件夹内；
3. 可在Vita3K内容管理检查DLC是否放置正确，或在游戏中浏览已安装的DLC内容。

第二种，readdcont/其他的解密DLC(s)也可以打包为zip安装，前提是必须有param.sfo文件，否则可能无法正常安装，安装方式与zip一致。
### Android
第一种，例如他人提供的readdcont/其他的解密DLC(s)就可使用。

1. 打开谷歌原生文件管理器，解压readdcont/其他的解密DLC(s)补丁压缩包；
2. 选择复制，打开侧边栏复制覆盖到Vita3K存放路径的`ux0\addcont\[标题ID]`中；
3. 可在Vita3K内容管理检查DLC是否放置正确，或在游戏中浏览已安装的DLC内容。

第二种，readdcont/其他的解密DLC(s)也可以打包为zip安装，前提是必须有param.sfo文件，否则可能无法正常安装，安装方式与zip一致。

## 相关的安装教程
- [应用程序/游戏安装](http://croden1999.github.io/Vita3K-Quick-Guide/app)
- [补丁安装](http://croden1999.github.io/Vita3K-Quick-Guide/patch)
