# Python-Normalization

在實務上我們在Train model時常常會遇到Overfitting的問題，
也是Model在Training的Data正確率很高，但是拿到Testing Data的時候錯誤率卻很高。
背後的主因是我們真正需要的Model比我們Train出來的Model還要簡單，也就是Train出來的Model太複雜了！
如上圖所示假設我們需要的Model是一條回歸的直線，但是Train出來的Model為了讓在Traing Data中錯誤率最小化，因此Model變得奇形怪狀，這樣的Model拿去新的資料中錯誤率就會很高


# 這時的解決方法：

1. 收集更多的Training Data
2. 減少資料的維度(特徵)
3. 使用更簡單的Model
4. 對現有的Model加上使用L1 or L2正規化(懲罰penalty)
