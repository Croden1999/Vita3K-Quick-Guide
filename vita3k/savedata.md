# 存档导入
## 导入
将PSVita的存档导入到Vita3K中，两种导入方式都不需要PSVita，但需要解密的PSVita存档文件，Vita3K只读取解密的文件。
- 注意：仅支持解密的存档转换，无法在Vita3K中直接安装加密/解密存档。不要企图将存档压缩zip在Vita3K安装，它并不会认为是存档，而认为是补丁。

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
4. 使用原生文件管理器，将提取的存档槽文件以及原存档数据文件（不再需要sce_sys文件夹），选择复制；
5. 点击左上的图标开启文件管理器菜单，选择Vita3K，打开`ux0/user/[user_num]/savedata/[TITLE_ID]`文件夹，将存档文件粘贴到此目录，运行游戏读取存档。

### 手动修改导入（适合高级用户）
无需保存任何数据都可以导入，导入方式会比较麻烦，同时这个方法适用于所有游戏导入，可以使用自己提取的存档或者他人分享的存档，且必须是解密的。需要使用十六进制编辑器（如UltraEdit、WinHex等）。

PC
1. 打开解密的sdslot.dat存档文件找到区间，如0x400-0x740区间是槽位0位置；
2. 选中此区间的值，粘贴到对应SlotParam_X.bin（X为槽位数，按照槽位生成的存档位置命名和槽位数来命名）值后保存，并按照对应槽位重命名（根据Vita3K log cmd窗口来查看读取存档槽，如0x400-0x740是槽位0 `SlotParam_0.bin`）；
3. 打开Vita3K，右键应用图标选择`打开文件夹`->`保存数据`；
4. 将存档文件放入到此目录，运行游戏读取存档。

Android
1. 打开解密的sdslot.dat存档文件找到区间，如0x400-0x740区间是槽位0位置；
2. 选中此区间的值，粘贴到对应SlotParam_X.bin（X为槽位数，按照槽位生成的存档位置命名和槽位数来命名）值后保存，并按照对应槽位重命名（根据vita3k.log日志文件来查看读取存档槽，如0x400-0x740是槽位0 `SlotParam_0.bin`）；
3. 使用原生文件管理器，将存档文件里的文件复制；
4. 点击左上的图标开启菜单，选择Vita3K，打开`ux0/user/[user_num]/savedata/[TITLE_ID]`文件夹，将存档文件粘贴到此目录，运行游戏读取存档。
