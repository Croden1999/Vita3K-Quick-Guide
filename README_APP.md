# 应用程序/游戏安装
应用程序以及游戏安装方式都是通用的，目前支持4种格式的安装：
1. [PKG](http://croden1999.github.io/Vita3K-quick-guide/README_APP#pkg)*：加密，需要work.bin文件或者输入zrif密钥。
2. [ZIP](http://croden1999.github.io/Vita3K-quick-guide/README_APP#zip)*：如PSN游戏/NoNpDrm，这是目前比较推荐的方式。
3. [VPK](http://croden1999.github.io/Vita3K-quick-guide/README_APP#vpk)：解密，本质也是zip格式，游戏的vpk只支持[Mai](http://croden1999.github.io/Vita3K-quick-guide/README_APP#mai)，不支持Vitamin。
4. 文件夹安装（仅适用于PC）：将游戏文件夹拖动到Vita3K图形用户界面窗口进行安装，对于安装格式要求较高（仅nonpdrm），且没有安装对话框显示，一般情况下不推荐该方式。

- *指当前推荐的格式。
- 支持选择目录文件夹内的多个zip/vpk安装。（仅PC）
- 不支持Vitamin提取的游戏（例如sce_module文件夹存在steroid.suprx），请更换其他非Vitamin的资源。

## PKG

打开Vita3K模拟器，在菜单栏点击`文件`—>`安装pkg`，`选择pkg`文件，`输入zrif密钥`或者`导入work.bin`文件，等待安装完成后运行即可。

关于获取pkg、zrif或者work.bin文件，pkg、zrif和work.bin可以在[NoPayStation](https://nopaystation.com)上搜索内容获取，或者在NPS Browser搜索内容右键复制pkg/zrif都是可以的。

![1](https://user-images.githubusercontent.com/61804715/131707016-03ff7df3-4891-4bec-8398-3311c88398f7.png)

## ZIP
使用zip安装NoNpDrm游戏相比pkg安装方式省略了需要输入密钥或者导入work.bin这一步，Vita3K会检测到NoNpDrm zip里的`sce_sys/package/work.bin`文件后解压解密安装。
- 注意：NoNpDrm zip不能直接解压到`ux0/app`里，如果直接解压NoNpDrm zip的游戏，在Vita3K中则无法运行该游戏（PSN游戏/NoNpDrm文件是加密未解密），因为Vita3K只读取解密的文件，所以必须要在Vita3K中安装。

在NPS Browser下载的内容可在NoPayStation文件夹里找到，NoNpDrm zip打包方式如下图所示：

![2](https://user-images.githubusercontent.com/61804715/188533955-393d4953-5da9-4956-a49a-35a42eec4bbd.png)

### PC
1. 打开Vita3K模拟器，在顶部选项栏点击`文件`->`安装zip、vpk`；
2. 点击`选择文件`，选择要安装的zip文件；
3. 等待安装完成后点确定运行即可。

- 如果是安装更多zip/vpk可以`选择目录`来进行多个安装。(仅适用于PC版本，安卓版本没有此选项)

### Android
1. 打开Vita3K模拟器，在顶部选项栏点击`文件`->`安装zip、vpk`；
2. 点击`选择文件`，选择要安装的zip文件；
3. 等待安装完成后点确定运行即可。

## VPK
通常Homebrew自制程序vpk都可以安装，但不保证所有都能运行，因为某些自制程序（如调用了PSV系统的库的自制程序或者使用Lua语言的程序）可能导致无法运行或者闪退。

- Vita3K不支持Vitamin提取的游戏安装，请更换其他非Vitamin的资源。

### Mai
PC/Android分为两种方式安装：
#### PC
安装
1. 直接拖到Vita3K模拟器图标安装，或者打开Vita3K模拟器；
2. 在顶部选项栏点击`文件`—>`安装zip、vpk`，点击`选择文件`，选择vpk文件后点确定；
3. 等待安装完成后点确定，运行游戏即可。

解压
1. 打开Vita3K模拟器，在顶部选项栏点击`文件`—>`打开存放路径`；
2. 将vpk改zip解压放到`ux0/app`文件夹里，并按照param.sfo文件信息将文件夹名字更改为标题ID（如PCSX00000）；
3. 在Vita3K中点击`刷新`选项显示应用程序图标，运行游戏即可。

#### Android
安装
1. 在顶部选项栏点击`文件`->`选择zip/vpk`，`安装zip、vpk`，点击`选择文件`，选择vpk文件后等待安装完成；
2. 安装完成后运行游戏即可。

解压
1. 打开谷歌原生文件管理器，将vpk文件后缀更改为zip，解压并检查标题ID（如PCSX00000）；
2. 检查无误后，选择复制，打开侧边栏复制到Vita3K存放路径的`ux0\app`中；
3. 在Vita3K中点击`刷新`选项显示应用程序，运行游戏即可。

## 相关的安装教程
- [追加内容DLC安装](http://croden1999.github.io/Vita3K-quick-guide/README_ADDCONT)
- [补丁安装](http://croden1999.github.io/Vita3K-quick-guide/README_PATCH)
