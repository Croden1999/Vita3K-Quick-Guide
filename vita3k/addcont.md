# 追加内容安装
分为三种类型：
1. [pkg](http:///croden1999.github.io/Vita3K-Quick-Guide/vita3k/addcont#pkg)（加密）
2. [zip](http://croden1999.github.io/Vita3K-Quick-Guide/vita3k/addcont#zip)（如nonpdrm）
3. [decrypt](http://croden1999.github.io/Vita3K-Quick-Guide/vita3k/addcont#decrypt)（解密，例如readdcont的DLC、mai游戏附带的DLC文件夹等解密的追加内容DLC文件）

## pkg
1. 打开Vita3K，PC在顶部菜单栏点击`文件`->`安装软件包pkg`；Android在主页中点击右下角`+`->`软件包（PKG）`；
2. 选择`pkg`文件，选择`输入zrif密钥`或`导入work.bin/rif`文件，等待安装完成后启动游戏；
3. 在游戏中浏览已安装的DLC内容。

## zip
PC与Android安装方式通用，分两种情况：
- PSVita（已安装的DLC无法直接在Vita3K使用，需要在PSVita使用maidumptool提取解密的DLC）
- NPS

1. 打开Vita3K，PC在顶部菜单栏点击`打开`->`安装压缩包（zip/vpk/vci）`；Android在主页中点击右下角`+`->`压缩包（ZIP/VPK）`；
2. `选择文件`或`选择目录`，选择`*.zip文件`或`目录`，等待安装完成即可;
3. 可在Vita3K内容管理查看已安装的DLC，或在游戏中浏览已安装的DLC内容。

## decrypt
### PC
第一种，例如他人提供的readdcont/其他的解密DLC就可使用。

1. 打开Vita3K，在顶部菜单栏选择`文件`->选择`打开模拟器存储路径`；
2. 将下载的DLC压缩包解压覆盖到`ux0/addcont/[TITLE_ID]`中；
3. 在游戏中浏览已安装的DLC内容。

第二种，readdcont/其他的解密DLC也可以打包为zip安装，前提是必须有param.sfo文件，否则可能无法正常安装，安装方式与zip一致。

### Android
第一种，例如他人提供的readdcont/其他的解密DLC就可使用。

1. 使用原生文件管理器，解压readdcont/其他的解密DLC补丁压缩包，复制里面的DLC；
2. 点击左上的图标开启文件管理器菜单，选择Vita3K，复制内容到`ux0/addcont/[TITLE_ID]`中；
3. 在游戏中浏览已安装的DLC内容。

第二种，readdcont/其他的解密DLC也可以打包为zip安装，前提是必须有param.sfo文件，否则可能无法正常安装，安装方式与zip一致。

## 相关的安装教程
- [应用程序/游戏安装](http://croden1999.github.io/Vita3K-Quick-Guide/vita3k/app)
- [更新补丁安装](http://croden1999.github.io/Vita3K-Quick-Guide/vita3k/patch)
- [授权安装](http://croden1999.github.io/Vita3K-Quick-Guide/vita3k/license)
