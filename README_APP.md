# 应用程序/游戏安装
应用程序以及游戏安装方式都是通用的，当前分为三种格式安装的支持：
1. [pkg](http://croden1999.github.io/Vita3K-quick-guide/README_APP#pkg)*：加密，需要work.bin文件或者输入zrif密钥
2. [zip](http://croden1999.github.io/Vita3K-quick-guide/README_APP#zip)*：nonpdrm，这是目前比较推荐的方式
3. [vpk](http://croden1999.github.io/Vita3K-quick-guide/README_APP#vpk)：解密，本质也是zip格式，游戏的vpk只支持Mai，不支持Vitamin

- 支持选择文件夹内的多个zip/vpk安装。
- *指当前推荐的格式。
- 不支持Vitamin提取的游戏（例如名称带有FULLGAME），请更换其他非Vitamin的资源。

## pkg

打开Vita3K模拟器，在菜单栏点击`文件`—>`安装pkg`，`选择pkg`文件，`输入zrif密钥`或者`导入work.bin`文件，等待安装完成后运行即可。

关于获取pkg、zrif或者work.bin文件，pkg、zrif和work.bin可以在[NoPayStation](https://nopaystation.com)上搜索内容获取，或者在 NPS Browser 搜索内容右键复制pkg/zrif都是可以的。

![1](https://user-images.githubusercontent.com/61804715/131707016-03ff7df3-4891-4bec-8398-3311c88398f7.png)

## zip
使用zip安装NoNpDrm游戏相比pkg安装方式省略了需要输入密钥或者导入work.bin这一步，Vita3K会检测到NoNpDrm zip里的`sce_sys/package/work.bin`文件后解压解密安装。
- 注意：NoNpDrm zip不能直接解压到`ux0/app`里，如果直接解压NoNpDrm zip的游戏，在Vita3K中则无法运行该游戏，所以必须要在Vita3K中安装。

在 NPS Browser 下载的内容可在NoPayStation文件夹里找到，NoNpDrm zip打包方式如下图所示：

![2](https://user-images.githubusercontent.com/61804715/188533955-393d4953-5da9-4956-a49a-35a42eec4bbd.png)

1. 打开Vita3K模拟器，在菜单栏点击`文件`->`安装zip、vpk`；
2. 点击`选择文件`，`选择zip`文件；
3. 等待安装完成后点确定运行即可。

- 如果是安装更多zip/vpk可以`选择目录`来进行多个安装。(仅适用于PC)

## vpk
通常Homebrew自制程序vpk都可以安装，但不保证所有都能运行，因为某些自制程序（如调用了PSV系统的库的自制程序或者使用Lua语言的程序）可能导致无法运行或者闪退。

游戏vpk以mai vpk示例，分为两种加载方式（可以以记事本浏览`mai_moe/load_type.mai`文件显示的数字）：
1. 0（加载方式0）
2. 5（加载方式5）

- Vita3K不支持Vitamin提取的游戏安装。

### Mai（加载方式0）
分为两种机型安装：
- 安装（PC）
1. 打开Vita3K模拟器在顶部选项栏点击`文件`—>`安装zip、vpk`，点击`选择文件`，点右下角选择项选择`PlayStation Vita homebrew software package (*.vpk)`，选择vpk文件后点确定
2. 等待安装完成后点确定，运行游戏即可。

- 安装（Android）
1. 打开Vita3K模拟器在顶部选项栏点击`文件`—>`安装zip、vpk`，选择vpk文件后就会开始安装
2. 等待安装完成后点确定，运行游戏即可。

### Mai（加载方式5）
不能在Vita3K上直接安装的缺点是因为eboot是修改过的，且带有dlc文件，mai修改后的eboot只适用于实机，不能直接在Vita3K中安装，直接安装会导致失败，需要解压到模拟器存储路径。替换为原版eboot，重新启动Vita3K模拟器再运行游戏即可。

PC
1. 在菜单栏点击`文件`->`打开存放路径`；
2. 在`ux0/app`文件夹中，将游戏vpk改为zip解压到此目录，并按照param.sfo文件信息将游戏文件夹名字改成标题ID（如PCSX00000）；
3. 打开游戏文件夹，把`mai_moe/eboot_origin.bin`(原版eboot文件)移动到`ux0/app/[标题ID]`文件夹，删除该文件夹的`eboot.bin`，将`eboot_origin.bin`更名为`eboot.bin`；
4. 将dlc文件夹命名为同游戏ID文件夹，并移动`ux0/addcont`里，若游戏文件夹内没有dlc文件夹可以跳过此操作。
5. 在Vita3K中点击`刷新`选项显示应用程序，运行游戏即可。

Android（需要PC）
1. 将你的设备连接至PC，vpk更改为zip后缀，解压文件传输至设备的`Android/data/org.vita3k.emulator/files/vita/ux0/app`文件夹中；
2. 在`app`文件夹中，并按照param.sfo文件信息将游戏文件夹名字改成标题ID（如PCSX00000）；
3. 把`mai_moe/eboot_origin.bin`(原版eboot文件)移动到`ux0/app/[标题ID]`文件夹，删除该文件夹的`eboot.bin`，将`eboot_origin.bin`更名为`eboot.bin`；
4. 将dlc文件夹命名为同标题ID文件夹，并移动`ux0/addcont`里，若游戏文件夹内没有dlc文件夹可以跳过此操作。
5. 在Vita3K中点击`刷新`选项显示应用程序，运行游戏即可。

## 相关的安装教程
- [追加内容DLC安装](http://croden1999.github.io/Vita3K-quick-guide/README_ADDCONT)
- [补丁安装](http://croden1999.github.io/Vita3K-quick-guide/README_PATCH)
