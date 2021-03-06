之前我希望有数学, 物理或者同等专业水平的同学, 能帮我指出一些错误或者一起讨论一些问题. 但发现有不少人没看懂, 责任一定在我, 没写得更通俗, 也希望读者能把在何处放弃反馈给我助我改进. 其中确实有错误, 不过不是很关键, 好奇心强的可以去发掘发掘.

这篇文章核心其实是旋转. 没看明白的我猜主要是被花式旋转转晕了. 

一开始是线代部分, 相信大部分人耐着性子能撑过这一段, 正交化过程的公式长了一点, 这一段主要是为了引入基, 正交化过程, 基函数, 为后面建立联系做准备. 可能与大家平时理解的点乘不一样, 这里的定义更泛, 比如函数的"点乘"定义到一定范围内的积分, 本质上只是把求和换成了积分而已.

接下来是拉氏算子, 这部分主要是解微分方程, 跳跃性不算强, 主要是读者先要认识这个解法, 需要一定的微分方程基础, 内容上比较一般, 属于谈球谐必会提及的数学内容.

下面转到旋转, 无穷小的旋转, 切换e的各种表示方式, 这是个人最喜爱的部分. 大家都接触过这几种: 
$$
e^{i\theta}= \cos\theta + i\sin\theta, \\
e^x = 1+x/1+x^2/2!+x^3/3!..., \\
e^x = \lim_{n\rightarrow\infty}(1+x/n)^n
$$

当x变成矩阵, 变成四元数, 变成微分算子, 这上面的公式一样适用, 因为我们的x满足乘法(合成法则)就可以了. 比如文中二维的旋转:
$$
\begin{pmatrix}
\cos\theta & \sin\theta \\
-\sin\theta & \cos\theta
\end{pmatrix}
= \cos\theta \begin{pmatrix}1&0\\0&1 \end{pmatrix} + \sin\theta \begin{pmatrix}0&1\\-1&0 \end{pmatrix}
\\
\begin{pmatrix}0&1\\-1&0 \end{pmatrix} ^2 = -\begin{pmatrix}1&0\\0&1 \end{pmatrix}
$$
我觉得对比$e^{i\theta}$, 可以看出上面一个矩阵与$i: i^2=-1$的关系了.

对函数的旋转是核心内容, 是我们为什么要用球谐去表达的原因, 以及球谐的各种性质都可以从里面获取. 通过矩阵与微分算子的对应, 两者最后合二为一殊途同归, 这部分是全文最难却是最有趣的, 参考了量子物理以及群表示的一些资料, 才打通了两者. 读完可能需要相当的耐心, 无奈我还没想到更加简明直观的方式去表达. 我还是很想再分享一下梯子算子(矩阵)$J_\pm$ 与 $\frac{d}{dx}$的联系: 反复使用$J_\pm$是有终点的, 因为他们是幂零的,  存在足够大的n使得$J_\pm ^n = 0$;  而对一个多项式$f(x)$, 我们反复求导, 也存在一个足够大的n使得 $\frac{d^nf}{dx^n}=0$. 这些有趣的现象往往蕴含着更多的内涵, 这也是我非常想触及的内容.

时枝正好像说过类似的话: 音乐家能看到音符的美妙, 而普通人可以通过听演奏来欣赏. 数学公式是数学的音符, 是最简洁的表达, 有时千言万语都很难表达几行公式, 那么如何"演奏"数学公式使得每个人都能欣赏? 这大概是门艺术吧.
