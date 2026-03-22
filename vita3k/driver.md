# 驱动安装及卸载
针对Android且Qualcomm Adreno GPU的设备，安装Mesa Turnip GPU驱动可以改善某些游戏的图形问题（并非所有），在此处下载[Adreno Mesa Turnip GPU驱动](https://github.com/K11MCH1/AdrenoToolsDrivers/releases)，GPU驱动安装仅适用于Qualcomm Adreno 6xx/7xx/8xx GPU。

- Android建议是安装/更新至更高的版本（至少为Android 11），搭配Mesa Turnip GPU驱动以获取更好的游玩体验。

## 注意
仅适用于Qualcomm Adreno GPU，不支持其他GPU的安装。
- 低于Qualcomm Adreno 6xx GPU无可用的GPU驱动。
- 对于Qualcomm Adreno 6xx GPU且Android 10，需要使用[turnip-v12-adpkg](https://github.com/K11MCH1/AdrenoToolsDrivers/releases/download/Turnip_v12/turnip-v12-adpkg.zip)的GPU驱动（该驱动存在易卡死以及闪退问题，无法长时间游玩，建议更新系统版本）。
- 对于Qualcomm Adreno 8xx GPU使用[turnip_a8xx](https://github.com/K11MCH1/AdrenoToolsDrivers/releases/download/v26.0.0-rc08/turnip_a8xx.zip)驱动，处于实验性阶段，谨慎使用。

## 安装
常规安装自定义驱动步骤，基于K11MCH1的[Vita3K驱动安装](https://github.com/K11MCH1/AdrenoToolsDrivers/blob/main/docs/vita3k.md)步骤：
1. 下载对应您设备的GPU型号的驱动，打开Vita3K；
2. 在顶部选项栏点击`配置`->`设置`，点击`GPU`选项卡；
3. 点击`添加自定义驱动`，然后选择驱动zip文件；
4. 在`设置`对话框的`GPU`选项卡中，在GPU的`Default`更换为已安装的新驱动。

## 卸载
### 常规
常规卸载自定义驱动步骤：
1. 打开Vita3K，在顶部选项栏点击`配置`->`设置`，点击`GPU`选项卡；
2. 点击`移除自定义驱动`。

### 修改
如果使用错误的GPU驱动无法打开Vita3K，解决步骤如下：
1. 使用原生文件管理器或[MT管理器](https://mt2.cn/download);
2. 在/Android/data/org.vita3k.emulator/files找到config.yml使用文本文档将其打开；
3. 将`custom-driver-name: [driver_name]`更改为`custom-driver-name: ""`，将`gpu-idx: 1`更改为`gpu-idx: 0`，编辑完后保存，令其使用默认的GPU驱动；
4. 打开Vita3K，在顶部选项栏点击`配置`->`设置`，点击`GPU`选项卡；
5. 切换不支持的驱动，点击`移除自定义驱动`。

## 特殊（PC）
仅针对PC版本，如果出现无法游玩以及闪退的情况，建议在显卡官方网站获取，下载并安装最新版本的显卡驱动，再尝试在Vita3K运行游玩。如果更新显卡驱动至最新版本，但仍低于OpenGL 4.4或Vulkan 1.0，且依旧无法游玩的情况下，请更换PC硬件配置或者新设备。
