# 课题组deep learning学习小组

## 简介

我创建了三个分支，分别是陈哲、卢啸岩、兰凯鹏的姓名全拼，以后每个人做的东西都传到自己的分支上。**不要在master分支上做任何修改！** 大家不用参加什么杂七杂八的网上培训了，在这里，咱们就可以一起把深度学习学好（**前提是我布置的任务要认真完成**）。


## 注意事项
- data文件夹放到根目录的上一级，因为这个文件夹可能很大，GitHub仓库是有容量限制的。根目录里面也可以创建一个data文件夹，如果数据很小(比如小于40M)，就可以放到这里  
- 不懂的地方及时问我  
## 任务  
### 2019年5月17日——2019年5月24日  
- 熟悉四个最基础最常用的git命令，分别是git add, git commit, git push, git pull。  
- 学会pytorch的使用。把notebook中00，01，02，03，04，05的内容看懂，自己动手抄一遍代码，运行一下。这些是线性回归、逻辑回归、多层感知器、卷积神经网络、循环神经网络等算法的具体实现。你们可以尝试修改一下模型结构。
- 使用GitHub desktop管理仓库。Windows上用这个软件比git命令更方便，上面让你们掌握的git命令以后在Linux上会用到。
- 学会基本的markdown语法，这对于写技术文档里是非常重要的。后面会有**paper研读计划、实际项目练习**等，你们在学习过程中的经验教训等的总结都写在自己的分支里面。大家可以查看别人的branch，共同提高。

### 2019年7月15日——2019年7月21日

**图像分类重要论文研读。图像分类是深度学习中最基础最重要的任务，通过对图像分类的学习，可以透彻理解深度学习中最重要的基础知识。而且，在现实应用中，图像分类任务还有很多问题没有得到解决，因此图像分类值得多花时间学习研究。**

#### 任务

- [VGG](https://arxiv.org/abs/1409.1556)
  - 代码学习

- [PReLU-nets](https://arxiv.org/abs/1409.4842)
  - **各种激活函数分析**

- [GoogleNet](https://arxiv.org/abs/1409.4842)
  - 也叫Inception v1

- [ResNet](https://arxiv.org/abs/1512.03385)
  - 个人认为是深度学习中开天辟地的一篇论文:joy:
  - 代码学习

- [Inception v2 v3](https://arxiv.org/abs/1512.00567)

- [Inception v4](https://arxiv.org/abs/1602.07261)

- [WRN](https://arxiv.org/abs/1605.07146)
  - 学会分析网络深度、宽度和输入分辨率对计算量的影响

- [PyramidNet](https://arxiv.org/abs/1610.02915)

- [DenseNet](https://arxiv.org/abs/1608.06993)

- [ResNext](https://arxiv.org/abs/1611.05431)

- [Xception](https://arxiv.org/abs/1610.02357)

- [Residual Attention Network](https://arxiv.org/abs/1704.06904)
  - 基于attention机制的模型

- [SENet](https://arxiv.org/abs/1709.01507)
  - 也类似于attention机制，只不过是通道之间的attention

- [MobileNet v1](https://arxiv.org/abs/1704.04861)
  - 轻量级网络

- [ShuffleNet v1](https://arxiv.org/abs/1707.01083)
  - 轻量级网络

- [MobileNet v2](https://arxiv.org/abs/1801.04381)

- [ShuffleNet v2](https://arxiv.org/abs/1807.11164)

- [Res2Net](https://arxiv.org/abs/1904.01169)
  - 多尺度
#### 要求
- 做好笔记，不漏过任何一个知识点。**最后三个人合作写一个总结，放到master分支的notes文件夹中，文件名为“图像分类模型总结.md”**
- 任何有疑点的地方都要讨论清楚
