# 驱动安装
仅适用高通Adreno GPU 6XX以及7XX系列的安装步骤，当前安装驱动有两种方式：
- 安装
- 解压

[Adreno驱动下载](https://github.com/K11MCH1/AdrenoToolsDrivers/releases)

## 安装
这是通常的安装步骤，基于K11MCH1的[Vita3K驱动安装](https://github.com/K11MCH1/AdrenoToolsDrivers/blob/main/docs/vita3k.md)步骤。

1. 下载对应您设备的GPU型号的驱动，打开Vita3K；
2. 在顶部选项栏点击`配置`—>`设置`，点击`GPU`选项卡；
3. 点击`Add custom driver（添加自定义驱动）`，然后选择驱动zip文件；
4. 在`设置`对话框的`GPU`选项卡中，在GPU的`Default`更换为已安装的新驱动，再运行游戏即可。

## 解压（进阶）
在此之前您需要将您的设备解锁Bootloader锁并刷入[Magisk](https://github.com/topjohnwu/Magisk/releases)进行root，才能进行下列步骤。

1. 下载对应您设备的GPU型号的驱动，打开MT管理器；
2. 转到根目录，找到/data/data/org.vita3k.emulator/files/driver路径；
3. 解压驱动到该目录，新建txt文件，并命名为`driver_name.txt`，文件中填写驱动so文件`[driver].so`后保存（例如`turnip-23.2.0-A7XX.adpkg_R3`驱动对应的驱动so文件是`vulkan.ad07XX.so`）;![](https://github.com/Croden1999/Vita3K-quick-guide/assets/61804715/f885b096-34ec-439f-b71c-9f1437a6c732)
4. 将所有文件属性更改为600权限、u0_aXXX（Vita3K）所有者和用户组（例如我的设备中Vita3K的应用ID是10295，即u0_a295），若不更改则会导致无法进入Vita3K；![](https://github.com/Croden1999/Vita3K-quick-guide/assets/61804715/9b339ef5-1946-40ee-a842-a5a719537d68)![](https://github.com/Croden1999/Vita3K-quick-guide/assets/61804715/b25e84f1-c239-4810-aeee-d3fc909d3388)
5. 完成后打开Vita3K；
6. 在顶部选项栏点击`配置`—>`设置`，点击`GPU`选项卡；
7. 在GPU中将`default`更换为新驱动，再运行游戏即可。![](https://github.com/Croden1999/Vita3K-quick-guide/assets/61804715/b98ff44b-9554-4282-be41-8b0f9ba6432a)
