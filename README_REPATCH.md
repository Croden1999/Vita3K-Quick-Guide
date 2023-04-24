# 语言/Mod补丁包与安装
## 前言
关于语言、Mod补丁您需要从各大网站、论坛社区获取由作者、汉化组团队等其他人员分享的内容，我在这里只按照区分是repatch补丁或者是readdcont追加内容DLC打包安装的简单步骤。

需要准备原游戏的eboot.bin（仅解密，可在Vita3K安装游戏后提取）以及sce_sys\param.sfo文件，打包安装步骤需要这些文件才能在Vita3K中识别并安装。另外，重新打包的文件也可以分享给其他玩家用户在Vita3K中安装。

## Language/Mods Patch(repatch)
### 如果是以repatch补丁的形式，如图所示

![image](https://user-images.githubusercontent.com/61804715/232274681-1fc62599-9754-4189-afea-35d99aac9191.png)

### 那么则需要补充原游戏的eboot.bin以及sce_sys\param.sfo文件，将param.sfo内的类别更改为gp（若原来是gp就无需更改）；另外如果语言补丁有附带eboot.bin文件则优先使用语言补丁内的，只需补充原游戏的sce_sys\param.sfo文件，更改类别，之后重新打包压缩zip，如图所示

![image](https://user-images.githubusercontent.com/61804715/232275180-05309ae9-0023-41a3-b99c-7f957159f6e9.png)

### 在Vita3K安装重新打包好的补丁zip压缩包，再进游戏检查效果

![image](https://user-images.githubusercontent.com/61804715/232276065-dd86fa2d-3bdc-4dd2-95c1-4c624a2483da.png)
![image](https://user-images.githubusercontent.com/61804715/232276277-3d38169d-2215-427f-90f1-56f69f0b8b0b.png)
![image](https://user-images.githubusercontent.com/61804715/232276346-ff1ab7e8-27c1-4cd7-80cc-55f350bd3367.png)

## Mods Patch(readdcont)
### 如果是以readdcont补丁的形式，如图所示

![image](https://user-images.githubusercontent.com/61804715/232277589-ac783f26-9c2d-4d00-b9f3-9a372b89c3b7.png)

### [如果不存在param.sfo]若检查不存在sce_sys\param.sfo情况下，首先需要提取原追加内存DLC的sce_sys\param.sfo，放到Mod补丁DLC中，并重新将所有Mod DLC打包压缩zip，如图所示

![image](https://user-images.githubusercontent.com/61804715/232277205-386cd730-a783-46c1-b6f9-36a617e8bb72.png)
![image](https://user-images.githubusercontent.com/61804715/232277543-6f638200-ff7a-41a8-8612-b75adea94604.png)

### 在Vita3K安装重新打包好的Mod DLC补丁zip压缩包，再进游戏检查效果，也可以在Vita3K内容管理查看应用程序已安装追加内容DLC

![image](https://user-images.githubusercontent.com/61804715/232277620-f5524452-368d-4d4e-8ef1-b367d9fc453b.png)
