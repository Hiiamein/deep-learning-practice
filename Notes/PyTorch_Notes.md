# PyTorch学习笔记

## 小细节

### 1. numpy()和from_numpy()相互转化的问题
使用这两个方法将tensor和array相互转化后，共享内存。但其中一个的形状变化（比如转置）之后，另一个维持不变，但里面的元素还是按照原先的顺序一一对应。比如a.t_()之后，执行a[1, 0] = 0，对应变化的是b[0, 1]。

### 2. data()和detach()
data()和detach()方法都能返回不带梯度的tensor，但data()返回的值被修改后，原先的梯度也会变化，这样引起的错误不容易被发现。detach()返回值被修改后，用到原梯度时会报错，所以新版本推荐使用detach()。

### 3. nn.RNN/nn.LSTM中输入、输出的维度
model = nn.RNN(input_size, hidden_layer, num_layers)  
&emsp;&emsp;input_size是输入每一个单独数据自身的维度，即属性个数  
&emsp;&emsp;hidden_size是RNN的隐层单元数  
&emsp;&emsp;num_layers是RNN层数  
  
inputs = torch.randn(time_steps, batch_size, input_size)  
&emsp;&emsp;time_steps是输入时间序列的序列长度，如输入一个十个单词的句子，time_steps即为10  
&emsp;&emsp;batch_size就是字面意思  
&emsp;&emsp;input_size是输入每一个单独数据自身的维度，即属性个数（与上面一样)  
&emsp;&emsp;注意：这里是默认需要的inputs数据维度，batch_size位于第二维，如果在model的参数里面将batch_first=True，则需要的inputs维度变为(batch_size, time_steps, input_size)  
  
h0 = torch.zeros(num_layers, batch_size, hidden_size)  
out, h = model(inputs, h0)  
&emsp;&emsp;out的shape为[time_steps, batch_size, hidden_size]  
&emsp;&emsp;h的shape为[num_layers, batch_size, hidden_size]  
&emsp;&emsp;所以out[-1, :, :]与h[-1, :, :]相等
