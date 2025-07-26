# 存档导入/导出
## 导入（PSVita->Vita3K）
首先需要将您的PSVita安装了HENkaku，才能进行下面的操作。将PSVita的存档导入到Vita3K中，导出存档需要使用PSVita，并配合Savemgr或VitaShell转储解密存档。

转储/提取解密存档（Savemgr）：
1. 在PSVita安装Savemgr、VitaShell；
2. 运行Savemgr；
3. 选择游戏，选择备份，备份到第一个空槽位（存档位置0）；
4. 运行VitaShell;
5. 找到已备份的存档路径`ux0:data/savegame/[TITLE_ID]/SLOT0`；
6. 压缩已备份的解密存档，传至PC/Android，按照下面的导入方式导入存档至Vita3K。

转储/提取解密存档（VitaShell）：
1. 在PSVita安装VitaShell；
2. 运行VitaShell；
3. 找到存档路径`ux0:user/[user_num]/savedata`；
4. 选中要提取[TITLE_ID]的存档，按下△键显示右侧菜单，选择`以解密方式打开`；
5. 文件全选，将解密存档复制到ux0:data；
6. 压缩已转储的解密存档，传至PC/Android，按照下面的导入方式导入存档至Vita3K。

- 注意：Vita3K仅支持读取已解密的存档，无法在Vita3K中直接安装加密/解密存档。不要企图将存档压缩zip在Vita3K安装，它并不会认为是存档，而认为是补丁。

分为两种导入方式：
1. 覆盖，已存在保存的数据覆盖替换当前的存档文件来实现导入存档（根据游戏保存情况，每个游戏存档文件也会有所不同）的方式。
2. 导入，手动修改存档SlotParam_X.bin（X是数字，代表游戏存档槽）文件的数据来实现导入存档的方式。

- Vita3K无法运行Savemgr存档管理器，PSVita存档与Vita3K存档是有区别的。

### 覆盖
在导入存档前你的游戏必须是有存档的，需要使用自己提取的存档或者他人分享的存档，且必须是解密的。

PC
1. 打开Vita3K，右键应用图标选择`打开文件夹`->`保存数据`；
2. 将存档文件覆盖此目录，运行游戏读取存档。

Android
1. 使用原生文件管理器，将存档文件里的文件选择移动或复制；
2. 点击左上的图标开启菜单，选择Vita3K，打开`ux0/user/[user_num]/savedata/[TITLE_ID]`文件夹，将存档文件粘贴到此目录，运行游戏读取存档。

- 注意：并非所有游戏都适用此方式来导入存档，部分游戏需要先生成存档才能使用此方式操作。

### 导入
无需保存任何数据都可以导入，可以使用该脚本（需要安装最新版本的Python）提取为Vita3K使用的存档槽文件，需要使用自己提取的存档或者他人分享的存档，且必须是解密的。

