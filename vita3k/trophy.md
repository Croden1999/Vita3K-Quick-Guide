# 奖杯修改
每个游戏奖杯（除同游戏不同区域）不同，在修改之前你需要知道游戏对应的奖杯ID（例如：PCSH00250死或生沙滩排球3对应奖杯ID是NPWR10022_00），可以在`ux0\app\[TITLE_ID]\sce_sys\thophy`以及`ux0\user\[user_num]\trophy\data`中找到游戏对应的奖杯ID，在TROPUSR.DAT文件中使用十六进制编辑器浏览编辑，奖杯开头以0x04为起始，修改奖杯基本以F这个字符，来获取100%奖杯进度。奖杯时间修改以0x70为起始（这是白金奖杯的位置），每隔0x08为一个奖杯区间，可以修改任意一个时间点，但需要转换hex。

![1](https://user-images.githubusercontent.com/61804715/145160207-230fcf68-45cd-49c8-b6c4-2f3089d1b2d6.jpg)
![2](https://user-images.githubusercontent.com/61804715/145160375-37c8d3b7-92d1-437e-a578-90445a2ddb88.jpg)

## 演示
### 秋之回忆8
![3](https://user-images.githubusercontent.com/61804715/134748436-38d512ff-9d3d-48fe-afed-1d16963c48c2.png)
![4](https://user-images.githubusercontent.com/61804715/134748321-568ba06a-d757-477b-8595-24148ed9d112.png)

### 重力异想世界
- Before（未修改前）
![5](https://user-images.githubusercontent.com/61804715/134748607-ee706c7c-424a-4a8e-846e-2b5e46c98b11.png)
![6](https://user-images.githubusercontent.com/61804715/134748317-9c5af35b-976c-48ac-a35a-008f0831fb0d.png)

- After（修改后）
![7](https://user-images.githubusercontent.com/61804715/134748631-b9d876a7-3346-44c3-b1a3-76da23f9193e.png)
![8](https://user-images.githubusercontent.com/61804715/134748613-b7017b81-b783-4935-969d-25ace6a893fc.png)
