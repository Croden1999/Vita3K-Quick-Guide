# Vita3K使用教程
首次使用Vita3K前，请不要放在带有中文文件夹里，否则打开Vita3K会闪退。

## 打开Vita3K，首次为您的Vita3K初始设置
1. 选择语言，选择好语言后点Next继续。
2. 选择存放路径（即模拟PSVita的文件路径），修改或不修改路径都可以点击Next继续。
3. 下载一般固件和字体固件选项，并选择下面的Install Firmware安装固件，两个固件都已安装且显示 V 就可以点Next继续；不安装固件也不影响使用，但还是建议安装固件。
4. 设置Vita3K基本设置，例如显示样式、信息栏设置，设置后可以点Next继续。
5. 初始设置完成，点击OK就开始使用Vita3K吧。
6. 创建用户，创建完用户后点击你刚才创建的用户图标继续操作。
7. 进入到锁屏界面再次点击任何地方进入到Vita3K的Livearea主页面，选择顶部选项栏的配置->设置选项，点击GUI勾选Asia Region选项，重启Vita3K模拟器以显示正常文字。

## 系统固件安装流程（若已安装可忽略此步骤）
在Vita3K模拟器安装任意版本的系统固件都不会因为系统版本而受到限制。
1. 打开Vita3K；
2. 点击顶部选项栏的 Files（文件） 选项；
3. 选择 Install Firmware（安装系统固件） 选项；
4. 选择PUP文件；
5. 安装完固件后可以继续选择安装字体固件，或者确认即可。

## 字体固件安装流程（若已安装可忽略此步骤）
1. 打开Vita3K；
2. 点击顶部选项栏的 Files（文件） 选项；
3. 选择 Install Firmware（安装系统固件） 选项；
4. 选择PUP文件；
5. 安装完固件后点击顶部选项栏Configuration（配置）选项；
6. 点击Settings（设置）选项；
7. 点击GUI选项；
8. 勾选Asia Region选项后重启模拟器即可。

## 设置完成Vita3K后的其他教程
此流程安装完就可以进行安装游戏、DLC和主题，你还可以按F11显示全屏。

[->游戏安装教程](http://croden1999.github.io/Vita3K-quick-guide/README_game)

[->DLC追加内容安装教程](http://croden1999.github.io/Vita3K-quick-guide/README_dlc)

[->主题安装教程](http://croden1999.github.io/Vita3K-quick-guide/README_theme)

## Vita3K切换语言
在Vita3K的Livearea主页面中选择 【NPXS10015】 设定 应用程序，选择Language语言->System Language系统语言来切换语言。
- Chinese - Simplified —— 简体中文
- Chinese - Traditional —— 繁体中文

![](https://user-images.githubusercontent.com/61804715/131735493-7b80ae2e-dfe0-4d83-bcc8-454fb5d0873d.png)


## Vita3K界面介绍
![](https://user-images.githubusercontent.com/61804715/131706598-114cd931-e30c-4da3-a1cd-17270b749aee.png)

用户管理：
- 新建、编辑、删除用户、名称、头像更换的操作

Livearea主页面选项：
1. 列表模式（未勾选Grid Mode）：
- Filter：筛选显示应用程序
- Title ID：应用程序ID
- Ver：应用程序版本
- Cat：类型（gd：游戏数据、gp：游戏补丁、gda：系统应用）
- Last Time：最近游玩的时间
- Title：应用程序名称
- Refresh：刷新应用程序
2. 网格模式（勾选Grid Mode）：
- Filter：筛选显示应用程序
- Sort App By：选择对于类型的应用程序排序，如：按应用程序版本、类型、最近游玩的时间、应用程序名称或者应用程序ID来排序
- Refresh：刷新应用程序

Filter（筛选）选项：
- 所有
- 按地区：USA（美版）、Europe（欧版）、Japan（日版）、Asia（亚版）
- 按类型：Commercial（商业）、Homebrew（自制）

应用程序右键选项：
- Boot：运行
- Check APP Compatibility：检查应用程序兼容性
- Copy APP Info：复制应用程序信息
- Custom Config：自定义配置
- Open Folder：打开文件夹
- Delete：删除
- Update History：更新历史记录
- Information：信息

菜单栏选项：
- 文件：打开存放路径、安装系统固件、pkg、zip、vpk和授权文件
- 模拟器：最近使用的应用
- Debug（调试选项）
- 配置：设置、用户管理
- 控制：键盘按键映射、手柄控制器
- 帮助：关于、欢迎界面

## 配置设置选项介绍
Core 核心：
- Modules Mode（模块模式）：启用实验性功能模块，自动选择、自动手动并用或者手动选择模块
- Modules List（模块列表）：Automatic（自动选择）、Auto&Manual（自动&手动并用，也可以手动选择模块）和Manual（手动选择）

CPU 处理器:
- CPU后端：Dynarmic或者Unicorn，仅Dynarmic的CPU后端才能启用JIT选项

GPU 显卡：
- 使用着色器缓存
- 使用Spir-V着色器（不是所有显卡都有这个选项，取决于显卡的支持）

System 系统：
- 切换O / X键为确认键
- 模拟PSVTV / PSTV模式

Emulator 模拟器：
- 禁用at9音频解码器
- 禁用支持实验性ngs
- 启用支持视频播放
- 日志等级
- 归档日志
- 不和谐丰富的存在
- 性能叠加（显示FPS帧数、平均以及最高帧、帧数线性流动图、调整显示位置）
- 纹理缓存
- 模拟器系统存储文件夹路径（即模拟PSVita分区的路径）

GUI 界面：
- 界面可见：运行应用程序中显示菜单栏
- 显示应用程序的Livearea界面：显示应用程序背景图片、图标、说明书的界面，取消勾选该选项运行应用程序会直接运行
- 网格模式：应用程序图标由列表变为网格显示
- 字体支持：亚洲地区（启用能显示正常文字）
- 主题&背景：还原默认主题、使用主题背景、背景透明度、延时背景切换、延时锁屏的操作

Debug 调试（非开发人员建议忽略此项）：
- 日志导入
- 日志导出
- 着色器日志
- 统一日志
- 保存表面颜色
- 提取纹理
- 提取elfs
- 浏览代码
- 浏览内存
- 浏览导入调用
