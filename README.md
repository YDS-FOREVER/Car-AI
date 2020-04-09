## own总结：
大概思路就是：
用全连层对汽车xy速度、方向角、五个方向距离墙的距离大小输入网络，输出的是xy速度、方向角的改变值操作。
在训练的时候每次保存最大走的距离最远的小车的对于的网络权重参数，然后使用遗传算法初始化新一轮的网络参数（即拿出一部分小车对其初始化好的参数权重进行随机扰动，目的增加多种参数，为了能刷选出更好的小车参数。）

# 小车AI-demo 0.1.1
- 邮箱:812860165@qq.com
- 原始工程地址：[https://github.com/heucoder/carAI-Demo](原工程)
[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)
- **使用python编写的小车AI，使用浅层神经网络控制小车，使用遗传算法选择表现表现好的神经网络；编译环境为python3.6.2**
## 小车部分
- 使用pygame绘制简易赛道和作为方块的小车，其中小车有速度、角度、距离赛道边缘距离等重要属。
## 神经网络
- 使用numpy编写的浅层神经网络
    - 包含数据层、线性层、和非线性层sigmoid
    - 提供了一个节点列表，用户可以更加方便的调整网络的大小
    - 没有使用bp算法优化，而是使用遗传算法进行优化
    - 实现了保存和加载网络参数功能
## 遗传算法
- distur_param:对权值进行随机扰动
- _replace_one_layer_param:随机重置某一层的权值

## 需要安装的python库
- numpy
- pygame
## 如何运行

进入Car-AI目录下，运行下列代码即可(linux/windows):
```python mainGame.py```
即可
## 适合人群
- 有一定的python基础，熟悉pygame库、对神经网络和遗传算法有一定的了解
## 视频见如下链接
https://zhuanlan.zhihu.com/p/60195914
### 存在的小问题
- 数值溢出问题






[]: https://github.com/heucoder/carAI-Demo
