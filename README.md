# Asian Face DCGAN using keras

## Language options
* [中文](/README_CHINESE.md)
* [日本語](/README_JAPANESE.md)

## Table of contents
* English
    * [Introduction](#Introduction)
    * [Method](#Method)
    * [Architecture](#Architecture)
    * [Result](#Result)
    * [Learned](#Learned)

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
