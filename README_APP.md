# 游戏安装教程
分为三种格式：
1. PKG（加密）
2. ZIP
3. VPK（解密）= ZIP格式

### 关于其他安装问题
- 不支持Vitamin提取的游戏（例如名称带有FULLGAME），请更换其他非Vitamin的资源。
- 同时在安装前把文件命名为非中文再安装。

## Mai VPK
分为两种加载方式（可以以记事本浏览mai_moe/load_type.mai文件显示的数字）：
1. 加载方式0（可直接安装，也可以选择文件夹多个安装）
2. 加载方式5

### mai游戏为加载方式0的安装流程：
分为两种方式安装：
- 打开Vita3K模拟器，在菜单栏点击文件—>打开存放路径选项，将vpk改zip解压放到ux0/app文件夹里，并按照param.sfo文件信息将文件夹名字更改为标题ID（如PCSX00000），在Vita3K模拟器点击Refresh刷新应用程序图标后再运行游戏即可。
- 直接拖到Vita3K模拟器图标安装，或者打开Vita3K模拟器，在菜单栏点击文件—>安装zip、vpk选项，点击Select File（选择），选择vpk文件，等待安装完成后运行游戏即可。

### mai游戏为加载方式5的安装流程：
不能在Vita3K上直接安装的缺点是因为eboot是修改过的，只适用于实机，不能直接安装，直接安装会崩溃闪退，需要解压。切换加载方式或者替换为原版eboot，重新启动Vita3K模拟器再运行游戏即可。
- 切换加载方式流程（推荐）：
1. 在菜单栏点击文件->打开存放路径选项；
2. 在ux0/app文件夹中，将游戏vpk改为zip解压到此目录，并按照param.sfo文件信息将游戏文件夹名字改成标题ID（如PCSX00000）；
3. 在Vita3K上安装MaiDumpTool，并运行该应用程序，选择切换加载方式，选择对应的游戏设置为加载方式0或者4，之后重新启动Vita3K模拟器运行游戏即可。

![1](https://user-images.githubusercontent.com/61804715/131707916-51a83901-f72e-4f99-a17f-fc4f8a090802.png)

- 切换原版eboot流程：
1. 在菜单栏点击文件->打开存放路径选项；
2. 在ux0/app文件夹中，将游戏vpk改为zip解压到此目录，并按照param.sfo文件信息将游戏文件夹名字改成标题ID（如PCSX00000）；
3. 打开游戏文件夹，把在mai_moe/eboot_origin.bin原版eboot替换掉，并改名为eboot.bin；同时将dlc文件夹命名为同游戏ID文件夹，并移动ux0/addcont里，之后点击Refresh刷新显示应用程序，运行游戏即可。

## ZIP
使用zip安装NoNpDrm游戏相比pkg安装方式省略了需要输入密钥或者导入work.bin这一步，Vita3K会检测到NoNpDrm zip里的sce_sys/package/work.bin文件后解压解密安装。
- 注意：NoNpDrm zip不能直接解压到ux0/app里，如果直接解压NoNpDrm zip的游戏，在Vita3K中则无法运行该游戏。

可以在 NPS Browser 下载游戏后在NoPayStation\app里找到【标题ID】的文件夹并打包zip，NoNpDrm zip打包方式与vpk打包方式一致，之后拖入到Vita3K图标安装，或者打开Vita3K模拟器，在菜单栏点击文件->安装zip、vpk选项，点击Select File（选择），选择zip文件，等待安装完成后运行即可。如果是安装多个内容建议在安装zip/vpk选择文件夹可以进行多个安装。

## PKG
打开Vita3K模拟器，在菜单栏点击文件—>安装pkg选项，选择pkg文件，输入zrif密钥或者导入work.bin文件，等待安装完成后运行即可。

关于获取zrif或者work.bin文件，zrif和work.bin可以在[NoPayStation](https://nopaystation.com)上搜索内容获取，或者在 NPS Browser 软件搜索内容右键复制zrif都是可以的。

![2](https://user-images.githubusercontent.com/61804715/131707016-03ff7df3-4891-4bec-8398-3311c88398f7.png)

## 与游戏安装相关的其他教程
- [->更新补丁安装教程](http://croden1999.github.io/Vita3K-quick-guide/README_patch)
- [->DLC追加内容安装教程](http://croden1999.github.io/Vita3K-quick-guide/README_dlc)
