# Support-Vector-Machine and Linear Regression

## SVM
SVM有三宝，间隔、对偶、核技巧  
定义：在特征空间上的间隔最大的线性分类器，即求解能够正确划分训练数据集并且几何间隔最大的分离超平面。  
区别于感知机：对于线性可分的数据集来说，感知机划分的超平面有无穷多个，但是几何间隔最大的分离超平面却是唯一的
  
## 推导  
 <div align=left><img width="1000" height="1700" src="https://github.com/zhenshen-mla/Support-Vector-Machine/blob/master/examples/total.png"/></div>  
 
## Linear Regression

回归用于预测输入变量和输出变量之间的关系，特别是当输入变量的值发生变化时，输出变量的值随之发生变化。回归模型正是表示从输入变量到输出变量之间映射的函数。
回归问题的学习等价于函数拟合：选择一条函数曲线使其很好地拟合已知数据且很好地预测未知数据。
回归就是要尽可能的把所有的样本点拟合到一条曲线上，尽管有的样本点不满足曲线，但是要使得离曲线距离尽可能近。  

  
## 推导  
 <div align=left><img width="1000" height="1700" src="https://github.com/zhenshen-mla/Support-Vector-Machine/blob/master/examples/linear regression.jpg"/></div>  
