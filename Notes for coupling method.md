

## Notes for coupling method



## Def: Metric

A function  $d: S\times S\rightarrow \mathbb{R}$ is called a metric if:

1. $d(s,t)=d(t,s)\geq0$ for all $s,t \in S$
2. $d(s,t)=0$ if and only if $s=t$
3. $d(s,t) \leq d(s,u) + d(u,t)$ for all $s,t,u \in S$



#### 定义 总变差距离：

假设F,G是两个离散分布函数，在点$x_n$处的概率为$f_n,g_n$,则

$d_{TV}(F,G)=\sum_{k\geq1}|f_k-g_k|$



#### 耦合不等式：

首先，有：$|P(S=k)-P(P=k)|=|P(S=k,P\neq k)-P(P=k,S\neq k)|$

$\leq P(S=k,S\neq P)+P(P=k,S\neq P)$

因此可以得到：$d_{TV}(S,P)=\sum_k|P(S=k)-P(P=k)|\leq2P(S\neq P)$

可以发现距离可以被两个分布的随机变量不相等的概率控制住。



### Examples

#### Theorem-1:

​	设${X_r:1\leq r\leq n}$是独立的伯努利变量，参数为${p_r:1\leq r\leq n}$，设$S=\sum_{r=1}^n X_r$。再取$P\sim Poisson(\lambda),\lambda=\sum_{r=1}^np_r$,则有

$$d_{TV}(S,P)\leq2\sum_{r=1}^np_r^2$$



#### Proof to Theorem-1：

​	技巧是找到一个coupling，构造随机变量对序列$(X_r,Y_r)$，取值于$\{0,1\}\times\{0,1,2,...\}$,对应概率分布如下：
$$
Y = \begin{cases} 1-p_r  \quad if\quad x=y=0\\
e^{-p_r}-1+p_r  \quad if\quad x=1,y=0\\
\frac{p_r^y}{y!}e^{-p_r} \quad if\quad x=1,y\geq0
\end{cases}
$$
容易得到$X_r\sim B(p_r),Y_r\sim Poisson(p_r)$，进而可取$S=\sum_{r=1}^n X_r,P=\sum_{r=1}^n Y_r$满足条件。

根据上面的不等式，$d_{TV}(S,P)\leq2P(S\neq P)$，接下来只需要控制住$P(S\neq P)$

有：$P(S\neq P)\leq P(X_r\neq Y_r,\exists r)\leq\sum_{r=1}^nP(X_r \neq Y_r)=\sum_{r=1}^n\{e^{-p_r}-1+p_r+P(Y_r\geq2)\}$

$=\sum_{r=1}^np_r(1-e^{p_r})\leq\sum_{r=1}^np_r^2$

得证



## Notes for Renewal Theorem



#### Renewal Theorem:

若中间间隔时间的期望$\mu<+\infty$，且过程是non-arithmetic的，则$u_n=P(H_n)$满足当$n\to\infty$时$u_n\to\mu^{-1}$ 



