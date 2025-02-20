# 使用Vita3K
## 打开Vita3K，初次为Vita3K进行初始设置
1. 选择语言，选择完成后点击右下角继续。
2. 选择存放路径（即模拟PSVita的文件路径），更改或保持默认路径都可以点击右下角继续。（Android版本注意的是更改路径需要先授权存储权限才能使用）
3. 在该页面下载[预装固件](http://dus01.psp2.update.playstation.net/update/psp2/image/2022_0209/pre_efd1ef6c1cc2fe92e72e9e783e421237/PSP2UPDAT.PUP)、[固件](http://dus01.psv.update.playstation.net/update/psv/image/2022_0209/rel_f2c7b12fe85496ec88a0391b514d6e3b/PSVUPDAT.PUP)以及[字体固件](http://dus01.psp2.update.playstation.net/update/psp2/image/2022_0209/sd_59dcf059d3328fb67be7e51f8aa33418/PSP2UPDAT.PUP)选项，并选择下面的安装固件文件逐个安装，固件若都已安装则显示V（代表√，已安装），可以点击右下角继续；不安装固件也不影响使用，部分应用程序需要固件模块才能正常运行，但强烈建议还是安装固件。
4. 设置Vita3K基本设置，例如显示样式、信息栏设置，设置完可以点击右下角继续。
5. 初始设置已完成，点击OK就开始使用Vita3K吧。
6. 创建用户，创建完用户后点击你刚才创建的用户图标继续操作。
7. [该步骤仅适用PC，切勿在Android启用] 进入到锁屏界面点击任意地方进入到Vita3K的Livearea主页面，选择顶部选项栏的`配置`->`设置`选项，点击`GUI`勾选`亚洲区域`选项，点击保存并重启Vita3K模拟器以显示正常文字。

## 固件安装
### 预装固件、固件安装步骤（若已安装可跳过此操作）
- 在Vita3K模拟器安装任意版本的固件都不会因为系统版本而受到限制。

1. 点顶部主菜单栏的`文件`；
2. 选择`安装固件`；
3. 选择PUP文件；
4. 安装完固件后可以继续选择安装字体固件，或者重启模拟器即可。

### 字体固件安装步骤（若已安装可跳过此操作）
1. 点顶部主菜单栏的`文件`；
2. 选择`安装固件`；
3. 选择PUP文件；
4. 安装完固件后点顶部菜单栏`配置`->`设置`选项；
5. 打开`设置`对话框后点`图形用户界面`选项，点击勾选`亚洲区域`选项，点击保存并重启模拟器以显示正常文字。

- ⚠️注意：安卓版本安装固件后千万不要勾选亚洲区域字体支持，否则不显示文字。

## 设置完成Vita3K相关教程
此流程安装完就可以进行安装应用程序/游戏、补丁更新、追加内容DLC和主题。
- [追加内容DLC安装](http://croden1999.github.io/Vita3K-Quick-Guide/vita3k/addcont)
- [应用程序/游戏安装](http://croden1999.github.io/Vita3K-Quick-Guide/vita3k/app)
- [更新补丁安装](http://croden1999.github.io/Vita3K-Quick-Guide/vita3k/patch)
- [主题安装](http://croden1999.github.io/Vita3K-Quick-Guide/vita3k/theme)

## Vita3K界面介绍
### 用户管理
进行创建、编辑、删除用户、名称、头像选择更换的操作，类似于PS4界面。初次使用会显示欢迎对话框，可以取消勾选`下次显示`，以后打开Vita3K不再弹出此对话框。另外如果不想反复登入同一个用户，可以勾选自动登入此用户，以后将该用户作为默认登入用户。

### 系统应用程序
- 互联网浏览器 [NPXS10003]：访问Vita3K官网
- Trophy（奖杯）收藏 [NPXS10008]：管理获得的游戏奖杯信息
- 设定 [NPXS10015]：管理主题&背景、日期&时间、语言以及语言键盘的设置
- 内容管理 [NPXS10026]：管理应用程序、存档以及主题

### Livearea页面
菜单栏选项：
- 文件：打开存放路径、打开纹理文件夹、安装固件/pkg/zip/vpk/授权、退出
- 模拟：最近使用的应用程序（至多显示8个）、系统应用程序（仅在禁用系统应用程序时显示）
- Debug（仅适用于开发人员）：线程、信号量、互斥锁、轻量互斥锁、条件变量、轻量条件变量、事件标志、内存分配、反汇编
- 配置：设置、用户管理
- 控制：[仅Android版本显示] 虚拟按键、[仅PC版本显示] 键盘控制、控制器
- 帮助：关于、[Android不存在] Vita3K更新、欢迎

筛选，通过筛选显示的应用程序：
- 所有
- 按地区：美版、欧版、日版、亚版
- 按类型：商业、自制
- 按兼容性状态：全部、未知、无法启动、可引导、有图像、可进入菜单、可进入游戏-、可进入游戏+、可玩

1. 列表模式：
- 兼容性：以应用程序的兼容性状态排序
- 标题ID：以应用程序的标题ID排序
- 版本：以应用程序的版本排序
- 类别（gd：游戏数据、gp：游戏补丁、gda：系统应用）：以应用程序的类别排序
- 最近使用时间：以应用程序的最近使用时间排序
- 标题：以应用程序的标题名称排序
- 刷新：刷新应用程序图标

2. 网格模式（配置设置对话框中启用网格模式）：
- 应用程序排序按：版本/类别/兼容性/最近使用时间/标题/标题ID
- 刷新：刷新应用程序图标

应用程序右键选项：
- 开始/继续
- 兼容性（兼容性状态、兼容性状态日期、复制Vita3K摘要、打开状态报告、更新数据库）
- 复制应用程序信息（名称和标题ID、名称、标题ID、应用程序摘要）
- 自定义配置（单独应用程序的配置设置，不影响整体配置设置；GPU的后端渲染器、内存映射方案以及PSTV模式有影响）
- [仅Android版本显示，部分设备可能有效/没有效果] 创建快捷方式
- [Android不存在] 打开文件夹（应用程序、追加内容、授权、保存数据、着色器缓存、着色器日志、导入纹理、导出纹理）
- 删除（应用程序、追加内容、授权、保存数据、着色器缓存、着色器日志、导入纹理、导出纹理）
- [仅在禁用Live Area应用屏幕显示] Live Area（Live Area、搜索、说明书、升级）
- 更新历史记录
- 信息

### 配置设置选项
核心：

⚠️注意：安装系统固件后才会显示模块列表，一部分游戏需要固件中的模块才能正常运行。

- 模块模式：Automatic（自动选择）、Auto&Manual（自动&手动并用，也可以手动选择模块）和Manual（手动选择），强烈推荐使用自动或者自动&手动并用模块模式，默认为Automatic。
- 模块列表：仅Auto&Manual以及Manual能手动选择模块加载，可以在搜索模块查找你需要的模块，选择模块后显示为黄色（表示在应用程序中会调用该模块）。若想清除所有手动加载的模块可以点清除列表）恢复。
- 清除列表
- 刷新列表

CPU：
- CPU后端：可切换Dynarmic/Unicorn（已弃用），默认为Dynarmic，Android不存在Unicorn
- [仅Dynarmic显示] 启用优化：启用额外CPU的JIT优化

GPU：
- 后端渲染器：可切换OpenGL/Vulkan，Windows & Linux默认为OpenGL，macOS & Android默认为Vulkan，更改后需要重启Vita3K才能生效。另外需要检查显卡是否支持Vulkan，若显卡不支持Vulkan打开Vita3K则可能会闪退/报错，在config.yml将Vulkan更改为OpenGL保存就能正常运行Vita3K（macOS则忽略此设置，因为OpenGL不存在）
- [此选项仅在Vulkan时显示] GPU/驱动程序，更改为Vulkan后可以自动或者手动选择GPU显卡/驱动程序，更改后需要重启Vita3K才能生效
- [仅Android版本且Qualcomm Snapdragon SoC时显示] 添加自定义驱动
- [仅Android版本且Qualcomm Snapdragon SoC时显示] 移除自定义驱动
- 渲染器精度：可切换标准/高，PC默认为高，Android默认为标准
- [仅OpenGL时显示] 垂直同步
- 禁用表面同步：禁用表面同步可以提升速度，某些游戏需要表面同步才能正确显示图形，默认启用
- 异步管线编译：允许管线多个线程同时编译，并减少编译过程中的卡顿情况，代价则是有短暂图形错误的故障，默认启用
- 屏幕过滤：OpenGL下可切换双线性/FXAA，Vulkan下可切换最邻近/双线性/双三次/FXAA/FSR（需要GPU支持），OpenGL/Vulkan都默认为双线性
- 提升分辨率（1x - 8x），选择重置会回调到1x（即960x544）分辨率
- 各向异性过滤（1x - 16x），选择重置会回调到1x
- 导出纹理
- 导入纹理
- 纹理导出格式：PNG/DDS，默认为PNG，支持png、未压缩纹理、BCn压缩纹理（PC支持，但在Android仅限高通骁龙soc）、ASTC压缩纹理
- 使用着色器缓存
- [此选项仅在OpenGL时且显卡支持下显示，Android不存在] 使用Spir-V着色器（已弃用）
- 清除着色器缓存和着色器日志
- FPS修改：可以使30FPS的应用程序/游戏提升至60FPS，但并非所有应用程序/游戏都有效果，有的正常，有的两倍速，还有的开启没有效果，默认禁用
- [仅Android版本显示] 内存映射方式：可切换禁用/双缓冲/页表/本机缓冲的设置，切换后需要重启才能生效默认双缓冲
- [仅Android版本且Qualcomm Adreno GPU显示] 启用睿频模式：提供了一种方法来强制GPU运行在最大合理的频率（温控仍然适用）

音频：
- 音频后端：可切换SDL/Cubeb，默认SDL
- 全局百分比音量：可设置在Vita3K中的百分比音量，它会影响所有应用程序/游戏，默认100%
- 启用NGS支持，默认启用，取消勾选则禁用应用程序/游戏的音频

系统：
- 可切换O/X键为确认按键，默认X键
- 模拟PSTV模式
- 模拟Show（展示）模式
- 模拟Demo（演示）模式

模拟器：
- [Android版本不存在该项，本身就是全屏] 运行应用程序时全屏
- 日志级别：可切换追踪/Debug/信息/警告/错误/关键/关闭，PC默认追踪，Android默认关闭
- 档案日志
- Discord Rich Presence（可以在Discord显示你正在游玩Vita3K的状态，Android版本不存在此选项）
- 纹理缓存
- 显示编译着色器：显示编译着色器弹窗，取消勾选则不显示
- 显示触摸板光标：显示PS4/5手柄的触摸板光标，取消勾选则不显示
- 日志兼容性警告：在日志窗口中显示兼容性的警告，默认禁用
- 检查更新：启动Vita3K时自动检查新版本更新，默认启用
- 性能图层：显示FPS
- [启用性能图层时显示] 细节：可切换最低/低/中/最高的细节显示
- [启用性能图层时显示] 位置：可切换左上/中上/右上/左下/中下/右下的位置显示
- [Windows不显示] 检查在区分大小写的文件系统上启用不区分大小写的路径查找。 重启时重置（允许模拟器尝试在非windows平台上搜索文件，无论大小写）
- 模拟器系统存储文件夹路径（即模拟PSVita分区的路径）（Android版本注意的是更改路径需要先授权存储权限才能使用） 
- 自定义配置设置（清除所有自定义配置设置）

图形用户界面：
- 图形用户界面可见：运行应用程序中显示顶部选项栏
- 信息栏可见：勾选则显示类似于PSVita样式的信息栏，取消勾选则显示顶部选项栏
- 图形用户界面语言：可以选择系统语言或者用户自定义语言
- 显示信息消息：显示兼容性状态弹窗，取消勾选则只在日志中显示信息消息
- 显示系统应用程序：在主页面中显示系统应用程序，取消勾选则仅在菜单栏中显示
- Livearea应用程序界面：显示应用程序背景图片、图标、说明书的界面，取消勾选该选项点应用程序图标会直接运行
- 拉伸显示区域：扩大显示区域以适应屏幕尺寸
- 网格模式：应用程序图标由列表变更为网格显示
- 字体支持：亚洲地区（启用后重启Vita3K能正常显示文字，安卓版本千万不要开启此项）
- 主题&背景：还原默认主题、使用主题背景、背景透明度、延时背景切换、延时锁屏

网络：
- 已登入PSN：勾选此项，游戏将认为用户已连接至PSN（但为离线状态）
- 启用HTTP：勾选此选项启用游戏在网络中使用HTTP协议。（一些游戏需要HTTP才能运行）
- HTTP超时尝试：当服务器没有响应时，要进行多次尝试。如果您有非常不稳定或是极慢的网络可能是有用的
- HTTP超时休眠：当服务器没有响应时，尝试休眠时间。如果您有非常不稳定或是极慢的网络可能是有用的
- HTTP读取终止尝试：当没有更多数据可读取时，尝试多次可以提升性能，但如果您的网络很糟糕，则会导致游戏不稳定
- HTTP读取终止休眠：尝试在没有更多数据可读取时进入休眠时间，这可以提高性能，但如果您的网络很糟糕，则会导致游戏不稳定

Debug（仅适用于开发人员）：
- 记录导入
- 记录导出
- 着色器记录
- 统一记录
- 保存颜色表面
- ELF提取
- 验证层：启用Vulkan验证层。
- 监视/取消监视代码
- 监视/取消监视内存
- 监视/取消监视导入调用
- [仅debug版本显示] Tracy（追踪）分析器

### [仅Android显示] Overlay 虚拟按键
- Show gamepad overlay ingame：在游戏中显示手柄虚拟按键
- Modify Gamepad Overlay：修改手柄虚拟按键
- Hide Gamepad Overlay：隐藏手柄虚拟按键
- Overlay scale：虚拟按键缩放
- Overlay opacity：虚拟按键不透明度
- Reset Gamepad：重置手柄布局
- Show front/back touchscreen switch button：显示前/后触屏切换按键
- L2/R2 triggers will be displayed only if PSTV mode is enabled：仅当启用PSTV模式时，才会显示L2/R2键
