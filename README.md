# Asian Face DCGAN using keras
## Table of contents
* English
    * [Introduction](#Introduction)
    * [Method](#Method)
    * [Architecture](#Architecture)
    * [Result](#Result)
    * [Learned](#Learned)

* [中文](/README_CHINESE.md)



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
#### Download a generator model and [test.ipynb](/test.ipynb) to generate faces
![](https://i.imgur.com/Z9wyikq.gif)

## Learned
1. Train with a same noise in the same epoch, otherwise the model will be prone to generate the same face --> mode collapse
2. Patient to the accuracy --> sometimes discriminator 50% or 100% accuracy is temporary





# DCGAN偽顔生成

## はじめに
DCGANモデルを使用して、アジア人の顔を生成します（トレーニングセット：AFAD）。
## 方法
DCGANモデルを使用
Sequential 1: 生成器
Sequential 2: 識別器
![](https://i.imgur.com/Neh3pu8.png)

## 結果
#### 生成器モデルと [test.ipynb](/test.ipynb) をダウンロードして顔を生成する
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
