# 城市轨道交通客流出行可视化技术


## 第五章

```
    客流出行特征的涵义：平均出行时间、平均出行距离、平均出行次数
```
本章关于客流出行特征可视化技术主要按照以下维度进行描述：
1. 客流特征关联可视化
2. 平均出行次数可视化
3. 片区平均停留时间轴可视化
4. 平均出行距离频率分布可视化
5. 平均出行时间分布可视化
6. 房价空间可视化

### 客流特征关联
由‘1’我们可以知道客流出行特征主要有三种：平均出行时间、平均出行距离与平均出行次数，这三者用于衡量客流出行特征。
客流出行特征可以对其他维度的分析进行影响。如房价偏高的轨道交通站点客流出行特征往往表现为平均出行时间较短，平均出行距离较短，平均停留时间较短但平均出行次数较多。房价偏低的轨道交通站点客流出行的特征则是相反。当要考虑到这些因素之间的相互影响的情况下时，在二维的情况下比较适合用雷达图进行表示。`此处存疑：尽管如此，如果维度的数量过多而且影响的正负、强度均不同时，用雷达图则很难分析`。但是在维度较少是，分析制作特征关联的可视化，雷达图仍不失为有效的方式。

### 平均出行次数、平均出行时间和平均出行距离
按照我们对第三章的分析，对于次数的比较方式有许多，典型的有南丁格尔玫瑰图，金字塔图等。按照书中所说，如果我们要比较多组数据在不同的功能区的表现：如工作日和周末分别在S0-S7这8个功能区的出行次数比较。则对图表的要求会更加挑剔一些，玫瑰图，金字塔图可能更加适用于单组数据的不同条件下的比较。如单纯的工作日或者单纯的周末在S0-S7这8个功能区的出行次数比较。这时候，书中给出的解决方案是利用两条折线图来展示，但这并非是最优解，折线图更适合用来表现一种变化的趋势，而不是展示多组数据。更好的解决方法是里用条形图或者雷达图，雷达图的各个轴代表了不同的功能区，颜色来区分工作日和周末。另外，热力图和第三章中提到的像素图(不知道还有没有人记得，就是github统计contribute次数的那张图)也是可以展示关键词为`次数`或者`频率`的图表，但是如果要展示多组数据，可能就要多绘制几张图表了。

对于出行距离的频率统计可视化手段，与次数类似，可以用条形图或者雷达图来表示。条形图如书上一般，每个区根据出行距离和频率做出一张条形图。而最后将全市的数据统一展示，放到一张大图中，这就是条形组图。而雷达图则如同次数统计图一般，各个轴代表不同的距离，在每条轴上的长度则代表频数。再用不同的颜色代表不同的行政区。

出行时间也是类似，条形组图、雷达图、平滑曲线图，与以上两种大同小异。小差异在于，对于时间的统计，我们可能会试图找其中一些规律性的东西，如早高峰，晚高峰等，这样条形组图并非十分试用。雷达图和平滑曲线图这样可以让多重数据重叠在一起且有峰、谷表现的图表，能不错地表现出一些规律。

### 房价空间可视化
二维作图下： 热力图
三位作图下： 三位立体喷泉图
没啥好说的，体现某一指标的高低与地理位置有关时，自然是在地图上做文章，二维用颜色来表示，三位用高度来表示。


