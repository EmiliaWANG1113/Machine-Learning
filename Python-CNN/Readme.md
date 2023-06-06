# Python-CNN

## 卷積神經網絡(Convolutional Neural Network)
卷積神經網絡(Convolutional Neural Network)簡稱CNN，CNN是所有深度學習課程、書籍必教的模型(Model)，
CNN在影像識別方面的威力非常強大，許多影樣辨識的模型也都是以CNN的架構為基礎去做延伸。另外值得一提的是CNN模型也是少數參考人的大腦視覺組織來建立的深度學習模型，
學會CNN之後，對於學習其他深度學習的模型也會很有幫助，本文將為示範如何使用CNN來達成99%正確度的手寫數字辨識。

Perception優點：
1. 最簡單的線性分類演算法，Perception演算法的原理可推廣至其他複雜的演算法，因此許多課程或是書籍皆會以此當作最初的教材。

Perception缺點：
1. 一定要線性可分Perception演算法才會停下來（實務上我們沒辦法事先知道資料是否線性可分）
2. Perception演算法的錯誤率不會逐步收斂
3. Perception演算法只知道結果是A類還B類，但沒辦法知道是A, B類的機率是多少
