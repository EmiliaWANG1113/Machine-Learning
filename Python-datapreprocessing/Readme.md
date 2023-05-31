# Python-datapreprocessing

## 缺失值處理(Missing data)
1. 丟棄，如果資料量夠多
2. 補值(常見補值方式有補固定值、平均值、眾數、中位數)


## One-hot encoding
若要在空間中表示點，所有的特徵都需要是數值

如果是Male, Female, Not Specified，這三種都是等價的關係因此需要找一個方法讓這三個屬性距離原點是相同距離，而One-hot encoding 就可解決此問題，

首先將Male, Female, Not Specified由Gender從成一個欄位拆成三個欄位，因此編號1的使用者的屬性資料為(1,0,0)編號2的使用者為(0,1,0) 

編號三個使用者為(0,0,1)這三個使用者對於原點的距離都是1，即達成想要的結果。

但One-hot encoding的方法只適合類別種類少的形況，若類別種類太多就會產生出一大堆的特徵，造成其他的問題（比方說維數災難）。


## 資料特徵縮放(Feature Scaling)
特徵縮放是資料前處理的一個很重要的關鍵，只少有部分的Model不需要做特徵縮放，像是**決策樹**以及**隨機森林**。
需要特徵縮放主要是因為Model背後是用空間中的距離來做區分，假設某一個特徵過大，該Model的成本函數會被這個特徵所支配。

簡單來說特徵縮放主要有兩種方法(這兩種常被混淆)：

1. Normalization(歸一化、常態化、區間縮放)

   最常見的Normalization為0–1區間縮放，經過Normalization之後資料的範圍會介在0~1之間，原本的最大值變為1，最小值變為0


<img width="650" height="150" src="https://github.com/EmiliaWANG1113/Python/blob/main/Python-datapreprocessing/Normalization.png"/>


2. Standardization(標準化)

<img width="650" height="150" src="https://github.com/EmiliaWANG1113/Python/blob/main/Python-datapreprocessing/Standardization.png"/>
經過Standardization資料的平均值會變為0, 標準差變為1

