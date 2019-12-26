# ＤＣＧＡＮ生成亞洲人臉(使用keras)
* [簡介](#簡介)
* [結構](#結構)
* [成果](#成果)
* [學到的東西](#學到的東西)
## 簡介
使用ＡＦＡＤ作為DCGAN模型訓練資料產生亞洲人的臉

## 結構
使用ＤＣＧＡＮ
Sequential 1 是generator
Sequential 2 是discriminator

![](https://i.imgur.com/Neh3pu8.png)
## 成果
#### 下載一個generator model然後執行 [test.ipynb](/test.ipynb) 來產生臉
![](https://i.imgur.com/Z9wyikq.gif)

## 學到的東西
1. 在同一個epoch裡的不同batch不要用不一樣的noise,如果用不一樣的noise會鼓勵model生成同一種臉（生成同一種臉比較簡單？）
2. 要有耐心：有時候discriminator的accuracy在50%或100%是暫時的，等一下就沒事了
