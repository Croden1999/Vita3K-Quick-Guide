# 60FPS补丁
基于[Vita3K Patches Wiki](https://github.com/Vita3K/Vita3K/wiki/Patches)翻译，由SpikeHD编写。

Vita3K补丁系统专为“60FPS”补丁设计，类似于它灵感来源的工具[VitaGrafix](https://github.com/Vita3K/Vita3K/wiki/Patches)。

# 使用补丁
> ⚠ 警告
> 
> 该系统与VitaGrafix补丁不完全兼容......至少现在还没有。你需要使用Vita3K专用的补丁。

在Vita3K文件夹中，有两个地方可以添加补丁代码：`patch`

1. 一个包含游戏标题ID的文件。它还可以包含多个标题ID，也可以包含任意文本（例如：`.txt` `PCS0000_60FPS.txt`)
2. 全局文件`patchlist.txt`

## 使用游戏专用文件
在游戏专用补丁文件中，你可以直接粘贴补丁代码，不做其他内容：

```0:0xFFFF 0x01```

或者指定要应用补丁的二进制：

```
[my_game.self]
0:0xFFFF 0x01
```

## 使用`patchlist.txt`文件
在这个文件中，你可以在头部指定标题ID和二进制：`patchlist.txt`

```
[PCSE00999, eboot.bin]
0:0xFFF 0x01
```

默认情况下，二进制是可选的：`eboot.bin`

```
[PCSE00999]
0:0xFFF 0x01
```

# 编写补丁
找到需要修补的内容需要逆向工程和技术知识。这里有一份为VitaGrafix编写的好指南：[https://wp.yuki.pet/make-your-own-patch-for-vitagrafix/](https://wp.yuki.pet/make-your-own-patch-for-vitagrafix/)（[archive.org](https://web.archive.org/web/20260113022855/https://wp.yuki.pet/make-your-own-patch-for-vitagrafix/)，[archive.ph](https://archive.ph/JMyNw))

原则相同，不过Vita3K提供的格式和辅助工具略有不同。

# 格式
补丁的头部格式如下：
```
[TITLE_ID, 二进制文件]
```

补丁的分段格式如下：
```
# 也支持评论
# <byte>也可以是一个辅助调用，比如t1_mov(0, 1)
<seg>:<offset> <hex1> <hex2> <...hexN>
```

需要帮助吗？看看下面的示例。

## 辅助
像VitaGrafix一样，你可以用辅助工具代替写原始16进制值，比如你可以在[`instructions.h`的头文件](https://github.com/Vita3K/Vita3K/blob/master/vita3k/patch/include/patch/instructions.h)中找到所有可用的辅助工具。`t1_mov()`

## 示例
用于测试该系统实现的补丁是 初音未来歌姬计划F2 的60帧补丁，它是从这个[VitaGrafix的PR](https://github.com/Electry/VitaGrafixPatchlist/pull/136)修改而来。

```
# 60 FPS
# 这个"eboot.bin"头是可选的，因为如果未指定，则默认使用"eboot.bin"
[PCSB00554, eboot.bin]
0:0xA994 t1_mov(0, 1)
0:0xAAF2 0xF7EE000A
0:0x2896F6 0xDCF88083
0:0x2896FE 0xDCF88493
0:0x2849b4 0x2022
```
