---
layout: post
title:  "Theano 之 Hello World"
date: 2016-08-19
categories: deep-learning
tags:  machine-learning, deep-learning, theano
---

* content
{:toc}



## 配置Theano运行环境

### 背景：

1. System: Win7 Professional
2. Anaconda 3, default python 3.5
3. No admin account

### 过程

1. 在Anaconda中新建一个python3.4的enviroment命名为py34， `conda create --name py34 python=3.4 anaconda`
2. 显示所有enviroment `conda info -e`
3. 激活py34 `activate py34`
4. 在py34里安装theano的dependences mingw和libpython（可能已经装好） `conda install mingw libpython`
5. 通过pip安装theano，`pip install Theano`
6. 将C:\Anaconda3\envs\py34 加入user enviroment path中的path。当激活py34开发环境的时候，在任何地方调用python都可以通过环境变量搜寻到Py34文件夹下的python.exe。


## 运行Theano tutorial

1. 下载theano tutorial的源代码 `git clone https://github.com/lisa-lab/DeepLearningTutorials.git`
2. 解压后到文件夹c:\theano_tutorial， `cd c:\theano_tutorial`
3. 打开Jupyter notebook， `Jupyter notebook`
4. 新建notebook theano_tutorial.ipynb
5. 在theano_tutorial.ipynb中实验其中的例子， 可以在例子中加入一些plot辅助理解

```
import matplotlib.pyplot as plt
%matplotlib inline
# edit the code to display some plot
# run logistic_sgd.py
%run code/logistic_sgd.py
# run cnn for handwritten digital recognition
%run code/convolutional_mlp.py
```