# Machine Learning_study notes

## Content
- [Learning Tutorials List](#learning_tuto)
- [知识点](#knowledge)
- [Questions](#questions)
- [掌握框架整理](#framework)
- [常用Tensorflow Functions](#tensorflow_functions)


## <h2 id="learning_tuto">Learning Tutorials List</h2>
当前学习中...

- [Machine learning - Coursera 课程](https://www.coursera.org/learn/machine-learning/home/welcome)
- [Google 官方机器学习教程](https://developers.google.cn/machine-learning/crash-course/)

教程资源列表：

- [Machine Learning Recipes - Google developers-Youtube Video](https://www.youtube.com/watch?v=cKxRvEZd3Mw&list=PLOU2XLYxmsIIuiBfYad6rFYQU_jL2ryal)



## <h2 id="knowledge">临时知识点记录</h2>

#### 回归 regression
凡是涉及到需要估计新的值的，预计新的值的，都用到回归。也是主要干这个估计新值用的。

##### TensorFlow 工具包的当前层次结构
<center> 
![TensorFlow 工具包的当前层次结构](https://developers.google.cn/machine-learning/crash-course/images/TFHierarchy.svg) 
</center>

##### TensorFlow 由以下两个组件组成：

- 图协议缓冲区
- 执行（分布式）图的运行时 

#####  scikit-learn 
[scikit-learn ](https://scikit-learn.org/stable/)是极其热门的 Python 开放源代码机器学习库，拥有超过 10 万名用户，其中包括许多 Google 员工。tf.estimator 与 scikit-learn API 兼容


## <h2 id="questions">Questions</h2>

## <h2 id="framework">掌握框架整理</h2>

## <h2 id="tensorflow_functions">Tensorflow Functions</h2>

```
import tensorflow as tf

静态值 
tf.constant([[1, 2, 3], [4, 5, 6]], dtype=tf.int32)

使用 tf.multiply 或 tf.pow 操作可求得 primes 矢量中每个元素值的平方。

tf.matmul(x, y)

tf.reshape(matrix, [2, 8])

print(reshaped_b.numpy())

# Create a scalar variable with the initial value 3.
v = tf.contrib.eager.Variable([3])

# Create a vector variable of shape [1, 4], with random initial values,
# sampled from a normal distribution with mean 1 and standard deviation 0.35.
w = tf.contrib.eager.Variable(tf.random_normal([1, 4], mean=1.0, stddev=0.35))

要更改变量的值，请使用 assign 操作：
tf.assign(v, [7])
向变量赋予新值时，其形状必须和之前的形状一致：


```


