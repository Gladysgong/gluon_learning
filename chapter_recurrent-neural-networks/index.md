# 循环神经网络

与之前介绍的多层感知机和卷积神经网络不同，循环神经网络（recurrent neural networks）引入了状态变量。在一个序列中，循环神经网络当前时刻的状态不仅保存了过去时刻的信息，还与当前时刻的输入共同决定当前时刻的输出。

循环神经网络常用于处理序列数据，例如一段文字或声音、购物或观影的顺序、甚至是图片中的一行或一列像素。因此，循环神经网络在实际中有着极为广泛的应用，例如语言模型、文本分类、机器翻译、语音识别、图像分析、手写识别和推荐系统。

由于本章中的应用基于语言模型，我们将先介绍语言模型的基本概念，并以此问题激发循环神经网络的设计灵感。接着，我们将描述循环神经网络中梯度计算方法，来探究循环神经网络训练可能存在的问题。对于其中的部分问题，我们可以使用本章稍后介绍的含门控的循环神经网络来解决。最后，我们将拓展循环神经网络的架构并介绍更精简的 Gluon 实现。

```eval_rst

.. toctree::
   :maxdepth: 2

   lang-model
   hidden-state
   rnn
   bptt
   gru
   lstm
   deep-rnn
   bi-rnn
   rnn-gluon
```