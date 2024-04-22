# 转储提取

首先需要将您的PSVita安装了HENkaku，才能进行下面的操作。

## 提取应用/游戏、更新补丁
### 使用nonpdrm提取
1. 确保在PSVita已安装了VitaShell以及nonpdrm插件；
2. 在PS Store下载您已购买拥有的app/游戏；
3. 安装完成后在PSVita运行app/游戏（如果有更新，请更新后再运行）；
4. 然后退出游戏，运行VitaShell；
5. 找到app路径`ux0:app`以及更新补丁路径`ux0:patch`；
6. 选中要提取[TITLE_ID]的游戏以及更新补丁文件夹，并分别复制到`ux0:data/app`、`ux0:data/patch`（需要新建文件夹）；
7. 找到nonpdrm授权路径`ux0:nonpdrm/license/app/[TITLE_ID]`，将rif文件重命名为work.bin，移动覆盖至`ux0:data/app/[TITLE_ID]/sce_sys/package`文件夹，使用nonpdrm生成的授权替换掉PSN官方授权；
8. 打包压缩`ux0:data`中的`app`以及`patch`文件夹为zip，命名为[TITLE_ID].zip，压缩级别不限；
9. 将已压缩的zip传至PC/Android安装。

### 使用maidumptool提取
1. 确保在PSVita已安装了VitaShell、maidumptool以及nonpdrm插件；
2. 在PS Store下载您已购买拥有的app/游戏；
3. 安装完成后在PSVita运行app/游戏（如果有更新，请更新后再运行）；
4. 运行maidumptool；
5. 提取完整游戏本体以及更新补丁；
6. 完成后运行VitaShell；
7. 找到mai路径`ux0:mai`；
8. 打包压缩`ux0:mai`中的`[TITLE_ID]`以及`[TITLE_ID]_patch`文件夹为zip，命名为[TITLE_ID].zip，压缩级别不限；
9. 将已压缩的zip传至PC/Android安装。

### 使用FAGDec提取
1. 确保在PSVita已安装了VitaShell、FAGDec以及nonpdrm插件；
2. 在PS Store下载您已购买拥有的app/游戏；
3. 安装完成后在PSVita运行app/游戏（如果有更新，请更新后再运行）；
4. 运行VitaShell；
5. 找到app路径`ux0:app`以及更新补丁路径`ux0:patch`；
6. 选中要提取[TITLE_ID]的游戏以及更新补丁，按下△键显示右侧菜单，选择`以解密方式打开`；
7. 文件全选，将全部文件复制到ux0:data/[TITLE_ID]（需要新建文件夹），依次先app再patch，文件覆盖；
8. 运行FAGDec；
9. 并向下滚动，直到找到想要提取的游戏；
10. 将光标悬停在游戏上并按下按钮，等待FAGDec找到所有模块，然后选择`DECRYPT ALL（解密全部）`
11. 您将看到模块已列在屏幕右侧。现在返回主菜单并按Start键；
12. 您将在此处看到两个选项，选择`[START] START DECRYPT(SELF)`；
13. 现在只需等到它完成对游戏模块的解密；
14. 您可以在以下位置找到输出文件`ux0:FAGDec/app/[TITLE_ID]`；
15. 将`ux0:FAGDec/app/[TITLE_ID]`里的所有文件移动覆盖至`ux0:data/[TITLE_ID]`，压缩`ux0:data/[TITLE_ID]`的文件为zip，命名为[TITLE_ID].zip/vpk，压缩级别不限；
16. 将已压缩的zip/vpk传至PC/Android安装。

## 追加内容DLC
### 使用maidumptool提取
1. 确保在PSVita已安装了VitaShell、maidumptool以及nonpdrm插件；
2. 在PS Store下载您已购买拥有的追加内容DLC；
3. 运行maidumptool；
4. 提取所有追加内容DLC；
5. 完成后运行VitaShell；
6. 找到mai路径`ux0:mai`；
7. 打包压缩`ux0:mai`中的`[TITLE_ID]_addc`文件夹为zip，命名为`[TITLE_ID]_DLC.zip`，压缩级别不限；
8. 将已压缩的zip传至PC/Android安装。

## 相关的安装教程
- [追加内容DLC安装](http://croden1999.github.io/Vita3K-Quick-Guide/vita3k/addcont)
- [应用程序/游戏安装](http://croden1999.github.io/Vita3K-Quick-Guide/vita3k/app)
- [更新补丁安装](http://croden1999.github.io/Vita3K-Quick-Guide/psvita-to-vita3k/patch)
