# Python-Logistic Regression

## 線性分類-邏輯斯回歸(Logistic Regression) 
Logistic Regression則是一個平滑的曲線，當w0*x0+w1*x1+…+wn*xn越大時判斷成A類的機率越大，越小時判斷成A類的機率越小。

由於是二元分類，如果判斷成A類的機率越小，B類的機率越大(判斷成B類的機率 = 1 - 判斷成A的機率)。

### Sigmoid函數
Sigmoid函數，也稱為logistic function，這個函數的y 的值介於 0~1，這樣的分布也符合機率是在0~1的範圍中。Logistic Regression為什麼要用這個Logistic函數？其實也可以改用其他符合0~1的函數（因為機率的值是介於0~1），只是Logistic 函數是這種介於0~1的平滑函數中相對簡單的。


依下圖所示，當Z=0時判斷成+1類(A類)的機率為0.5，因此只要 z >0 判斷成 A類的機率就會>0.5 ，我們也就把它判斷成+1類(A類)。(這邊跟上一章perceptron一樣，只是多了機率的資訊) 如果z≤0 判斷成A類的機率就≤0.5 ，因此我們就把他判斷成-1類(B類)


<img width="450" height="350" src="https://github.com/EmiliaWANG1113/Machine-Learning/blob/main/Python-Logistic%20Regression/%E6%88%AA%E5%9C%96%202023-06-05%20%E4%B8%8B%E5%8D%883.55.40.png"/>
