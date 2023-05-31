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

1. 丟棄，如果資料量夠多
2. 補值(常見補值方式有補固定值、平均值、眾數、中位數)

scikit-learn內建的資料
[scikit-learn datasets](https://scikit-learn.org/stable/datasets/toy_dataset.html)

## EX: Iris dataset為例
鳶尾花資料集是非常著名的生物資訊資料集之一，取自美國加州大學歐文分校的機器學習資料庫

[Iris dataset](http://archive.ics.uci.edu/ml/datasets/Iris)
資料的總筆數為150筆，共有五個欄位：

1. 花萼長度(Sepal Length)：計算單位是公分
2. 花萼寬度(Sepal Width)：計算單位是公分
3. 花瓣長度(Petal Length) ：計算單位是公分
4. 花瓣寬度(Petal Width)：計算單位是公分
5. 類別(Class)：可分為Setosa，Versicolor和Virginica三個品種


<img width="450" height="350" src="https://github.com/EmiliaWANG1113/Python/blob/main/Python-sklearn/post3-3.jpg"/>
