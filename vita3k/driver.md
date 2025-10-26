# 驱动安装及卸载
针对Android且Qualcomm Adreno GPU的设备，安装Mesa Turnip GPU驱动可以改善某些游戏的图形问题（并非所有），在此处下载[Adreno Mesa Turnip GPU驱动](https://github.com/K11MCH1/AdrenoToolsDrivers/releases)，仅适用于Qualcomm Adreno 6xx/7xx GPU的安装步骤，当前安装驱动有两种方式：
- 安装
- 解压

Android建议是安装/更新至更高的版本（至少为Android 11），搭配Mesa Turnip GPU驱动以获取更好的游玩体验。

### 注意
仅适用于Qualcomm Adreno GPU，不支持其他GPU的安装。
- 低于Qualcomm Adreno 6xx GPU无可用的GPU驱动。
- 对于Qualcomm Adreno 6xx GPU且Android 10，需要使用[turnip-v12-adpkg](https://github.com/K11MCH1/AdrenoToolsDrivers/releases/download/Turnip_v12/turnip-v12-adpkg.zip)的GPU驱动（该驱动存在易卡死以及闪退问题，无法长时间游玩，建议更新系统版本）。此外该GPU不支持Mesa Turnip GPU驱动25.x.x后的版本，使用后会导致崩溃闪退，最高仅能使用24.x.x包括之前版本的GPU驱动。
- 对于Qualcomm Adreno 8xx GPU无可用的Mesa Turnip GPU驱动。

## 安装
### 常规
常规安装自定义驱动步骤，基于K11MCH1的[Vita3K驱动安装](https://github.com/K11MCH1/AdrenoToolsDrivers/blob/main/docs/vita3k.md)步骤：

1. 下载对应您设备的GPU型号的驱动，打开Vita3K；
2. 在顶部选项栏点击`配置`->`设置`，点击`GPU`选项卡；
3. 点击`Add custom driver（添加自定义驱动）`，然后选择驱动zip文件；
4. 在`设置`对话框的`GPU`选项卡中，在GPU的`Default`更换为已安装的新驱动。

### 解压（进阶）
在此之前您需要将您的设备解锁Bootloader，并使用[apatch](https://github.com/bmax121/APatch/releases)/[KernelSU](https://github.com/tiann/KernelSU/releases)/[Magisk](https://github.com/topjohnwu/Magisk/releases)为您的设备获取Root权限，另外安装[MT管理器](https://mt2.cn/download)，才能进行下列步骤。

- 强烈提醒：未了解相关知识不建议使用该步骤，它可能会永久破坏您的设备数据。

1. 下载对应您设备的GPU型号的驱动，打开MT管理器，并授权Root权限；
2. 转到设备根目录（即/），找到/data/data/org.vita3k.emulator/files/driver路径；
3. 解压驱动到该目录，新建txt文件，并命名为`driver_name.txt`，文件中填写驱动so文件`[driver].so`后保存（例如`turnip-23.2.0-A7XX.adpkg_R3`驱动对应的驱动so文件是`vulkan.ad07XX.so`）;![](https://github.com/Croden1999/Vita3K-quick-guide/assets/61804715/f885b096-34ec-439f-b71c-9f1437a6c732)
4. 将所有文件属性更改为600权限、u0_aXXX（Vita3K）所有者和用户组（例如我设备中显示Vita3K的应用ID是10295，即u0_a295，其他设备的应用ID均有不同），若不更改则导致无法进入Vita3K；![](https://github.com/Croden1999/Vita3K-quick-guide/assets/61804715/9b339ef5-1946-40ee-a842-a5a719537d68)![](https://github.com/Croden1999/Vita3K-quick-guide/assets/61804715/b25e84f1-c239-4810-aeee-d3fc909d3388)
5. 设置完成后打开Vita3K，在顶部选项栏点击`配置`->`设置`，点击`GPU`选项卡，在GPU中将`Default`更换为新驱动。![](https://github.com/Croden1999/Vita3K-quick-guide/assets/61804715/b98ff44b-9554-4282-be41-8b0f9ba6432a)

## 卸载
### 常规
常规卸载自定义驱动步骤：

1. 打开Vita3K，在顶部选项栏点击`配置`->`设置`，点击`GPU`选项卡；
2. 点击`Remove custom driver（移除自定义驱动）`。

### 修改
如果使用错误的GPU驱动无法打开Vita3K，解决步骤如下：

1. 使用原生文件管理器或[MT管理器](https://mt2.cn/download);
2. 在/Android/data/org.vita3k.emulator/files找到config.yml使用文本文档将其打开；
3. 将`custom-driver-name: [driver_name]`更改为`custom-driver-name: ""`，将`gpu-idx: 1`更改为`gpu-idx: 0`，编辑完后保存，令其使用默认的GPU驱动；
4. 打开Vita3K，在顶部选项栏点击`配置`->`设置`，点击`GPU`选项卡；
5. 切换不支持的驱动，点击`Remove custom driver（移除自定义驱动）`。

## 特殊（PC）
仅针对PC版本，如果出现无法游玩以及闪退的情况，建议在显卡官方网站获取，下载并安装最新版本的显卡驱动，再尝试在Vita3K运行游玩。如果更新显卡驱动至最新版本，但仍低于OpenGL 4.4或Vulkan 1.0，且依旧无法游玩的情况下，请更换PC硬件配置或者新设备。
