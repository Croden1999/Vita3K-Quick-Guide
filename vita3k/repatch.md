# RePatch（语言/Mod等）补丁安装
## 前言
关于语言、Mod补丁您需要从各大网站、论坛社区获取由作者、汉化组团队等其他人员分享提供的内容，另外需要检查repatch补丁或是readdcont追加内容DLC，以便于使用下面的步骤进行安装。

repatch/readdcont安装的两种方式：
- 解压（推荐，通常使用频率多）
- 打包安装（需要准备原始游戏的sce_sys/param.sfo文件，打包安装步骤需此文件才能在Vita3K中识别并安装）

## repatch（语言/Mod补丁）
### 解压覆盖（通常）
PC 
1. 打开Vita3K，选择游戏右键打开菜单，选择打开应用程序文件夹；
2. 将repatch补丁解压至当前游戏的文件夹内，并检查文件名称一致覆盖文件；
3. 运行游戏检查补丁加载，直至生效即可。

Android
1. 打开原生文件管理器，将repatch补丁解压，进入repatch文件夹内选中标题ID文件夹复制；
2. 打开侧边栏，选择Vita3K，将已复制的文件夹放置在存放路径的`ux0\app`中，并检查文件名称一致覆盖文件；
3. 运行游戏检查补丁加载，直至生效即可。


### 打包安装 （进阶）
如果是以repatch补丁的形式，如图所示

![image](https://user-images.githubusercontent.com/61804715/232274681-1fc62599-9754-4189-afea-35d99aac9191.png)

那么则需要补充原游戏的sce_sys/param.sfo文件，将param.sfo内的类别更改为gp（若原来是gp就无需更改），需要使用十六进制编辑器修改保存（如Winhex等），修改后如图所示

![image](https://user-images.githubusercontent.com/61804715/232275180-05309ae9-0023-41a3-b99c-7f957159f6e9.png)

在Vita3K安装重新打包好的补丁zip压缩包，再进游戏检查效果

![image](https://user-images.githubusercontent.com/61804715/232276065-dd86fa2d-3bdc-4dd2-95c1-4c624a2483da.png)
![image](https://user-images.githubusercontent.com/61804715/232276277-3d38169d-2215-427f-90f1-56f69f0b8b0b.png)
![image](https://user-images.githubusercontent.com/61804715/232276346-ff1ab7e8-27c1-4cd7-80cc-55f350bd3367.png)

## readdcont（DLC Mod补丁）
### 解压（通常）
PC
1. 打开Vita3K，选择游戏右键打开菜单，选择打开DLC文件夹；
2. 将readdcont补丁解压至当前游戏的DLC文件夹内，如果有重复的DLC可覆盖；
3. 运行游戏检查，直至生效即可。

Android
1. 打开原生文件管理器，将readdcont补丁解压，进入readdcont文件夹内选中标题ID文件夹复制，
2. 打开侧边栏，选择Vita3K，将已复制的文件夹放置在存放路径的`ux0\addcont`中，如果有重复的DLC可覆盖；
3. 运行游戏检查，直至生效即可。

### 打包安装（进阶）
如果是以readdcont补丁的形式，如图所示

![image](https://user-images.githubusercontent.com/61804715/232277589-ac783f26-9c2d-4d00-b9f3-9a372b89c3b7.png)

[如果不存在param.sfo]若检查不存在sce_sys\param.sfo情况下，首先需要提取原始追加内存DLC的sce_sys/param.sfo，放到Mod补丁DLC中，并重新将所有Mod DLC打包压缩zip，如图所示

![image](https://user-images.githubusercontent.com/61804715/232277205-386cd730-a783-46c1-b6f9-36a617e8bb72.png)
![image](https://user-images.githubusercontent.com/61804715/232277543-6f638200-ff7a-41a8-8612-b75adea94604.png)

在Vita3K安装重新打包好的Mod DLC补丁zip压缩包，再进游戏检查效果，也可以在Vita3K内容管理查看应用程序已安装追加内容DLC

![image](https://user-images.githubusercontent.com/61804715/232277620-f5524452-368d-4d4e-8ef1-b367d9fc453b.png)
