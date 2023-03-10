# A Tensor Notebook #



### 爱因斯坦求和约定 ###

	简单来说，爱因斯坦求和约定指的是：在表达式中如果出现两个相同的指标，则代表要对这个指标进行求和。这个指标因为不发挥实际的作用，我们称之为“哑指标”。
	
	具体来说，约定主要是：

* 在同一项中，如果同一指标（如上式中的i）成对出现，就表示遍历其取值范围求和。这时求和符号可以省略，如上所示。

* 上述成对出现的指标叫做哑指标，简称哑标。表示哑标的小写字母可以用另一对小写字母替换，只要其取值范围不变。

* 当两个求和式相乘时，两个求和式的哑标不能使用相同的小写字母。为了避免混乱，常用的办法是根据上一条规则，先将其中一个求和式的哑标改换成其它小写字母。

下面放一个简单的例子：

$a_1b_1+a_2b_2+a_3b_3=\sum_1^3 a_ib_i=a_ib_i $

### Kronecker记号 ###

$$ f(x)=\left\{
\begin{aligned}
x & = & \cos(t) \\
y & = & \sin(t) \\
z & = & \frac xy
\end{aligned}
\right.
$$