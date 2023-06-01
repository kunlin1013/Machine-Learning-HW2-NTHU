# Machine-Learning-HW2-NTHU

神經網路模型的結構由一系列疊加的層來組成，每一層都由多個神經元組成，並透過權重和偏差(Bias)進行運算。每個神經元的輸入都會經過一個激勵函數(activation function)的處理，產生該神經元的輸出。

簡單來說，兩層神經網路就是指有一個隱藏層和一個輸出層的神經網路。其中，隱藏層是神經網路中介於輸入層和輸出層之間的那一層。在這裡，我們採用sigmoid函數作為激勵函數，使得神經元的輸出在0到1之間。這樣做的好處是可以把線性問題轉變為非線性問題，從而能夠捕捉到數據中更複雜的模式和特徵。

在輸出層，因為我們需要處理多分類問題，我們選擇了softmax作為激勵函數。softmax函數的好處在於，它能把神經元的輸出轉變為概率分布，即所有神經元的輸出之和為1。這樣就可以方便地解釋每個類別的概率。

至於模型的學習，我們使用了一種稱為損失函數(loss function)的方法來評估模型的預測結果和真實結果的差距。在訓練過程中，我們的目標就是儘量減小這個損失。透過反向傳播(Backpropagation)和梯度下降(Gradient Descent)等算法，我們可以根據損失函數的計算結果來更新神經網路的權重和偏差，從而使得模型的預測結果越來越接近真實的結果。

![image](https://github.com/kunlin1013/Machine-Learning-HW2-NTHU/assets/78029945/b2d10fd9-6db4-4068-bc1a-f1bf33c6c550)

## HW2.py
HW2的程式檔案

## 函示庫版本
numpy                     1.17.0
opencv-python             4.5.4.60
scikit-learn              1.0.2
matplotlib                3.3.2

有了以上函示庫，還須將Data_test、Data_train這兩個資料集放在與HW2.py同個資料夾路徑下，即可執行程式碼。

## HW2_111061528_Programming.pdf
HW2詳細作法，裡面標題1、2、3、4分別對應到Part 2. Programming assignment中的1~4小題。

## HW2_111061528_Handwriting.pdf
HW2中證明題之詳細作法
