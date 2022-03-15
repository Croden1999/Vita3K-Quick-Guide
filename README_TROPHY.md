# 奖杯修改教程
每个游戏奖杯（除同游戏不同区域）不同，在修改之前你需要知道游戏对应的奖杯ID（例如：PCSH00250死或生沙滩排球3对应奖杯ID是NPWR10022_00），在TROPUSR.DAT文件中使用十六进制编辑器浏览编辑，奖杯开头在区间第一行04项的第一个字符，修改奖杯基本是3、F这两个字符。

![1](https://user-images.githubusercontent.com/61804715/145160207-230fcf68-45cd-49c8-b6c4-2f3089d1b2d6.jpg)

（如果你没有PSV可以忽略这一步，这个步骤是浏览奖杯位置）你可以参考在你的PSV用VitaShell，到这个ur0:user/00/trophy/data文件夹里知道并找到游戏对应的奖杯ID，按△键菜单中选择解密方式打开，打开TRPTILTE.DAT文件，按△键菜单中选择16进制编辑器，在0x000006C0地址就可以找到，在Vita3K上的奖杯文件修改完保存，重新打开Vita3K模拟器在奖杯应用程序浏览效果。

![2](https://user-images.githubusercontent.com/61804715/145160284-b0ecb5aa-5ae0-4186-a6e2-d504f51ca060.jpg)
![3](https://user-images.githubusercontent.com/61804715/145160375-37c8d3b7-92d1-437e-a578-90445a2ddb88.jpg)

- 不过缺点是修改后的奖杯显示日期是1970/1/1，未来我会继续研究修改奖杯时间的问题。

## 演示
1. 秋之回忆8
![4](https://user-images.githubusercontent.com/61804715/134748321-568ba06a-d757-477b-8595-24148ed9d112.png)
![5](https://user-images.githubusercontent.com/61804715/134748436-38d512ff-9d3d-48fe-afed-1d16963c48c2.png)

2. 重力异想世界
- Before（未修改前）
![6](https://user-images.githubusercontent.com/61804715/134748607-ee706c7c-424a-4a8e-846e-2b5e46c98b11.png)
![7](https://user-images.githubusercontent.com/61804715/134748317-9c5af35b-976c-48ac-a35a-008f0831fb0d.png)

- After（修改后）
![8](https://user-images.githubusercontent.com/61804715/134748631-b9d876a7-3346-44c3-b1a3-76da23f9193e.png)
![9](https://user-images.githubusercontent.com/61804715/134748613-b7017b81-b783-4935-969d-25ace6a893fc.png)
