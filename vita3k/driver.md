# 驱动安装及卸载
针对Android且Qualcomm Adreno GPU的设备，安装Mesa Turnip GPU驱动可以改善某些游戏的图形问题（并非所有），在此处下载[Adreno Mesa Turnip GPU驱动](https://github.com/K11MCH1/AdrenoToolsDrivers/releases)，GPU驱动安装仅适用于Qualcomm Adreno 6xx/7xx/8xx GPU。

- Android建议是安装/更新至更高的版本（至少为Android 11），搭配Mesa Turnip GPU驱动以获取更好的游玩体验。

## 注意
仅适用于Qualcomm Adreno GPU，不支持其他GPU的安装。
- 低于Qualcomm Adreno 6xx GPU无可用的GPU驱动。
- 对于Qualcomm Adreno 6xx GPU且Android 10，需要使用[turnip-v12-adpkg](https://github.com/K11MCH1/AdrenoToolsDrivers/releases/download/Turnip_v12/turnip-v12-adpkg.zip)的GPU驱动（该驱动存在易卡死以及闪退问题，无法长时间游玩，建议更新系统版本）。
- 对于Qualcomm Adreno 8xx GPU使用[turnip_a8xx](https://github.com/K11MCH1/AdrenoToolsDrivers/releases/download/v26.0.0-rc08/turnip_a8xx.zip)驱动，处于实验性阶段，不推荐使用该驱动。

## 安装
1. 打开Vita3K，在设置的`图形`选项卡中找到`自定义GPU驱动`，选择`下载驱动`，下载对应您设备的GPU型号的驱动；
2. 在`自定义GPU驱动`中选择`安装驱动`，选择驱动的zip文件；
3. 在`自定义GPU驱动`中将`Default`更换为已安装的新驱动。

## 卸载
1. 打开Vita3K，在设置的`图形`选项卡中找到`自定义GPU驱动`；
2. 在`自定义GPU驱动`中选择`移除已选驱动`。

## 特殊（PC）
针对PC版本，如果出现无法游玩以及闪退的情况，建议在显卡官方网站获取，下载并安装最新版本的显卡驱动，再尝试在Vita3K运行游玩。如果更新显卡驱动至最新版本，但仍低于OpenGL 4.4或Vulkan 1.0，且依旧无法游玩的情况下，请更换PC硬件配置或者新设备。
