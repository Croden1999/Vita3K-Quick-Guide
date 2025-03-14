# 应用程序/游戏安装
应用程序以及游戏安装方式都是通用的，目前支持4种格式的安装：
1. [pkg](http://croden1999.github.io/Vita3K-Quick-Guide/vita3k/app#pkg)：加密，需要work.bin/rif文件或者输入zrif密钥。
2. [zip](http://croden1999.github.io/Vita3K-Quick-Guide/vita3k/app#zip)：如PSN游戏/NoNpDrm，这是目前比较推荐的方式。
3. [vpk](http://croden1999.github.io/Vita3K-Quick-Guide/vita3k/app#vpk)：解密，本质也是zip格式，游戏的vpk只支持Mai，自制程序vpk也支持（并非所有）；不支持Vitamin，不要企图安装或运行。
4. 文件夹安装（仅PC）：将游戏文件夹拖动到Vita3K图形用户界面窗口进行安装，对于安装格式要求较高（仅NoNpDrm），且没有安装对话框显示，一般情况下不推荐该方式。

## pkg
PC以及Android步骤通用：
1. 打开Vita3K模拟器，在顶部菜单栏点击`文件`->`安装pkg`；
2. 选择`pkg`文件，选择`导入work.bin/rif`或`输入zrif密钥`；
3. 若选择`导入work.bin/rif`你需要选择对应正确的标题ID的授权文件才能安装成功；
4. 若选择`输入zrif密钥`你需要输入正确的zrif密钥才能安装成功；
5. 等待安装完成后点确定，运行应用程序即可。

## zip
使用zip安装NoNpDrm游戏相比pkg安装方式省略了需要输入密钥或者导入work.bin这一步，Vita3K会检测到NoNpDrm zip里的`sce_sys/package/work.bin`文件后解压解密安装。
- 注意：NoNpDrm zip不能直接解压到`ux0/app`里，如果直接解压NoNpDrm zip的游戏，在Vita3K中则无法运行该游戏（PSN/NoNpDrm游戏是加密未解密的文件），Vita3K只读取解密的文件，因此必须要在Vita3K中安装。

### PC
1. 打开Vita3K模拟器，在顶部菜单栏点击`文件`->`安装zip、vpk`；
2. 点击`选择文件`，选择`zip`文件；
3. 等待安装完成后点确定，运行应用程序即可。

- 如果是安装更多zip/vpk可以`选择目录`来进行多个安装。(仅适用于PC版本，安卓版本没有此选项)

### Android
1. 打开Vita3K模拟器，在顶部菜单栏点击`文件`->`安装zip、vpk`；
2. 点击`选择文件`，选择`zip`文件；
3. 等待安装完成后点确定，运行应用程序即可。

## vpk
通常Homebrew自制程序vpk都可以安装，但不保证所有都能运行，因为某些自制程序（如调用了PSV系统的库的自制程序或者使用Lua语言的程序）可能导致无法运行或者闪退。
- 不要企图安装Vitamin，Vita3K不支持Vitamin提取的游戏安装以及运行，请更换其他非Vitamin的资源。

PC/Android分为安装/解压两种方式安装。

### PC
安装：
1. 打开Vita3K，在顶部菜单栏点击`文件`->`安装zip、vpk`；
2. 点击`选择文件`，选择`vpk`文件；
3. 等待安装完成后点确定，运行应用程序即可。

解压：
1. 打开Vita3K，在顶部菜单栏点击`文件`->`打开存放路径`；
2. 将vpk改zip解压放到`ux0/app`文件夹里，并按照param.sfo文件信息将文件夹名字更改为标题ID（如PCSX00000）；
3. 在Vita3K中点击`刷新`选项显示应用程序图标，运行应用程序即可。

### Android
安装：
1. 打开Vita3K，在顶部菜单栏点击`文件`->`安装zip、vpk`；
2. 点击`选择文件`，选择`vpk`文件；
3. 等待安装完成后点确定，运行应用程序即可。

解压：
1. 打开原生文件管理器，将vpk文件后缀更改为zip，解压并检查标题ID（如PCSX00000）；
2. 检查无误后，选择复制，打开侧边栏粘贴到Vita3K存放路径的`ux0\app`中；
3. 在Vita3K中点击`刷新`选项显示应用程序，运行应用程序即可。

## 相关的安装教程
- [追加内容DLC安装](http://croden1999.github.io/Vita3K-Quick-Guide/vita3k/addcont)
- [更新补丁安装](http://croden1999.github.io/Vita3K-Quick-Guide/vita3k/patch)
