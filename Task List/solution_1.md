# Activation function（激活函数）

## 定义：In artificial neural networks, the activation function of a node defines the output of that node, or "neuron," given an input or set of inputs.
### 激活函数在一个神经元当中跟随在 f(x) = wx + b 函数之后，用来加入一些 **非线性因素**。 If we do not apply a Activation function then the output signal would simply be a simple linear function.A linear function is just a polynomial of one degree.

## 类型
![image](https://github.com/songmingpeng/deep-learning/blob/master/Images/activation.png)

常见的激活函数如上表很多，但是ReLU函数是设计神经网络使用最广泛的，其实非线性的，比较容易反向传播误差。
ReLU缺点：不会同时激活所有的神经元。如果输入值是负的，ReLU函数会转换为0，而神经元不被激活。神经网络的这种稀疏性使其变得高效且易于计算。
         但同时也会导致很多死神经元。
         
         
## Conclusion
### The question was which one is better to use ?
### Answer to this question is that nowadays we should use ReLu which should only be applied to the hidden layers. And if your model suffers form dead neurons during training we should use leaky ReLu or Maxout function.

### It’s just that Sigmoid and Tanh should not be used nowadays due to the vanishing Gradient Problem which causes a lots of problems to train,degrades the accuracy and performance of a deep Neural Network Model.
