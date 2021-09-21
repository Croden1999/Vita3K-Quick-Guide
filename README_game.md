# 游戏安装教程
分为三种格式：
1. PKG（加密）
2. ZIP
3. VPK（解密）= ZIP格式

关于patch游戏更新补丁
- 目前只支持Mai的游戏patch补丁，不支持PKG/ZIP的游戏patch补丁。

# Mai VPK游戏的安装
分为两种加载方式（可以以记事本浏览mai_moe/load_type.mai文件显示的数字）：
1. 加载方式0（可直接安装，也可以选择文件夹多个安装）
2. 加载方式5

mai游戏为加载方式0的安装流程：

分两种方式安装，推荐第1种安装方式，因为带补丁的游戏在Vita3K模拟器安装会放到ux0/patch里面。
- 打开Vita3K模拟器，在菜单栏点击文件—>打开存放路径选项，将vpk改zip解压放到ux0/app文件夹里，并按照param.sfo文件信息将文件夹名字更改为游戏ID（如PCSX00000），再去Vita3K模拟器运行游戏。

- 直接拖到Vita3K模拟器图标安装，或者打开Vita3K模拟器，在菜单栏点击文件—>安装zip、vpk选项，点击Select File（选择），选择vpk文件，等待安装完成后需要在菜单栏文件打开存放路径文件夹，在ux0/patch文件夹找到该游戏移动到ux0/app，点击Refresh刷新应用显示游戏运行即可。

mai游戏为加载方式5的安装流程：

不能在Vita3K上直接安装的缺点是因为eboot是修改过的，只适用于实机，不能直接安装，直接安装会崩溃闪退，需要解压。

- 切换加载方式流程（推荐）：
1. 在菜单栏点击文件—>打开存放路径选项；
2. 在ux0/app文件夹中，将游戏vpk改为zip解压到此目录，并按照param.sfo文件信息将游戏文件夹名字改成游戏ID（如PCSX00000）；
3. 在Vita3K上安装MaiDumpTool，并运行该应用程序，选择切换加载方式，选择对应的游戏设置为加载方式0，之后重新启动Vita3K模拟器运行游戏即可。

![](https://user-images.githubusercontent.com/61804715/131707916-51a83901-f72e-4f99-a17f-fc4f8a090802.png)

- 切换原版eboot流程：
1. 在菜单栏点击文件—>打开存放路径选项；
2. 在ux0/app文件夹中，将游戏vpk改为zip解压到此目录，并按照param.sfo文件信息将游戏文件夹名字改成游戏ID（如PCSX00000）；
3. 打开游戏文件夹，把在mai_moe/eboot_origin.bin原版eboot替换掉，并改名为eboot.bin；同时将dlc文件夹命名为同游戏ID文件夹，并移动ux0/addcont里，之后点击Refresh刷新显示应用程序，运行游戏即可。

# ZIP游戏的安装
相比pkg安装方式省略了需要输入密钥或者导入work.bin这一步，Vita3K会检测到nonpdrm zip里的sce_sys/package/work.bin文件后解压解密安装。
- 注意：nonpdrm zip不能直接解压到ux0/app里，如果直接解压nonpdrm zip的游戏，在Vita3K中则无法运行该游戏。

可以在 NPS Browser 下载游戏后在NoPayStation\app里找到【标题ID】的文件夹并打包zip，nonpdrm zip打包方式与vpk打包方式一致，之后拖入到Vita3K图标安装，或者打开Vita3K模拟器，在菜单栏点击文件—>安装zip、vpk选项，点击Select File（选择），选择zip文件，等待安装完成后运行即可。如果是安装多个内容建议在安装zip/vpk选择文件夹可以进行多个安装。

# PKG游戏的安装
打开Vita3K模拟器，在菜单栏点击文件—>安装pkg选项，选择pkg文件，输入zrif密钥或者导入work.bin文件，等待安装完成后运行即可。

关于获取zrif或者work.bin文件，zrif和work.bin可以在[NoPayStation](https://nopaystation.com)上搜索内容获取，或者在 NPS Browser 软件搜索内容右键复制zrif都是可以的。

![](https://user-images.githubusercontent.com/61804715/131707016-03ff7df3-4891-4bec-8398-3311c88398f7.png)
