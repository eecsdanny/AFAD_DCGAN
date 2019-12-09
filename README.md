# Asian Face DCGAN using keras
## Table of contents
* English
    * [Introduction](#Introduction)
    * [Method](#Method)
    * [Architecture](#Architecture)
    * [Result](#Result)
    * [Learned](#Learned)

* [中文](#ＤＣＧＡＮ生成亞洲人臉(使用keras))
    * [簡介](#簡介)
    * [結構](#結構)
    * [成果](#成果)
    * [學到的東西](#學到的東西)


* [日本語](#DCGAN偽顔生成)
    * [はじめに](#はじめに)
    * [方法](#方法)
    * [結果](#結果)
    * [学んだこと](#学んだこと)


* [More to do](#More)
* [Reference](#Reference)
## Introduction
Using DCGAN model to generate Asian faces (traing set： ＡＦＡＤ).

## Method
Use DCGAN
## Architecture
first block is generator
Second is Discriminator
![](https://i.imgur.com/Neh3pu8.png)

(using Google colab to train)

 
## Result
#### Download a generator model and test.py to generate faces
![](https://i.imgur.com/Z9wyikq.gif)

## Learned
1. Train with a same noise in the same epoch, otherwise the model will be prone to generate the same face --> mode collapse
2. Patient to the accuracy --> sometimes discriminator 50% or 100% accuracy is temporary


# ＤＣＧＡＮ生成亞洲人臉(使用keras)

## 簡介
使用ＡＦＡＤ作為DCGAN模型訓練資料產生亞洲人的臉

## 結構
使用ＤＣＧＡＮ
Sequential 1 是generator
Sequential 2 是discriminator

![](https://i.imgur.com/Neh3pu8.png)
## 成果
#### 下載一個generator model然後執行 test.py 來產生臉
![](https://i.imgur.com/Z9wyikq.gif)

## 學到的東西
1. 在同一個epoch裡的不同batch不要用不一樣的noise,如果用不一樣的noise會鼓勵model生成同一種臉（生成同一種臉比較簡單？）
2. 要有耐心：有時候discriminator的accuracy在50%或100%是暫時的，等一下就沒事了


# DCGAN偽顔生成

## はじめに
DCGANモデルを使用して、アジア人の顔を生成します（トレーニングセット：AFAD）。
## 方法
DCGANモデルを使用
Sequential 1: 生成器
Sequential 2: 識別器
![](https://i.imgur.com/Neh3pu8.png)

## 結果
#### 生成器モデルと test.py をダウンロードして顔を生成する
![](https://i.imgur.com/Z9wyikq.gif)

## 学んだこと
1. 同じエポックで同じノイズでトレーニングします。そうしないと、モデルは同じ顔を生成する傾向があります。 --> mode collapse
2. 辛抱強い --> 50％または100％の精度の識別器が一時的な場合がある

## More
1. Transfer learning
2. Use SRGAN to boost resolution
3. Improve resolution (GPU, Training set... etc)
## Reference
https://github.com/nyoki-mtl/keras-facenet/blob/master/notebook/demo-images.ipynb
https://www.tensorflow.org/tutorials/generative/dcgan
https://fairyonice.github.io/My-first-GAN-using-CelebA-data.html
https://github.com/nyoki-mtl/keras-facenet
https://arxiv.org/pdf/1511.06434.pdf
https://github.com/afad-dataset
