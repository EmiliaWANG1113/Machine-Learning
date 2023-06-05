# Python-Perceptron

## 感知器Perceptron（Perceptron Learning Algorithm，PLA）
* 為機器學習領域最早被開發出來的演算法
* Perceptron這個演算法只有在資料為線性可分的形況下才能正確分類（演算法才會停止）

Perception優點：
1. 最簡單的線性分類演算法，Perception演算法的原理可推廣至其他複雜的演算法，因此許多課程或是書籍皆會以此當作最初的教材。

Perception缺點：
1. 一定要線性可分Perception演算法才會停下來（實務上我們沒辦法事先知道資料是否線性可分）
2. Perception演算法的錯誤率不會逐步收斂
3. Perception演算法只知道結果是A類還B類，但沒辦法知道是A, B類的機率是多少
