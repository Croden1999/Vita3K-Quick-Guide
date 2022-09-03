# 应用程序/游戏安装
应用程序以及游戏安装方式都是通用的，当前分为三种格式安装的支持：
1. pkg（加密，需要work.bin或者输入zrif密钥）
2. zip
3. vpk（解密，本质也是zip格式，游戏的vpk只支持Mai，不支持Vitamin）

- 支持选择文件夹内的多个zip/vpk安装。

### 关于其他安装问题
- 不支持Vitamin提取的游戏（例如名称带有FULLGAME），请更换其他非Vitamin的资源。
- 同时在安装前把文件命名为非中文再安装。
- 不要使用MaiDumpTool安装内容，安装没有任何效果和用途意义，只能作为Mai游戏切换加载方式使用。

## pkg

打开Vita3K模拟器，在菜单栏点击`文件`—>`安装pkg`，`选择pkg`文件，`输入zrif密钥`或者`导入work.bin`文件，等待安装完成后运行即可。

关于获取zrif或者work.bin文件，zrif和work.bin可以在[NoPayStation](https://nopaystation.com)上搜索内容获取，或者在 NPS Browser 软件搜索内容右键复制zrif都是可以的。

![2](https://user-images.githubusercontent.com/61804715/131707016-03ff7df3-4891-4bec-8398-3311c88398f7.png)

## zip
使用zip安装NoNpDrm游戏相比pkg安装方式省略了需要输入密钥或者导入work.bin这一步，Vita3K会检测到NoNpDrm zip里的`sce_sys/package/work.bin`文件后解压解密安装。
- 注意：NoNpDrm zip不能直接解压到`ux0/app`里，如果直接解压NoNpDrm zip的游戏，在Vita3K中则无法运行该游戏，所以必须要在Vita3K中安装。

可以在 NPS Browser 下载游戏后在`NoPayStation\app`里找到【标题ID】的文件夹并打包zip，NoNpDrm zip打包方式与vpk打包方式一致，之后拖入到Vita3K图标安装，或者打开Vita3K模拟器，在菜单栏点击`文件`->`安装zip、vpk`，点击`选择文件`，`选择zip`文件，等待安装完成后运行即可。如果是安装多个内容建议在安装zip/vpk选择文件夹可以进行多个安装。

## vpk
以mai vpk示例，分为两种加载方式（可以以记事本浏览`mai_moe/load_type.mai`文件显示的数字）：
1. 0（加载方式0）
2. 5（加载方式5）

- Vita3K不支持Vitamin的vpk格式安装。

### mai游戏（加载方式0）安装流程：
分为两种方式安装：
- 打开Vita3K模拟器，在菜单栏点击`文件`—>`打开存放路径`，将vpk改zip解压放到`ux0/app`文件夹里，并按照param.sfo文件信息将文件夹名字更改为标题ID（如PCSX00000），在Vita3K中点击`刷新`选项显示应用程序图标，运行游戏即可。
- 直接拖到Vita3K模拟器图标安装，或者打开Vita3K模拟器，在菜单栏点击`文件`—>`安装zip、vpk`，点击`选择文件`，`选择vpk`文件，等待安装完成后运行游戏即可。

### mai游戏（加载方式5）安装流程：
不能在Vita3K上直接安装的缺点是因为eboot是修改过的，只适用于实机，不能直接安装，直接安装可能会失败，需要解压到模拟器存储路径。切换加载方式或者替换为原版eboot，重新启动Vita3K模拟器再运行游戏即可。
- 切换加载方式流程（推荐）：
1. 在菜单栏点击`文件`->`打开存放路径`；
2. 在`ux0/app`文件夹中，将游戏vpk改为zip解压到此目录，并按照param.sfo文件信息将游戏文件夹名字改成标题ID（如PCSX00000）；
3. 在Vita3K上安装MaiDumpTool，并运行该应用程序，选择切换加载方式，选择对应的游戏设置为加载方式4（使用原版eboot.bin），之后重启Vita3K运行游戏即可。

![1](https://user-images.githubusercontent.com/61804715/131707916-51a83901-f72e-4f99-a17f-fc4f8a090802.png)

- 切换原版eboot流程：
1. 在菜单栏点击`文件`->`打开存放路径`；
2. 在`ux0/app`文件夹中，将游戏vpk改为zip解压到此目录，并按照param.sfo文件信息将游戏文件夹名字改成标题ID（如PCSX00000）；
3. 打开游戏文件夹，把在`mai_moe/eboot_origin.bin`(原版eboot文件)移动到`ux0/app/[标题ID]`文件夹，删除之前的eboot.bin，将eboot_origin.bin更名为eboot.bin；同时将dlc文件夹命名为同游戏ID文件夹，并移动ux0/addcont里，之后在Vita3K中点击`刷新`选项显示应用程序，运行游戏即可。

## 相关的安装教程
- [更新补丁安装](http://croden1999.github.io/Vita3K-quick-guide/README_PATCH)
- [追加内容安装](http://croden1999.github.io/Vita3K-quick-guide/README_ADDCONT)