PC
1. 使用[nishinji的split_sdslot](https://github.com/nishinji/split_sdslot)，将PSVita存档中的sdslot.dat与脚本文件处于同一个文件夹；
2. 打开命令提示符，输入`python split_file.py`；
3. 提取的存档槽文件会在output文件夹中；
4. 打开Vita3K，右键应用图标选择`打开文件夹`->`保存数据`；
5. 将提取的存档槽文件以及原存档数据文件（不再需要sce_sys文件夹）放入到此目录，运行游戏读取存档。

Android
1. 使用[nishinji的split_sdslot](https://github.com/nishinji/split_sdslot)，将PSVita存档中的sdslot.dat与脚本文件处于同一个文件夹；
2. 打开命令提示符，输入`python split_file.py`；
3. 提取的存档槽文件会在output文件夹中；
4. 使用原生文件管理器，将提取的存档槽文件以及原存档数据文件（不再需要sce_sys文件夹）选择移动或复制；
5. 点击左上的图标开启文件管理器菜单，选择Vita3K，打开`ux0/user/[user_num]/savedata/[TITLE_ID]`文件夹，将存档文件粘贴到此目录，运行游戏读取存档。

### 手动修改导入（适合高级用户）
无需保存任何数据都可以导入，导入方式会比较麻烦，同时这个方法适用于所有游戏导入，可以使用自己提取的存档或者他人分享的存档，且必须是解密的。需要使用十六进制编辑器（如UltraEdit、WinHex等）。

PC
1. 打开解密的sdslot.dat存档文件找到区间，如0x400-0x740是槽位0位置，0x800-0xB40是槽位1位置，每隔0x400为一个槽位以此类推；
2. 选中此区间的值，粘贴到对应SlotParam_X.bin（X为槽位数，按照槽位生成的存档位置命名和槽位数来命名）值后保存，并按照对应槽位重命名（根据Vita3K log cmd窗口来查看读取存档槽，如0x400-0x740是槽位0 `SlotParam_0.bin`）；
3. 打开Vita3K，右键应用图标选择`打开文件夹`->`保存数据`；
4. 将存档文件放入到此目录，运行游戏读取存档。

Android
1. 打开解密的sdslot.dat存档文件找到区间，如0x400-0x740是槽位0位置，0x800-0xB40是槽位1位置，每隔0x400为一个槽位以此类推；
2. 选中此区间的值，粘贴到对应SlotParam_X.bin（X为槽位数，按照槽位生成的存档位置命名和槽位数来命名）值后保存，并按照对应槽位重命名（根据vita3k.log日志文件来查看读取存档槽，如0x400-0x740是槽位0 `SlotParam_0.bin`）；
3. 使用原生文件管理器，将存档文件里的文件选择移动或复制；
4. 点击左上的图标开启菜单，选择Vita3K，打开`ux0/user/[user_num]/savedata/[TITLE_ID]`文件夹，将存档文件粘贴到此目录，运行游戏读取存档。

## 导出（Vita3K->PSVita）
反向将Vita3K存档导入回到PSVita，这需要一点繁琐操作，并使用VitaShell将解密转为加密存档。

PC
1. 需要在PSVita的当前游玩游戏中新建存档（如果你在Vita3K有多个存档也多创建存档），使用VitaShell准备将Vita3K的存档导入至PSVita；
3. 打开Vita3K，右键应用程序选择`打开文件夹`->`保存数据`，将您要提取的存档文件使用FTP或USB传输到您PSVita的`ux0:data`文件夹内（没有文件夹就建一个）；
4. 在PSVita打开VitaShell，将对应的存档文件按方形键选中，按下△键弹出右侧菜单，选择复制；
5. 打开到`ux0:user/00/savedata`路径，选标到指定的`[Titie_ID]`文件夹，按下△弹出右侧菜单，选择`以解密方式打开`；
6. 将存档文件粘贴到该位置即可，删除所有SlotParam_X.bin文件，关闭VitaShell，运行游戏读取存档。

Android
1. 需要在PSVita的当前游玩游戏中新建存档（如果你在Vita3K有多个存档也多创建存档），使用VitaShell准备将Vita3K的存档导入至PSVita；
2. 使用原生文件管理器，点击左上的图标开启菜单，选择Vita3K，打开`ux0/user/[user_num]/savedata/[TITLE_ID]`文件夹，将您要提取的存档文件至设备目录的Download文件夹下，再使用FTP或USB连接传输到PSVita的`ux0:data`文件夹内（没有文件夹就建一个）；
3. 在PSVita打开VitaShell，将对应的存档文件按方形键选中，按下△键弹出右侧菜单，选择复制；
4. 打开到`ux0:user/00/savedata`路径，选标到指定的`[Titie_ID]`文件夹，按下△弹出右侧菜单，选择`以解密方式打开`；
5. 将存档文件粘贴到该位置即可，删除所有SlotParam_X.bin文件，关闭VitaShell，运行游戏读取存档。
