# 数学是创造时空的浪漫

作者：诗弈羽弦

## 第一章 数学分析

### 1.1 数列极限与函数极限

1. 数列极限为有界量

   $$\lim_{n\to\infty}a_n=a:\forall\varepsilon>0,\exist N(\varepsilon)\in\N,s.t.\forall n>N(\varepsilon),|a_n-a|<\varepsilon$$

2. 数列极限为无穷

   $$\lim_{n\to\infty}a_n=\infty:\forall M>0,\exist N(M)\in\N,s.t.\forall n>N(M),|a_n|>M$$

3. 单调有界定理

   数列$\{a_n\}$极限存在，如果数列$\{a_n\}$单调递增有上界，或单调递减有下界。

4. $Cauchy$收敛原理

   数列$\{a_n\}$极限存在，当且仅当

   $$\forall\varepsilon>0,\exist N(\varepsilon)\in\N,s.t.\forall n,p>N(\varepsilon),|a_{n+p}-a_n|<\varepsilon$$

5. $Stolz$定理

   若$\{a_n\},\{b_n\}$极限均为无穷，且$b_n$严格递增趋于无穷，则

   $$\lim_{n\to\infty}\frac{a_n}{b_n}=\lim_{n\to\infty}\frac{a_n-a_{n-1}}{b_n-b_{n-1}}$$

   若$\{a_n\},\{b_n\}$极限均为零，且$b_n$严格单调，则

   $$\lim_{n\to\infty}\frac{a_n}{b_n}=\lim_{n\to\infty}\frac{a_n-a_{n-1}}{b_n-b_{n-1}}$$

6. 夹逼定理

   若$a_n\le b_n\le c_n$，则

   $$\lim_{n\to\infty}a_n=\lim_{n\to\infty}c_n=A\Rightarrow\lim_{n\to\infty}b_n=A$$

7. 平均收敛定理

   $$\lim_{n\to\infty}a_n=A\Rightarrow\lim_{n\to\infty}\frac{a_1+a_2+\cdots+a_n}n=A$$

8. 数列收敛则其所有子列均收敛

   若数列中某一子列发散，则数列发散，且

   $$\lim_{n\to\infty}a_{np+i}=a(i=0,1,\cdots,p-1)\Rightarrow\lim_{n\to\infty}a_n=a$$

9. 定积分求解数列极限

   $$\lim_{n\to\infty}\sum_{k=1}^n\frac 1nf(\frac kn)=\int_0^1f(x)dx$$

10. 其他实数相关定理

    确界存在定理，闭区间套定理，列紧性定理，有限覆盖定理

11. 常用数列极限

    $$\begin{aligned}
      &(1)\lim_{n\to\infty}\sqrt[n]a=\lim_{n\to\infty}\sqrt[n]n=1\\
      &(2)\lim_{n\to\infty}\frac{a^n}{n!}=\lim_{n\to\infty}\frac{n!}{n^n}=0\\
      &(3)e=\lim_{n\to\infty}(1+\frac 1n)^n=\lim_{n\to\infty}\sum_{k=0}^n\frac 1{k!}
      \end{aligned}$$

12. 函数极限在实数点处为有界量

    $$\lim_{x\to a}f(x)=A:\forall \varepsilon>0,\exist\delta(\varepsilon)>0,s.t.\forall 0<|x-a|<\delta(\varepsilon),|f(x)-A|<\varepsilon$$

13. 函数极限在实数点处为无穷

    $$\lim_{x\to a}f(x)=\infty:\forall M>0,\exist\delta(M)>0,s.t.\forall 0<|x-a|<\delta(M),|f(x)|>M$$

14. 函数极限在为无穷处为有界量

    $$\lim_{x\to \infty}f(x)=A:\forall \varepsilon>0,\exist X(\varepsilon)>0,s.t.\forall |x|>X(\varepsilon),|f(x)-A|<\varepsilon$$

15. 函数极限在无穷处为无穷

    $$\lim_{x\to \infty}f(x)=\infty:\forall M>0,\exist X(M)>0,s.t.\forall |x|>X(M),|f(x)|>M$$

16. 函数的连续性

    $$f(x)在x_0处连续:\forall \varepsilon>0,\exist \delta(\varepsilon)>0,s.t.\forall|x-x_0|<\delta(\varepsilon),|f(x)-f(x_0)|<\varepsilon$$

    更一般地

    $$f(x)在x_0处连续:\lim_{x\to x_0}f(x)=f(x_0)$$

17. 海涅定理

    $$若\lim_{n\to\infty}a_n=a,则\lim_{x\to a}f(x)=\lim_{n\to \infty}f(a_n)$$

18. 无穷小与有界

    $$\begin{aligned}
      &(1)无穷小:f(x_0)=o(g(x_0))\Leftrightarrow\lim_{x\to x_0}\frac{f(x)}{g(x)}=0\\
      &(2)有界:f(x)=O(g(x))\Leftrightarrow\exist M>0,s.t.|\frac{f(x)}{g(x)}|\le M
      \end{aligned}$$

19. 一致连续

    函数$f(x)$在定义域$I$上一致连续，定义为

    $$\forall\varepsilon>0,\exist\delta>0,s.t.\forall x',x''\in I,|x'-x''|<\delta\Rightarrow|f(x')-f(x'')|<\varepsilon$$

20. 间断点类型

    第一类间断点

    $$\begin{aligned}
      &(1)可去间断点:\lim_{x\to x_0^-}f(x)=\lim_{x\to x_0^+}f(x)\ne f(x_0)\\
      &(2)跳跃间断点:\lim_{x\to x_0^-}f(x)\ne\lim_{x\to x_0^+}f(x)
      \end{aligned}$$

    第二类间断点：$f(x_0^-)$与$f(x_0^+)$至少一个不存在，例如无穷间断点和振荡间断点。

21. 连续函数的最值定理

    连续函数在闭区间上必定能取到最大值和最小值。

22. 连续函数的零点存在定理

    $$若f(x)\in C(a,b),f(a)f(b)<0,则\exist\xi\in(a,b),f(\xi)=0$$

23. 连续函数的介质定理

    $$若f(x)\in C(a,b),[f(a)-A][f(b)-A]<0,则\exist\xi\in(a,b),f(\xi)=A$$

24. 常用等价无穷小和极限运算

    $$\begin{aligned}
      &(1)x\sim \sin x\sim\tan x\sim\arcsin x\sim\arctan x\sim\ln(x+1)\sim e^x-1\\
      &(2)\frac{x^2}2\sim 1-\cos x\sim x-\ln(1+x)\sim e^x-1-x\\
      &(3)(1+x)^\alpha-1\sim\alpha x\\
      &(4)\lim_{x\to x_0}u(x)^{v(x)}=\exp\{\lim_{x\to x_0}(v(x)\ln u(x))\}=\exp\{\lim_{x\to x_0}v(x)(u(x)-1)\}\\
      &(5)e^{x+f(x)}-e^{f(x)}=e^{f(x)}(e^x-1)\sim xe^{f(x)}
      \end{aligned}$$

### 1.2 一元函数微分学

1. 函数可导

   函数$f(x)$在点$x_0$处可导，当且仅当

   $$f'(x_0)=\lim_{h\to0}\frac{f(x_0+h)-f(x_0)}h存在,或当且仅当 f'(x_0^-)=f'(x_0^+)$$

   一元函数可导一定连续，连续不一定可导

2. 可导函数的单调性

   $$\begin{aligned}
     &(1)f(x)单调递增\Leftrightarrow f’(x)\ge 0\\
     &(2)f(x)严格单调递增\Leftrightarrow f'(x)除有限个点为零之外,其余点f'(x)>0
     \end{aligned}$$

3. 可导函数的驻点

   若$f'(x)=0$，则称$x$为函数$f(x)$的驻点

4. 可导函数极值的第一充分条件

   函数$f(x)$在包含$x_0$某一邻域内连续，且存在一个左邻域内导函数非负、右邻域内导函数非正，则$x_0$为函数的极大值点。若左邻域内导函数非正、右邻域内导函数非负，则$x_0$为函数的极小值点。

5. 可导函数极值的第二充分条件

   设$x_0$为$f(x)$的一个驻点，且$f''(x_0)<0$，则$x_0$为函数的极大值点。若$f''(x_0)>0$，则$x_0$为函数的极小值点。

6. 凸函数

   设函数$f(x)$在区间$I$上有定义，若$I$中任意两点$a,b$以及任意$\lambda\in(0,1)$，都有

   $$f((1-\lambda)a+\lambda b)\le(1-\lambda)f(a)+\lambda f(b)$$

   则称$f(x)$为$I$上的凸函数。若改变上述不等号的方向，则定义凹函数。

   若$f(x)$在$I$上二阶可导，则$f(x)$是凸函数$\Leftrightarrow\forall x\in I, f''(x)\ge0$

7. 二阶可导函数的拐点

   若函数$f(x)$在$x$的两侧分布严格凸和严格凹，且$f''(x)=0$，则称$x$为函数$f(x)$的拐点

8. $Fermat$引理

   若函数在极值点处可导，则其导数值为零。

9. $Role$定理

   若函数$f(x)\in C[a,b]$，$(a,b)$可导，$f(a)=f(b)$，则

   $$\exist\xi\in(a,b),s.t.f'(\xi)=0$$

10. $Lagrange$中值定理

    若函数$f(x)\in C[a,b]$，$(a,b)$可导，则

    $$\exist\xi\in(a,b),s.t.f'(\xi)=\frac{f(b)-f(a)}{b-a}$$

11. $Cauchy$中值定理

    若$f(x),g(x)\in C[a,b]$，$(a,b)$可导，$\forall x\in(a,b),g'(x)\ne0$，则

    $$\exist\xi\in(a,b),s.t.\frac{f'(\xi)}{g'(\xi)}=\frac{f(b)-f(a)}{g(b)-g(a)}$$

12. $Jensen$不等式

    若函数$f(x)$在$I$上是凸函数，取$\forall x_1,\cdots,x_n\in I,\lambda_1,\cdots,\lambda\in[0,1]$，满足$\sum \lambda_k=1$，则有

    $$f(\sum_{k=1}^n\lambda_k x_k)\le\sum_{k=1}^n\lambda_kf(x_k)$$

13. 常用导数公式（极其简单的函数不再介绍）

    一阶求导公式

    $$\begin{aligned}
      &(1)(\tan x)'=\sec^2x\\
      &(2)(\cot x)'=-\csc^2x\\
      &(3)(\sec x)'=\tan x\sec x\\
      &(4)(\csc x)'=-\cot x\csc x\\
      &(5)(\arcsin x)'=\frac 1{\sqrt{1-x^2}}\\
      &(6)(\arccos x)'=-\frac 1{\sqrt{1-x^2}}\\
      &(7)(\arctan x)'=\frac 1{1+x^2}\\
      &(8)({\rm{arccot}}x)'=-\frac 1{1+x^2}\\
      &(9)(a^x)'=a^x\ln a\\
      &(10)(\log_ax)'=\frac 1{x\ln a}
      \end{aligned}$$

    高阶求导公式

    $$\begin{aligned}
      &(1)(x^\alpha)^{(n)}=\alpha(\alpha-1)\cdots(\alpha-n+1)x^{\alpha-n}\\
      &(2)(e^{\lambda x})^{(n)}=\lambda^ne^{\lambda x}\\
      &(3)(\ln x)^{(n)}=(-1)^{n-1}\frac{(n-1)!}{x^n}\\
      &(4)(\frac 1{x+a})^{(n)}=(-1)^n\frac{n!}{(x+a)^{n+1}}\\
      &(5)(\sin kx)^{(n)}=k^n\sin(kx+\frac n2\pi)\\
      &(6)(\cos kx)^{(n)}=k^n\cos(kx+\frac n2\pi)
      \end{aligned}$$

14. $Leibniz$求导公式

    $$[f(x)g(x)]^{(n)}=\sum_{k=0}^nC_n^kf^{(n-k)}(x)g^{(k)}(x)$$

15. 带$Peano$余项的$Taylor$公式

    若$f(x)$在$x_0$处具有$n$阶导数，则在$x_0$附近有

    $$f(x)=\sum_{k=0}^n\frac{f^{k}(x_0)}{k!}(x-x_0)^k+o((x-x_0)^k)$$

16. $Maclaurin$公式

    带$Peano$余项的$Taylor$公式中$x_0=0$的特殊形式

17. 带$Lagrange$余项的$Taylor$公式

    若$f(x)$在$[a,b]$具有连续$n$阶导数，在$(a,b)$有$n+1$阶导数，则$\forall x,x_0\in[a,b]$，$\exists\xi\in(x,x_0)$或$(x_0,x)$，有

    $$f(x)=\sum_{k=0}^n\frac{f^{k}(x_0)}{k!}(x-x_0)^k+\frac{f^{(n+1)}(\xi)}{(n+1)!}(x-x_0)^{n+1}$$

18. 常用函数的$Taylor$展开

    需要考虑收敛域，参照$1.6$级数部分

19. $Taylor$展开式的另一种构造方法

    $$f(x\pm h)=\sum_{k=0}^n\frac{f^{k}(x)}{k!}(\pm h)^k+\frac{f^{(n+1)}(\xi)}{(n+1)!}(\pm h)^{n+1}$$

### 1.3 一元函数积分学

1. 不定积分

   对函数$f(x)$，若存在函数$F(x)$，使得在区间$I$上有$F'(x)=f(x)$，则$F(x)$为$f(x)$在$I$上的原函数。

   记$\int f(x)dx$为全体原函数，表示一个函数族

   $$\int f(x)dx=\int dF(x)=F(x)+C$$

   称$F(x)+C$为函数$f(x)$的不定积分。

2. 常用积分公式（求导部分出现过的不再介绍）

   $$\begin{aligned}
     &(1)\int \frac 1 xdx=\ln|x|+C\\
     &(2)\int\csc xdx=\ln|\csc x-\cot x|+C\\
     &(3)\int\sec xdx=\ln|\sec x+\tan x|+C\\
     &(4)\int\tan xdx=-\ln|\cos x|+C\\
     &(5)\int\cot xdx=\ln|\sin x|+C\\
     &(6)\int\frac 1{x^2+a^2}dx=\frac 1a\arctan\frac xa+C\\
     &(7)\int\frac 1{\sqrt{a^2-x^2}}dx=\arcsin\frac xa+C\\
     &(8)\int\frac 1{a^2-x^2}dx=\frac 1{2a}\ln|\frac{a+x}{a-x}|+C\\
     &(9)\int\frac 1{x^2-a^2}dx=\frac 1{2a}\ln|\frac{a-x}{a+x}|+C\\
     &(10)\int\frac 1{\sqrt{x^2\pm a^2}}dx=\ln|x+\sqrt{x^2\pm a^2}|+C\\
     &(11)\int\frac{x}{\sqrt{1+x^2}}dx=\sqrt{1+x^2}+C
     \end{aligned}$$

3. 积分求解常用换元方法

   三角换元、倒代换、有理分式拆分、凑微分（技巧性最强）、奇偶性构造（定积分）

4. 定积分的基本性质

   $$\begin{aligned}
     &(1)若f(x)\ge g(x),则\int_a^bf(x)dx\ge\int_a^bg(x)dx\\
     &(2)若m\le f(x)\le M，则m(b-a)\le\int_a^bf(x)dx\le M(b-a)
     \end{aligned}$$

5. 第一积分中值定理

   若函数$f(x),g(x)$在$[a,b]$上连续，且$g(x)$在$[a,b]$上不变号，则

   $$\exist\xi\in[a,b],s.t.\int_a^bf(x)g(x)dx=f(\xi)\int_a^bg(x)dx$$

   特别地，若函数$f(x)$在$[a,b]$上连续，则

   $$\exist\xi\in[a,b],s.t.\int_a^bf(x)dx=f(\xi)(b-a)$$

6. 第二积分中值定理

   若函数$f(x)$在$[a,b]$上可积，$g(x)$在$[a,b]$上单调递减，且$g(x)\ge0$，则

   $$\exist\xi\in[a,b],s.t.\int_a^bf(x)g(x)dx=g(a)\int_a^\xi f(x)dx$$

   若函数$f(x)$在$[a,b]$上可积，$g(x)$在$[a,b]$上单调递增，且$g(x)\ge0$，则

   $$\exist\eta\in[a,b],s.t.\int_a^bf(x)g(x)dx=g(a)\int_\eta^b f(x)dx$$

7. 第三积分中值定理

   设函数$f(x)$在$[a,b]$上可积，$g(x)$在$[a,b]$上单调，则

   $$\exist\xi\in[a,b],s.t.\int_a^bf(x)g(x)dx=g(a)\int_a^\xi f(x)dx+g(b)\int_\xi^bf(x)dx$$

8. 微积分基本定理：$Newton-Leibniz$公式

   若$F(x)$是连续函数$f(x)$在$[a,b]$上的一个原函数，则

   $$\int_a^bf(x)dx=F(b)-F(a)$$

9. 变上限函数求导公式

   $$\frac{d}{dx}\int_{v(x)}^{u(x)}f(t)dt=f[u(x)]u'(x)-f[v(x)]v'(x)$$

10. 对称区间的定积分

    若$f(x)$在对称区间$[-a,a]$上可积，则

    $$\begin{aligned}
      &若f(x)是偶函数,则\int_{-a}^af(x)dx=2\int_0^af(x)dx\\
      &若f(x)是奇函数,则\int_{-a}^af(x)dx=0
      \end{aligned}$$

11. 定积分的几何应用

    平面图形的面积

    $$\begin{aligned}
      &直角坐标形式:\int_a^bf(x)dx,(x,y)\in[a,b]\times[0,f(x)]\\
      &极坐标形式:\int_\alpha^\beta\frac 12r^2(\theta)d\theta,(r,\theta)\in[0,r(\theta)]\times[\alpha,\beta]\\
      &参数形式:\int_u^vy(t)dx(t),(x,y)\in[x(u),x(v)]\times[0,y(t)]
      \end{aligned}$$

    曲线$y=f(x)$绕$y$轴旋转得到的旋转体体积

    $$\begin{aligned}
      &直角坐标形式:\int_a^b2\pi f(x)xdx\\
      &参数形式:\int_u^v2\pi x(t)y(t)dx(t)
      \end{aligned}$$

    曲线$y=f(x)$绕$x$轴旋转得到的旋转曲面面积

    $$\begin{aligned}
      &直角坐标形式:2\pi\int_a^by\sqrt{1+[f'(x)]^2}dx\\
      &参数形式:2\pi\int_u^vy(t)\sqrt{1+(\frac{dy}{dx})^2}dx(t)
      \end{aligned}$$

    平面曲线的弧长公式

    $$\begin{aligned}
      &直角坐标形式:\int_a^b\sqrt{1+(y')^2}dx=\int_a^b\sqrt{(dx)^2+(dy)^2}\\
      &参数形式:\int_u^v\sqrt{(\frac{dx}{dt})^2+(\frac{dy}{dt})^2}dt\\
      &极坐标形式:\int_\alpha^\beta\sqrt{[r(\theta)]^2+[r'(\theta)]^2}d\theta
      \end{aligned}$$

12. 曲率公式

    $$K=\lim_{\Delta s\to0}\frac{\Delta\varphi}{\Delta s}=\frac{|y''|}{(1+y'^2)^{\frac 32}}$$

    曲率半径

    $$R=\frac 1K=\frac{(1+y'^2)^{\frac 32}}{|y''|}$$

13. 无穷积分

    $$\int_a^\infty f(x)dx=\lim_{A\to\infty}\int_a^Af(x)dx$$

14. 绝对收敛

    $$若\int_a^{\infty}|f(x)|dx收敛，则称\int_a^\infty f(x)dx绝对收敛，且\int_a^\infty f(x)dx收敛。$$

15. $Cauchy$收敛原理

    $\int_a^\infty f(x)dx$收敛的充要条件是

    $$\forall \varepsilon>0,\exist X(\varepsilon)\in\R,s.t.\forall A_2>A_1>X,|\int_{A_1}^{A_2}f(x)dx|<\varepsilon$$

16. 比较判别法

    设$f(x),g(x)$是$[a,+\infty)$上的非负函数，且有$\lim\limits_{x\to+\infty}\frac{f(x)}{g(x)}=l$，则

    $$\begin{aligned}
      &(1)若l<+\infty,则级数\int_a^{+\infty}g(x)dx收敛时,\int_a^{+\infty}f(x)dx收敛\\
      &(2)若l>0,则级数\int_a^{+\infty}g(x)dx发散时,\int_a^{+\infty}f(x)dx发散
      \end{aligned}$$

17. $P$级数敛散性讨论

    $$\begin{aligned}
      &\int_1^{+\infty}\frac 1{x^p}dx\begin{cases}发散,p\le 1\\收敛,p>1\end{cases}\\
      &\int_0^1\frac 1{x^p}dx\begin{cases}收敛,p<1\\发散,p\ge 1\end{cases}
      \end{aligned}$$

18. $Dirichlet$判别法

    若区间$[a,+\infty)$上定义的函数$f(x),g(x)$满足

    $$\begin{aligned}
      &(1)F(A)=\int_a^Af(x)dx在[a,+\infty)有界\\
      &(2)g(x)在[a,+\infty)单调,且\lim_{x\to+\infty}g(x)=0
      \end{aligned}$$

    则$\int_a^{+\infty}f(x)g(x)dx$收敛。

19. $Abel$判别法

    若区间$[a,+\infty)$上定义的函数$f(x),g(x)$满足

    $$\begin{aligned}
      &(1)无穷级数\int_a^{+\infty}f(x)dx收敛\\
      &(2)g(x)在[a,+\infty)单调有界
      \end{aligned}$$

    则$\int_a^{+\infty}f(x)g(x)dx$收敛。

20. 瑕积分

    若$a$为函数$f(x)$的暇点，则

    $$\int_a^bf(x)dx=\lim_{\eta\to0^+}\int_{a+\eta}^bf(x)dx$$

    瑕积分敛散性判别法与无穷积分判别法类似。

### 1.4 多元函数微分学

1. $\R^n$中的点列极限

   设$\{\boldsymbol{x_k}\}\in\R^n,\boldsymbol{a}\in\R^n$，则点列$\{\boldsymbol{x_k}\}$极限为$\boldsymbol{a}$定义为

   $$\lim_{k\to\infty}\boldsymbol{x_k}=\boldsymbol{a}:\forall\varepsilon>0,\exist N(\varepsilon)\in\N,s.t.\forall k>N,||\boldsymbol{x_k}-\boldsymbol{a}||<\varepsilon$$

   点列收敛于一点，等价于点列各分量收敛于该点各分量

   $$\lim_{k\to\infty}\boldsymbol{x_k}=\boldsymbol{a}\Leftrightarrow\lim_{k\to\infty}\boldsymbol{x_k^{(i)}}=\boldsymbol{a^{(i)}},i=1,2,\cdots,n$$

2. 多元函数的极限

   设$D\in\R^n,f:D\to\R$，则函数于点$\boldsymbol{x}_0$处收敛于$A$定义为

   $$\lim_{\boldsymbol{x}\to\boldsymbol{x_0}}f(\boldsymbol{x})=A:\forall\varepsilon>0,\exist\delta>0.s.t.\forall \boldsymbol{x}\in\{\boldsymbol{x}\in D|0<||\boldsymbol{x}-\boldsymbol{x_0}||<\delta\},|f(\boldsymbol{x})-A|<\varepsilon$$

3. 多元函数的$Heine$定理

   $$若\lim_{k\to\infty}\boldsymbol{x}=\boldsymbol{x_0},则\lim_{k\to\infty}f(\boldsymbol{x})=\lim_{\boldsymbol{x}\to\boldsymbol{x_o}}f(\boldsymbol{x_0})=A$$

4. 多元函数的$Cauchy$收敛准则

   $$极限\lim_{k\to\infty}f(\boldsymbol{x})存在,当且仅当对\forall\varepsilon>0,\exist\delta>0,s.t.\forall \boldsymbol{x'},\boldsymbol{x''}\in D,满足:\\
     0<||\boldsymbol{x'}-\boldsymbol{x_0}||,||\boldsymbol{x''}-\boldsymbol{x_0}||<\delta\Rightarrow|f(\boldsymbol{x'})-f(\boldsymbol{x''})|<\varepsilon$$

5. 多元函数的连续性

   $$f(\boldsymbol{x})在\boldsymbol{x_0}处连续\Leftrightarrow\lim_{\boldsymbol{x}\to\boldsymbol{x_0}}f(\boldsymbol{x})=f(\boldsymbol{x_0})$$

6. 多元函数的最值定理

   在有界闭区域$D$上的多元连续函数$f$在$D$上有界，且至少取得它的最大值和最小值各一次。

7. 多元函数的介值定理

   在有界闭区域$D$上的多元连续函数，如果在$D$上取得两个不同的函数值，则它在$D$上取得介于这两个函数值之间的任何值至少一次。

8. 多元函数的偏导数

   若关于$x$的一元函数$f(x,y_0)$在$x_0$处可导，则$z=f(x,y)$在$(x_0,y_0)$处对$x_0$的偏导数存在，即

   $$\frac{\part f(x_0,y_0)}{\part x}=\lim_{t\to0}\frac{f(x_0+t,y_0)-f(x_0,y_0)}t$$

9. 多元函数的全微分

   若多元函数$z=f(x,y)$在$(x_0,y_0)$的某一邻域内有定义，且$f(x,y)$在该点处的全增量可表示为

   $$\Delta z=A\Delta x+B\Delta y+o(\rho),\rho=\sqrt{(\Delta x)^2+(\Delta y)^2}$$

   则称$z=f(x,y)$在点$(x_0,y_0)$处可微，并记$z$在该点处的全微分为$dz=A\Delta x+B\Delta y$。

   函数可微的判断依据：函数$z=f(x,y)$在$(x_0,y_0)$处可微，当且仅当

   $$\lim_{\rho\to0^+}\frac{f(x_0+\Delta x,y_0+\Delta y)-f_x(x_0,y_0)\Delta x-f_y(x_0,y_0)\Delta y-f(x_0,y_0)}\rho=0$$

10. 若函数$z=f(x,y)$的两个偏导数连续，则函数可微，且

    $$dz=\frac{\part z}{\part x}dx+\frac{\part z}{\part y}dy$$

11. 方向导数的定义

    函数$z=f(x,y)$在一点沿某一方向$\boldsymbol{\vec{l}}$的变化率，称为方向导数，记为

    $$\frac{\part f}{\part\boldsymbol{\vec{l}}}=\lim_{\rho\to0^+}\frac{f(x+\Delta x,y+\Delta y)-f(x,y)}{\rho}$$

12. 方向导数与梯度的关系

    若方向$\boldsymbol{\vec{l}}$的单位向量为$(\cos\alpha,\cos\beta)$，函数的梯度为$\nabla f(x,y)=(\frac{\part f}{\part x},\frac{\part f}{\part y})$，则

    $$\frac{\part f}{\part\boldsymbol{\vec{l}}}=\frac{\part f}{\part x}\cos\alpha+\frac{\part f}{\part y}\cos\beta=(\cos\alpha,\cos\beta)\cdot(\frac{\part f}{\part x},\frac{\part f}{\part y})$$

13. 复合函数求导的链式法则

    设$m$元函数$f(u_1,u_2,\cdots,u_m)$在$(u_1,u_2,\cdots,u_m)$可微，$u_k(x_1,x_2,\cdots,x_n),k=1,2,\cdots,m$均为$n$元函数且在$(x_1,x_2,\cdots,x_n)$可微，则

    $$\frac{\part f}{\part x_i}=\sum_{k=1}^m\frac{\part f}{\part u_k}\frac{\part u_k}{\part x_i},i=1,2,\cdots,n$$

14. 高阶偏导数

    $$\frac{\part}{\part x}\frac{\part z}{\part y}=\frac{\part^2z}{\part x\part y}=f_{yx}(x,y)$$

15. 多元微分中值定理

    设$D\sub\R^n$是凸区域，$f:D\to\R$可微，则

    $$\forall \boldsymbol{a},\boldsymbol{b}\in D,\exist\boldsymbol{\xi}\in D,s.t.f(\boldsymbol{b})-f(\boldsymbol{a})=[\nabla f(\boldsymbol{\xi})]^T(\boldsymbol{b}-\boldsymbol{a})$$

16. 二元函数的$Taylor$公式

    $$f(x,y)=\sum_{k=0}^n\frac 1{k!}\left((x-x_0)\frac{\part}{\part x}+(y-y_0)\frac{\part}{\part y}\right)^kf(x_0,y_0)+R_k$$

    $Peano$余项形式为

    $$R_k=o(||(x-x_0,y-y_0)||^k)$$

    $Lagrange$余项形式为

    $$R_k=\frac 1{(k+1)!}\left((x-x_0)\frac{\part}{\part x}+(y-y_0)\frac{\part}{\part y}\right)^{k+1}f(x_0+\theta(x-x_0),y_0+\theta(y-y_0)),\theta\in(0,1)$$

17. 曲线的切线方程与法平面

    曲线的参数方程

    $$\begin{aligned}
      &若曲线方程为\begin{cases}
      x=x(t)\\y=y(t)\\z=z(t)
      \end{cases},则在曲线上t=t_0对应的点(x_0,y_0,z_0)处有:\\
      &切线:\frac{x-x_0}{x'(t_0)}=\frac{y-y_0}{y'(t_0)}=\frac{z-z_0}{z'(t_0)}\\
      &切向量:\boldsymbol{\vec{T}}=(x'(t_0),y'(t_0),z'(t_0))\\
      &法平面:x'(t_0)(x-x_0)+y'(t_0)(y-y_0)+z'(t_0)(z-z_0)=0
      \end{aligned}$$

    曲线的一般方程

    $$\begin{aligned}
      &若曲线方程为\begin{cases}F(x,y,z)=0\\G(x,y,z)=0\end{cases},则在曲线上一点(x_0,y_0,z_0)点处有:\\
      &\begin{cases}F_xdx+F_ydy+F_zdz=0\\G_xdx+G_ydy+G_zdz=0\end{cases}\\
      &切线:\frac{x-x_0}{dx}=\frac{y-y_0}{dy}=\frac{z-z_0}{dz}\\
      &切向量:\boldsymbol{\vec{T}}=(dx,dy,dz)\\
      &法平面:(x-x_0)dx+(y-y_0)dy+(z-z_0)dz=0\\
      &其中(dx,dy,dz)需要根据\nabla F(x_0,y_0,z_0),\nabla G(x_0,y_0,z_0)解出比例关系
      \end{aligned}$$

18. 曲面的切平面方程与法线方程

    $$\begin{aligned}
      &若曲面方程为F(x,y,z)=0,则在曲面上一点(x_0,y_0,z_0)处有:\\
      &切平面:F_x(x_0,y_0,z_0)(x-x_0)+F_y(x_0,y_0,z_0)(y-y_0)+F_z(x_0,y_0,z_0)(z-z_0)=0\\
      &法向量:\boldsymbol{\vec{n}}=\nabla F(x_0,y_0,z_0)\\
      &法线:\frac{x-x_0}{F_x(x_0,y_0,z_0)}=\frac{y-y_0}{F_y(x_0,y_0,z_0)}=\frac{z-z_0}{F_z(x_0,y_0,z_0)}
      \end{aligned}$$

19. 多元函数的极值

    极值必要条件

    $$若\boldsymbol{\vec a}为f的极值点,则\boldsymbol{\vec a}为f的驻点,即\nabla f(\boldsymbol{\vec a})=\boldsymbol{\vec 0}$$

    极值充分条件

    $$\begin{aligned}
      &设开集D\sub\R^n,f:D\to\R有二阶连续偏导数,且\boldsymbol{\vec a}为f的驻点,则:\\
      &(1)若\boldsymbol{\vec a}处的Hessen矩阵\nabla^2f(\boldsymbol{\vec a})正(负)定,则\boldsymbol{\vec a}为f的严格极小(大)值点\\
      &(2)若\boldsymbol{\vec a}处的Hessen矩阵\nabla^2f(\boldsymbol{\vec a})为不定方阵,则\boldsymbol{\vec a}不是f的极值点
      \end{aligned}$$

    二元函数的极值分析

    $$\begin{aligned}
      &若二元函数f(x,y)有二阶连续偏导数,记A=f_{xx},B=f_{xy},C=f_{yy},则:\\
      &(1)若AC-B^2>0,则f在A>0时有极小值,A<0时有极大值\\
      &(2)若AC-B^2<0,则f没有极值\\
      &(3)若AC-B^2=0,则f的极值情况不确定
      \end{aligned}$$

20. $Lagrange$乘子法

    $$\begin{aligned}
      &若\boldsymbol{x}\in\R^n,则目标函数f(\boldsymbol{x})和m个约束条件h_i(\boldsymbol{x})=0(i=1,\cdots,m)可以构成Lagrange函数\\
      &L(\boldsymbol{x},\boldsymbol{\lambda})=f(\boldsymbol{x})+\sum_{i=1}^m\lambda_ih_i(\boldsymbol{x}),其中\boldsymbol{\lambda}=(\lambda_1,\cdots,\lambda_m)\in\R^m\\
      &\begin{cases}\nabla L_{\boldsymbol{x}}(\boldsymbol{x},\boldsymbol{\lambda})=0\\\nabla L_{\boldsymbol{\lambda}}(\boldsymbol{x},\boldsymbol{\lambda})=0\end{cases}的解中的\boldsymbol{x}部分即为可能的极值点
      \end{aligned}$$

### 1.5 多元函数积分学

1. 二重积分的中值定理

   设$f(x,y)$在有界闭区域$D$上连续，区域$D$的面积为$\sigma$，则

   $$\exist(\xi,\eta)\in D,s.t.\iint\limits_Df(x,y)d\sigma=f(\xi,\eta)\sigma$$

2. 二重积分的一般换元

   $$\iint\limits_{D_{xy}}f(x,y)dxdy=\iint\limits_{D_{uv}}f(x(u,v),y(u,v))|J|dudv$$

   其中$Jacobi$矩阵的行列式$|J|=|\frac{\part(x,y)}{\part(u,v)}|=\begin{vmatrix}x_u&x_v\\y_u&y_v\end{vmatrix}=\begin{vmatrix}u_x&u_y\\v_x&v_y\end{vmatrix}^{-1}$

3. 二重积分的极坐标变换

   $$\begin{cases}x=r\cos\theta\\y=r\sin\theta\end{cases}\Rightarrow|J|=|\frac{\part(x,y)}{\part(r,\theta)}|=r$$

   更一般地

   $$\begin{cases}x=x_0+ar\cos\theta\\y=y_0+br\sin\theta\end{cases}\Rightarrow|J|=|\frac{\part(x,y)}{\part(r,\theta)}|=abr$$

4. 三重积分的一般换元

   $$\iiint\limits_{\Omega_{xyz}}f(x,y,z)dxdydz=\iiint\limits_{\Omega_{uvw}}f(x,y,z)|J|dudvdw$$

   其中$Jacobi$矩阵的行列式$|J|=|\frac{\part(x,y,z)}{\part(u,v,w)}|=\begin{vmatrix}x_u&x_v&x_w\\y_u&y_v&y_w\\z_u&z_v&z_w\end{vmatrix}=\begin{vmatrix}u_x&u_y&u_z\\v_x&v_y&v_z\\w_x&w_y&w_z\end{vmatrix}^{-1}$

5. 三重积分的柱坐标变换

   $$\begin{cases}x=r\cos\theta\\y=r\sin\theta\\z=z\end{cases}\Rightarrow|J|=|\frac{\part(x,y,z)}{\part(r,\theta,z)}|=r$$

   更一般地

   $$\begin{cases}x=x_0+ar\cos\theta\\y=y_0+br\sin\theta\\z=z_0+z\end{cases}\Rightarrow|J|=|\frac{\part(x,y,z)}{\part(r,\theta,z)}|=abr$$

6. 三重积分的球坐标变换

   $$\begin{cases}x=r\sin\varphi\cos\theta\\y=r\sin\varphi\sin\theta\\z=r\cos\varphi\end{cases}\Rightarrow|J|=|\frac{\part(x,y,z)}{\part(r,\theta,\varphi)}|=r^2\sin\varphi$$

   更一般地

   $$\begin{cases}x=x_0+ar\sin\varphi\cos\theta\\y=y_0+br\sin\varphi\sin\theta\\z=z_0+cr\cos\varphi\end{cases}\Rightarrow|J|=|\frac{\part(x,y,z)}{\part(r,\theta,\varphi)}|=abcr^2\sin\varphi$$

7. 空间曲面的面积

   $z=f(x,y)$在区域$D$上的曲面面积为

   $$S=\iint\limits_SdS=\iint\limits_D\sqrt{1+z_x^2+z_y^2}dxdy$$

8. 质心坐标

   以二维为例

   $$\overline x=\frac{\iint x\rho(x,y)dxdy}{\iint\rho(x,y)dxdy},\overline y=\frac{\iint y\rho(x,y)dxdy}{\iint\rho(x,y)dxdy}$$

9. 转动惯量

   $$J_l=\iint\limits_Dr^2(x,y)\rho(x,y)dxdy$$

10. 万有引力分量

    $$F_i=\iiint\limits_\Omega\frac{m\rho(x,y,z)(i-i_0)}{r^3}dxdydz,i\in\{x,y,z\}$$

11. 第一类曲线积分

    设曲线$L:\begin{cases}x=x(t)\\y=y(t)\end{cases},t\in[\alpha,\beta]$，则$f(x,y)$沿$L$的积分为

    $$\int\limits_Lf(x,y)ds=\int_\alpha^\beta f(x(t),y(t))\sqrt{x_t^2+y_t^2}dt$$

12. 第二类曲线积分

    设曲线$L:\begin{cases}x=x(t)\\y=y(t)\end{cases},t\in[\alpha,\beta]$，则$\vec F(x,y)$沿$L$的积分为

    $$\int\limits_L\vec F(x,y)d\vec s=\int\limits_LP(x,y)dx+Q(x,y)dy$$

    进一步

    $$\int\limits_LP(x,y)dx+Q(x,y)dy=\int_\alpha^\beta [P(x(t),y(t))x'(t)+Q(x(t),y(t))y'(t)]dt$$

13. 第一类曲线积分与第二类曲线积分互相转化

    $$若(\cos\alpha,\cos\beta)为沿曲线方向的单位切向量,则\begin{cases}dx=ds\cos\alpha\\dy=ds\cos\beta\end{cases}$$

14. $Green$公式

    设区域$D$是由分段光滑的曲线$L$围成，且$P(x,y),Q(x,y)$在$D$上具有一阶连续偏导，则

    $$\iint\limits_D(\frac{\part Q}{\part x}-\frac{\part P}{\part y})dxdy=\oint\limits_LPdx+Qdy$$

    特别地，闭合曲线$L$围成的面积为

    $$S=\iint\limits_Ddxdy=\oint\limits_Lxdy=\frac 12\oint\limits_Lxdy-ydx$$

15. 平面曲线积分与路径无关

    $$\begin{aligned}
      &设D是单连通闭区域,且P,Q在D上具有一阶连续偏导数，则在区域D内以下四个条件等价:\\
      &(1)\int\limits_LPdx+Qdy积分值与路径无关\\
      &(2)任意一条光滑闭曲线L,有\oint\limits_LPdx+Qdy=0\\
      &(3)存在可微函数u(x,y),使得du=Pdx+Qdy\\
      &(4)\frac{\part Q}{\part x}=\frac{\part P}{\part y}
      \end{aligned}$$

16. 第一类曲面积分

    设曲面$\Sigma:z=z(x,y)$，函数$f(x,y,z)$在曲面$\Sigma$上的积分为

    $$\iint\limits_\Sigma f(x,y,z)dS=\iint\limits_{D_{xy}}f(x,y,z(x,y))\sqrt{1+z_x^2+z_y^2}dxdy$$

17. 第一类曲面积分换元公式

    若曲面$\Sigma$以参数形式给出或换元为参数形式$\begin{cases}x=x(u,v)\\y=y(u,v)\\z=z(u,v)\end{cases}$，则$f(x,y,z)$在曲面$\Sigma$上的积分为

    $$\iint\limits_\Sigma f(x,y,z)dS=\iint\limits_{D_{uv}}f(x,y,z)\sqrt{EG-F^2}dudv$$

    其中$E,F,G$称为曲面$\Sigma$的第一基本量：$\begin{cases}E=x_u^2+y_u^2+z_u^2\\F=x_ux_v+y_uy_v+z_uz_v\\G=x_v^2+y_v^2+z_v^2\end{cases}$

18. 第二类曲面积分

    曲面向上、向右、向前时为正方向

    $$\iint\limits_L\vec F(x,y,z)d\vec S=\int\limits_LPdydz+Qdzdx+Rdxdy$$

19. 第一类曲面积分与第二类曲面积分互相转化

    $$若(\cos\alpha,\cos\beta,\cos\gamma)为曲面方向的单位法向量,则\begin{cases}dydz=dS\cos\alpha\\dzdx=dS\cos\beta\\dxdy=dS\cos\gamma\end{cases}$$

    以上关系也用于同一积分在不同投影曲面之间的相互转化

20. $Gauss$公式

    设函数$P,Q,R$在封闭区域$\Omega$内有一阶连续偏导，$\Sigma$为区域$\Omega$的边界，并取外侧，则

    $$\iiint\limits_\Omega(\frac{\part P}{\part x}+\frac{\part Q}{\part y}+\frac{\part R}{\part z})dxdydz=\oiint\limits_{\Sigma} Pdydz+Qdzdx+Rdxdy$$

21. $Stokes$公式

    设函数$P,Q,R$在曲面$\Sigma$内有一阶连续偏导，$\Gamma$为曲面$\Sigma$的正向边界，则

    $$\iint_\limits\Sigma(\frac{\part R}{\part y}-\frac{\part Q}{\part z})dydz+(\frac{\part P}{\part z}-\frac{\part R}{\part x})dzdx+(\frac{\part Q}{\part x}-\frac{\part P}{\part y})dxdy=\oint\limits_\Gamma Pdx+Qdy+Rdz$$

    或者记为行列式形式

    $$\iint_\limits\Sigma\begin{vmatrix}dydz&dzdx&dxdy\\\frac{\part}{\part x}&\frac{\part}{\part y}&\frac{\part}{\part z}\\P&Q&R\end{vmatrix}=\iint_\limits\Sigma\begin{vmatrix}\cos\alpha&\cos\beta&\cos\gamma\\\frac{\part}{\part x}&\frac{\part}{\part y}&\frac{\part}{\part z}\\P&Q&R\end{vmatrix}dS=\oint\limits_\Gamma Pdx+Qdy+Rdz$$

22. 空间曲线积分与路径无关

    $$\begin{aligned}
      &设\Omega是单连通闭区域,且P,Q,R在\Omega上具有一阶连续偏导数，则在区域\Omega内以下四个条件等价:\\
      &(1)\int\limits_LPdx+Qdy+Rdz积分值与路径无关\\
      &(2)任意一条光滑闭曲线L,有\oint\limits_LPdx+Qdy+Rdz=0\\
      &(3)存在可微函数u(x,y,z),使得du=Pdx+Qdy+Rdz\\
      &(4)\frac{\part Q}{\part x}=\frac{\part P}{\part y},\frac{\part R}{\part y}=\frac{\part Q}{\part z},\frac{\part P}{\part z}=\frac{\part R}{\part x}
      \end{aligned}$$

23. 场论初步

    $Hamilton$算子

    $$\nabla=(\frac{\part}{\part x},\frac{\part}{\part y},\frac{\part}{\part z})$$

    梯度、散度与旋度

    $$\begin{aligned}
      &若定义数量场f=f(x,y,z)和向量场\vec F=(P,Q,R),则有:\\
      &从数量场到向量场的梯度:grad(f)=\nabla f=(\frac{\part f}{\part x},\frac{\part f}{\part y},\frac{\part f}{\part z})\\
      &从向量场到数量场的散度:div(f)=\nabla\cdot f=\frac{\part f}{\part x}+\frac{\part f}{\part y}+\frac{\part f}{\part z}\\
      &从向量场到向量场的旋度:rot(\vec F)=\nabla\times\vec F=(\frac{\part R}{\part y}-\frac{\part Q}{\part z},\frac{\part P}{\part z}-\frac{\part R}{\part x},\frac{\part Q}{\part x}-\frac{\part P}{\part y})
      \end{aligned}$$

    有势场、保守场与无旋场

    $$\begin{aligned}
      &对于向量场\vec F=(P,Q,R),定义如下三种性质:\\
      &(1)\vec F是有势场\dj存在数量场u(x,y,z),使得grad(u)=\vec F\\
      &(2)\vec F是保守场\dj对任意闭曲线\Gamma,有\oint\limits_\Gamma Pdx+Qdy+Rdz=0\\
      &(3)\vec F是无旋场\dj对空间中任意一点,有rot(\vec F)=0\\
      &且以上三种定义在数学上等价
      \end{aligned}$$

24. 场论与积分公式

    $Green$公式和$Stokes$公式

    $$\iint\limits_\Sigma rot(\vec F)\cdot d\vec S=\oint\limits_\Gamma\vec F\cdot d\vec s$$

    $Gauss$公式

    $$\iiint\limits_\Omega div(\vec F)d\Omega=\oiint\limits_S\vec F\cdot d\vec S$$

### 1.6 数项级数与函数项级数

1. 无穷级数收敛的必要条件

   $$若\sum_{n=1}^\infty a_n收敛，则\lim_{n\to\infty}a_n=0$$

2. 正项级数收敛的充要条件

   $$正向级数\sum_{n=1}^\infty a_n(a_n\ge0)收敛\dj部分和序列\{S_n|S_n=\sum_{k=1}^na_k\}有界$$

3. 正项级数的比较判别法

   若$\exist N>0,n>N$时，满足$b_n\ge a_n\ge0$，则

   $$(1)\sum_{n=1}^\infty a_n发散\Rightarrow\sum_{n=1}^\infty b_n发散\\
     (2)\sum_{n=1}^\infty b_n收敛\Rightarrow\sum_{n=1}^\infty a_n收敛$$

   若$\exist N>0,n>N$时，满足$a_n,b_n\ge0$，则比较判别法极限形式成立

   $$\begin{aligned}
     &(1)若\lim_{n\to\infty}\frac{b_n}{a_n}\ge q>0,则 \sum_{n=1}^\infty a_n发散\Rightarrow\sum_{n=1}^\infty b_n发散\\
     &(2)若\lim_{n\to\infty}\frac{a_n}{b_n}\le q<\infty,则\sum_{n=1}^\infty b_n收敛\Rightarrow\sum_{n=1}^\infty a_n收敛
     \end{aligned}$$

4. 比较判别法常用参考级数

   $$\begin{aligned}
     &(1)等比级数:\sum_{n=1}^\infty q^n\begin{cases}
     |q|<1时收敛\\
     |q|\ge 1时发散
     \end{cases}\\
     &(2)P级数:\sum_{n=1}^\infty \frac 1{n^p}\begin{cases}
     p>1时收敛\\
     p\le 1时发散
     \end{cases}\\
     &(3)广义P级数:\sum_{n=2}^\infty \frac 1{n\ln^pn},\sum_{n=2}^\infty \frac 1{n\ln n\ln\ln^pn}等,收敛条件同上
     \end{aligned}$$

5. 正项级数的$Cauchy$判别法（根值判别法）

   $$\begin{aligned}
     &记q=\lim_{n\to\infty}\sqrt[n]{a_n},则级数\sum_{n=1}^\infty a_n\begin{cases}
     收敛,q<1\\
     发散,q>1\\
     判别法失效,q=1
     \end{cases}\\
     &若取\overline{q}=\overline{\lim_{n\to\infty}}\sqrt[n]{a_n},结论依然成立
     \end{aligned}$$

6. 正项级数的$D'Alembert$判别法（比值判别法）

   $$\begin{aligned}
     &记q=\lim_{n\to\infty}\frac{a_{n+1}}{a_n},则级数\sum_{n=1}^\infty a_n\begin{cases}
     收敛,q<1\\
     发散,q>1\\
     判别法失效,q=1
     \end{cases}\\
     &若取\overline{q}=\overline{\lim_{n\to\infty}}\frac{a_{n+1}}{a_n},结论依然成立
     \end{aligned}$$

7. 正项级数的$Cauchy$积分判别法

   设$x\ge1,f(x)\ge0$且单调递减，则

   $$无穷级数\sum_{n=1}^\infty f(n)与广义积分\int_1^{+\infty}f(x)dx同敛散$$

8. 一般项级数的绝对收敛判别法

   $$\sum_{n=1}^\infty |a_n|收敛\Rightarrow\sum_{n=1}^\infty a_n收敛$$

9. 交错级数的$Leibniz$判别法

   $$定义交错级数\sum_{n=1}^\infty a_n=\sum_{n=1}^\infty (-1)^nu_n(u_n>0)$$

   若$u_n$单调递减趋于零，则该交错级数称为$Leibniz$级数，且收敛

10. 一般项级数的$Dirichlet$判别法

    $$\begin{aligned}
      &如果以下两个条件同时成立:\\
      &(1)数列\{a_n\}的部分和\{S_n|S_n=\sum_{k=1}^na_k\}有界\\
      &(2)数列\{b_n\}是单调数列，且\lim_{n\to\infty}b_n=0\\
      &那么级数\sum_{n=1}^\infty a_nb_n收敛
      \end{aligned}$$

11. 一般项级数的$Abel$判别法

    $$\begin{aligned}
      &如果以下两个条件同时成立:\\
      &(1)级数\sum_{n=1}^na_n收敛\\
      &(2)数列\{b_n\}单调有界\\
      &那么级数\sum_{n=1}^\infty a_nb_n收敛
      \end{aligned}$$

12. 幂级数的$Abel$定理

    $$\begin{aligned}
      &对于幂级数\sum_{n=0}^\infty a_nx^n有以下两条结论成立:\\
      &(1)若有某点x_0\neq 0使得\sum_{n=0}^\infty a_nx_0^n收敛,则当|x|<|x_0|时,\sum_{n=0}^\infty a_nx^n绝对收敛\\
      &(2)若有某点x_1\neq 0使得\sum_{n=0}^\infty a_nx_1^n发散,则当|x|>|x_1|时,\sum_{n=0}^\infty a_nx^n发散
      \end{aligned}$$

13. 幂级数的收敛半径

    $$幂级数\sum_{n=0}^\infty a_nx^n的收敛半径为:R=\lim_{n\to\infty}\left|\frac{a_n}{a_{n+1}}\right|或R=\left(\overline{\lim_{n\to\infty}}\sqrt[n]{|a_n|}\right)^{-1}$$

    收敛域需要在$x\in\{R,-R\}$处单独讨论

14. 幂级数的换序运算

    幂级数求导与求和换序

    $$\begin{aligned}
      &\sum_{n=0}^\infty f(x)(n+1)x^n\\
      =&f(x)\left[\sum_{n=0}^\infty x^{n+1}\right]'\\
      =&\frac{f(x)}{(x-1)^2}\\
      \end{aligned}$$

    幂级数积分与求和换序

    $$\begin{aligned}
      &\sum_{n=0}^\infty f(x)\frac{x^{n+1}}{n+1}\\
      =&f(x)\int_0^x\left[\sum_{n=0}^\infty x^n\right]dx\\
      =&-f(x)\ln(1-x)
      \end{aligned}$$

15. 函数展开成$Taylor$级数

    $$f(x)=\sum_{n=0}^\infty \frac{f^{(n)}(x_0)}{n!}(x-x_0)^n$$

    特别地，当$x_0=0$时，上式称为$Maclaurin$级数

16. 常用泰勒级数及其收敛域

    $$\begin{aligned}
      &(1)\sin x=\sum_{n=0}^\infty\frac{(-1)^nx^{2n+1}}{(2n+1)!},x\in(-\infty,+\infty)\\
      &(2)\cos x=\sum_{n=0}^\infty\frac{(-1)^nx^{2n}}{(2n)!},x\in(-\infty,+\infty)\\
      &(3)e^x=\sum_{n=0}^\infty\frac{x^n}{n!},x\in(-\infty,+\infty)\\
      &(4)\frac 1{1-x}=\sum_{n=0}^\infty x^n,x\in(-1,1)\\
      &(5)\frac 1{1+x}=\sum_{n=0}^\infty(-1)^nx^n,x\in(-1,1)\\
      &(6)\frac 1{(1-x)^k}=\sum_{n=0}^\infty \begin{pmatrix}n+k-1\\n\end{pmatrix}x^n,x\in(-1,1)\\
      &(7)\ln(1+x)=\sum_{n=0}^\infty\frac{(-1)^nx^{n+1}}{(n+1)},x\in(-1,1]\\
      &(8)\arctan x=\sum_{n=0}^\infty \frac{(-1)^nx^{2n+1}}{2n+1},x\in(-1,1)\\
      &(9)\frac 12(e^x+e^{-x})=\sum_{n=0}^\infty\frac{x^{2n}}{(2n)!},x\in(-\infty,+\infty)\\
      &(10)(1+x)^\alpha=\sum_{n=0}^\infty\frac{\alpha(\alpha-1)\cdots(\alpha-n+1)}{n!}x^n,x\in\begin{cases}(-1,1),\alpha\le-1\\ (-1,1],-1<\alpha<1\\ [-1,1],\alpha>1\end{cases}
      \end{aligned}$$

17. 周期函数的$Fourier$级数

    周期为$2\pi$的函数可以展开为如下形式的$Fourier$级数

    $$f(x)=\frac{a_0}2+\sum_{n=1}^\infty\left(a_n\cos nx+b_n\sin nx\right)$$

    其中

    $$\begin{aligned}
      &a_n=\frac 1\pi\int_{-\pi}^{\pi}f(x)\cos nxdx,n=0,1,2\cdots\\
      &b_n=\frac 1\pi\int_{-\pi}^{\pi}f(x)\sin nxdx,n=1,2,3\cdots
      \end{aligned}$$

    周期函数为$2l$的函数可以展开为如下形式的$Fourier$级数

    $$f(x)=\frac{a_0}2+\sum_{n=1}^\infty\left(a_n\cos\frac{n\pi x}l+b_n\sin\frac{n\pi x}l\right)$$

    其中

    $$\begin{aligned}
      &a_n=\frac 1l\int_{-l}^{l}f(x)\cos\frac{n\pi x}ldx,n=0,1,2\cdots\\
      &b_n=\frac 1l\int_{-l}^{l}f(x)\sin\frac{n\pi x}ldx,n=1,2,3\cdots
      \end{aligned}$$

18. $Fourier$级数的$Dirichlet$收敛定理

    对于周期为$2\pi$的周期函数$f(x)$，展开为$Fourier$级数时，有

    $$\frac{a_0}2+\sum_{n=1}^\infty\left(a_n\cos nx+b_n\sin nx\right)=\lim_{t\to0^+}\frac{f(x+t)+f(x-t)}2$$

19. 奇函数、偶函数、非周期函数进行$Fourier$展开

    需要将非周期函数$f(x)$周期延拓为$F(x)$：可进行奇延拓或偶延拓，其中奇延拓需保证$F(0)=0$

    奇函数的$Fourier$级数只含正弦部分，又称正弦级数，以周期为$2\pi$的函数为例，有

    $$f(x)=\sum_{n=1}^\infty b_n\sin nx,b_n=\frac 2\pi\int_0^\pi f(x)\sin nxdx$$

    偶函数的$Fourier$级数只含余弦部分，又称余弦级数，以周期为$2\pi$的函数为例，有

    $$f(x)=\frac{a_0}2+\sum_{n=1}^\infty a_n\cos nx,a_n=\frac 2\pi\int_0^\pi f(x)\cos nxdx$$

20. $Fourier$级数相关的数项级数

    $$\begin{aligned}
      &(1)\sum_{n=1}^\infty\frac 1{n^2}=\frac{\pi^2}6\\
      &(2)\sum_{n=1}^\infty\frac{(-1)^2}{n^2}=\frac{\pi^2}{12}\\
      &(3)\sum_{n=0}^\infty\frac 1{(2n+1)^2}=\frac{\pi^2}8\\
      \end{aligned}$$

### 1.7 常微分方程

1. 变量分离方程

   $$\frac{dy}{dx}=\frac{f(x)}{g(y)}\Rightarrow\int g(y)dy=\int f(x)dx+C$$

2. 齐次微分方程

   $$\frac{dy}{dx}=f(\frac{y}{x})(令y=ux)\Rightarrow\int\frac{du}{f(u)-u}=\int\frac{dx}{x}+C$$

3. 齐次微分方程的推广

   $$\begin{aligned}
     &\frac{dy}{dx}=f(\frac{ax+by+c}{mx+ny+l})\\
     &(1)\left|\begin{matrix}a&b\\m&n\end{matrix}\right|\neq 0,令\begin{cases}X=x-x_0\\Y=y-y_0\\Y=UX\end{cases}\Rightarrow\frac{dY}{dX}=f(\frac{aX+bY}{mX+nY})=g(\frac{Y}{X})\\
     &(2)\left|\begin{matrix}a&b\\m&n\end{matrix}\right|=0,令u=ax+by\Rightarrow\frac{du}{dx}=bf(\frac{u+c}{\frac{m}{a}u+l})+a=g(u)
     \end{aligned}$$

4. 一阶线性微分方程

   $$\begin{aligned}
     &\frac{dy}{dx}+P(x)y=Q(x)\\
     &基础解系:f(x)=e^{\int-P(x)dx}\\
     &齐次通解形式:y=Cf(x)\\
     &非齐次通解形式:y=C(x)f(x)\\
     &求解C(x):C'(x)f(x)=Q(x)\\
     &非齐次通解公式:y=e^{\int-P(x)dx}(\int Q(x)e^{\int P(x)dx}dx+C)
     \end{aligned}$$

5. 伯努利方程

   $$\frac{dy}{dx}+P(x)y=Q(x)y^\alpha(令u=y^{1-\alpha})\Rightarrow\frac{du}{dx}+(1-\alpha)P(x)u=(1-\alpha)Q(x)$$

   若$\alpha>0$，则$y=0$也是方程的解

6. 二阶线性常系数微分方程：

   $$\begin{aligned}
     &\frac{d^2y}{dx^2}+p\frac{dy}{dx}+qy=r(x)\\
     &特征方程:r^2+px+q=0\\
     &基础解系:f_1(x),f_2(x)=\begin{cases}
     e^{\alpha x},xe^{\alpha x},二重根\\
     e^{\alpha x},e^{\beta x},不同根\\
     e^{\alpha x}\cos\beta x,e^{\alpha x}\sin\beta x,复数根\\
     \end{cases}\\
     &齐次通解形式:y=C_1f_1(x)+C_2f_2(x)\\
     &非齐次通解形式:y=C_1(x)f_1(x)+C_2(x)f_2(x)\\
     \end{aligned}$$

   $$\begin{aligned}
     &求解C_{1,2}(x):\begin{cases}
     C_1'(x)f_1(x)+C_2'(x)f_2(x)=0\\
     C_1'(x)f_1'(x)+C_2'(x)f_2'(x)=r(x)\\
     \end{cases}\\
     &或采用待定系数法:\\
     &(1)当r(x)=e^{\mu x}P_m(x)时,P_m(x)表示最高次数为m次的实多项式:\\
     &实多项式特解形式:y^*=x^ke^{\mu x}A_m(x),k为\mu在特征方程根中的重数\\
     &(2)当r(x)=e^{\mu x}(A_k(x)\cos\lambda x+B_l(x)\sin\lambda x)时,取m=\max(k,l):\\
     &复多项式特解形式:y^*=x^ke^{\mu x}[A_m(x)\cos\lambda x+B_m(x)\sin\lambda x],k为\mu\pm\lambda i的重数
     \end{aligned}$$

7. 恰当方程与积分因子

   $$\begin{aligned}
     &若\frac{\part M}{\part y}=\frac{\part N}{\part x},则微分方程Mdx+Ndy=0称为恰当方程\\
     &且方程的解为\int Mdx+Ndy=C
     \end{aligned}$$

   若不满足，则可寻找积分因子$\mu(x,y)$使得$\mu Mdx+\mu Ndy=0$是恰当方程

   $$\begin{aligned}
     &(1)若\frac{\part}{\part y}[\frac 1N(\frac{\part M}{\part y}-\frac{\part N}{\part x})]=0,则可求得\mu(x)=\exp\{\int\frac 1N(\frac{\part M}{\part y}-\frac{\part N}{\part x})dx\}\\
     &(2)若\frac{\part}{\part x}[\frac 1M(\frac{\part M}{\part y}-\frac{\part N}{\part x})]=0,则可求得\mu(y)=\exp\{\int\frac 1M(\frac{\part M}{\part y}-\frac{\part N}{\part x})dy\}
     \end{aligned}$$

8. 一阶隐式微分方程

   $(1)$方程形式为$y=f(x,y')$，令$p=y'$

   $$\begin{aligned}
     &原方程两边对x求导:p=\frac{df}{dx}+\frac{df}{dp}\frac{dp}{dx}\\
     &(1)若方程有解:p=\varphi(x,C),则原方程有通解:y=f(x,\varphi(x,C))\\
     &(2)若方程有解:x=\psi(p,C),则原方程有通解:\begin{cases}x=\psi(p,C)\\y=f(\psi(p,C),p)\end{cases}\\
     &(3)若方程有解:\phi(x,p,c)=0,则原方程有通解:\begin{cases}\phi(x,p,c)=0\\y=f(x,p)\end{cases}
     \end{aligned}$$

   $(2)$方程形式为$F(x,y')=0$，令$p=y'$

   $$合理构造\begin{cases}x=\varphi(t)\\p=\psi(t)\end{cases},使得方程有解:\begin{cases}x=\varphi(t)\\y=\int\psi(t)\varphi'(t)dt+C\end{cases}$$

   $(3)$方程形式为$F(y,y')=0$，令$p=y'$

   $$\begin{aligned}
     &合理构造\begin{cases}y=\varphi(t)\\p=\psi(t)\end{cases},使得方程有解:\begin{cases}x=\int\frac{\varphi'(t)}{\psi(t)}dt+C\\y=\varphi(t)\end{cases}\\
     &此外,若方程F(y,0)=0有实根y=k,则y=k也是方程的解
     \end{aligned}$$

9. 微分方程的奇解

   若微分方程的某个解上任意一点至少还有方程的另外一个解存在，则该解称为微分方程的奇解

   $$其中p-判别曲线\begin{cases}F(x,y,p)=0\\F'_p(x,y,p)=0\end{cases}(p=\frac{dy}{dx})即为可能的奇解,需进一步验证$$

10. 克莱罗微分方程

    $$\begin{aligned}
      &y=xp+f(p),p=\frac{dy}{dx}连续可微时称为克莱罗微分方程\\
      &其通解为y=cx+f(c),奇解为通解直线族的包络
      \end{aligned}$$

11. 高阶常系数线性微分方程

    $$\begin{aligned}
      &微分方程:\frac{d^nx}{dt^n}+a_1\frac{d^{n-1}x}{dt^{n-1}}+\cdots+a_{n-1}\frac{dx}{dt}+a_nx=f(t)\\
      &特征方程:r^n+a_1r^{n-1}+\cdots+a_{n-1}r+a_n=0\\
      &k重实根\lambda的基础解系:t^{i-1}e^{\lambda t}(i=1,2,\cdots,k)\\
      &k重复根\alpha\pm\beta i的基础解系:t^{i-1}e^{\alpha t}\sin\beta t,t^{i-1}e^{\alpha t}\cos\beta t(i=1,2,\cdots,k)\\
      \end{aligned}$$

    待定系数法求解

    $$\begin{aligned}
      &(1)当f(t)=e^{\mu t}P_m(t)时,P_m(t)表示最高次数为m次的实多项式:\\
      &实多项式特解形式:x^*=t^ke^{\mu t}A_m(t),k为\mu在特征方程根中的重数\\
      &(2)当f(t)=e^{\mu t}(A_k(t)\cos\lambda t+B_l(t)\sin\lambda t)时,,取m=\max(k,l):\\
      &复多项式特解形式:x^*=t^ke^{\mu t}[A_m(t)\cos\lambda t+B_m(t)\sin\lambda t],k为\mu\pm\lambda i的重数\\
      \end{aligned}$$

    常数变易法求解

    $$\begin{aligned}
      &若x_1,\cdots,x_n构成齐次通解的基础解系,则非齐次通解为x=\sum_{k=1}^nC_k(t)x_k,其中\\
      &\sum_{k=1}^nC_k'(t)x_k^{(i)}(t)=0(i=0,1,\cdots,n-2)\\
      &\sum_{k=1}^nC_k'(t)x_k^{(n-1)}(t)=f(t)
      \end{aligned}$$

12. 欧拉方程

    $$\begin{aligned}
      &方程形式:x^n\frac{d^ny}{dx^n}+a_1x^{n-1}\frac{d^{n-1}y}{dx^{n-1}}+\cdots+a_{n-1}x\frac{dy}{dx}+a_ny=0\\
      &换元方式:令x=e^t或t=\ln x\\
      &换元结果:D(D-1)\cdots(D-k+1)y+\cdots+a_{n-1}Dy+a_ny=0,其中D=\frac{d}{dt}
      \end{aligned}$$

13. 二阶齐次线性方程与刘维尔公式

    $$\begin{aligned}
      &对于方程\frac{d^2y}{dx^2}+P(x)\frac{dy}{dx}+Q(x)y=0,如果已知一个特解y_1,则可以求出通解\\
      &根据刘维尔公式,齐次方程通解为:y=C_1y_1+C_2y_1\int\frac 1{y_1^2}e^{-\int P(x)dx}dx\\
      &通过观察法求特解:\\
      &(1)P(x)+xQ(x)=0\Rightarrow y=x\\
      &(2)1+P(x)+Q(x)=0\Rightarrow y=e^x\\
      &(3)1-P(X)+Q(x)=0\Rightarrow y=e^{-x}
      \end{aligned}$$

## 第二章 线性代数

### 2.1 空间向量与立体解析几何

1. 三维向量的点积与叉积

   设$\boldsymbol{a}=(a_1,a_2,a_3),\boldsymbol{b}=(b_1,b_2,b_3)$，则

   $\boldsymbol{a}\cdot\boldsymbol{b}=|\boldsymbol{a}||\boldsymbol{b}|\cos(\boldsymbol{a},\boldsymbol{b})=a_1b_1+a_2b_2+a_3b_3$

   $\boldsymbol{a}\times\boldsymbol{b}=\begin{vmatrix}\boldsymbol{i}&\boldsymbol{j}&\boldsymbol{k}\\a_1&a_2&a_3\\b_1&b_2&b_3\end{vmatrix}$，方向满足右手系

2. 三维向量的混合积

   $$[\boldsymbol{a},\boldsymbol{b},\boldsymbol{c}]=(\boldsymbol{a}\times\boldsymbol{b})\cdot \boldsymbol{c}=\begin{vmatrix}a_1&a_2&a_3\\b_1&b_2&b_3\\c_1&c_2&c_3\end{vmatrix}$$

3. 向量间的关系

   $\boldsymbol{a}\bot\boldsymbol{b}\Leftrightarrow\boldsymbol{a} \cdot\boldsymbol{b}=0$

   $\boldsymbol{a}//\boldsymbol{b}\Leftrightarrow\boldsymbol{a}\times\boldsymbol{b}=0\Leftrightarrow\lambda\boldsymbol{a}=\mu\boldsymbol{b}$，其中$\lambda,\mu$不全为零

   $\boldsymbol{a},\boldsymbol{b},\boldsymbol{c}$共面$\Leftrightarrow\boldsymbol{a},\boldsymbol{b},\boldsymbol{c}$线性相关$\Leftrightarrow[\boldsymbol{a},\boldsymbol{b},\boldsymbol{c}]=0$

4. 平面方程

   $$\begin{aligned}
     &(1)点法式:A(x-x_0)+B(y-y_0)+C(z-z_0)=0\\
     &(2)一般式:Ax+By+Cz+D=0\\
     &(3)截距式:\frac xa+\frac yb+\frac zc=1\\
     &(4)通过直线\begin{cases}L_1(x,y,z)=0\\L_2(x,y,z)=0\end{cases}的平面束方程:\lambda L_1+\mu L_2=0
     \end{aligned}$$

5. 空间直线方程

   $$\begin{aligned}
     &(1)对称式:\frac{x-x_0}m=\frac{y-y_0}n=\frac{z-z_0}p\\
     &(2)参数式:\begin{cases}x=x_0+mt\\y=y_0+nt\\z=z_0+pt\end{cases}\\
     &(3)一般式:\begin{cases}A_1x+B_1y+C_1z+D_1=0\\A_2x+B_2y+C_2z+D_2=0\end{cases}
     \end{aligned}$$

6. 点、空间直线、平面之间的关系

   设平面$\pi_1,\pi_2$的法向量为$\boldsymbol{n}_1,\boldsymbol{n}_2$，直线$L_1,L_2$的切向量为$\boldsymbol{s}_1,\boldsymbol{s}_2$，则

   相互垂直$\Leftrightarrow$对应向量点积为零

   相互平行$\Leftrightarrow$对应向量叉积为零向量

   平面夹角余弦：$\cos\theta=\frac{\boldsymbol{n}_1\cdot\boldsymbol{n}_2}{|\boldsymbol{n}_1||\boldsymbol{n}_2|}$

   直线夹角余弦：$\cos\theta=\frac{\boldsymbol{s}_1\cdot\boldsymbol{s}_2}{|\boldsymbol{s}_1||\boldsymbol{s}_2|}$

   直线与平面夹角的正弦：$\sin\theta=\frac{\boldsymbol{n}\cdot\boldsymbol{s}}{|\boldsymbol{n}||\boldsymbol{s}|}$

   点$(x_0,y_0,z_0)$到平面$Ax+By+Cz+D=0$的距离

   $$d=\frac{|Ax_0+By_0+Cz_0+D|}{\sqrt{A^2+B^2+C^2}}$$

7. 曲面方程

   旋转曲面：$\begin{cases}f(y,z)=0\\x=0\end{cases}$绕$z$轴旋转的旋转曲面方程是$f(\pm\sqrt{x^2+y^2},z)=0$

   柱面：准线为$\begin{cases}f(x,y)=0\\z=0\end{cases}$，母线平行于$z$轴的柱面方程是$f(x,y)=0$

8. 二次曲面

   球面：$x^2+y^2+z^2=r^2$

   椭球面：$\frac{x^2}{a^2}+\frac{y^2}{b^2}+\frac{z^2}{c^2}=1$

   圆锥面：$z^2=a^2(x^2+y^2)$

   椭圆锥面：$\frac{x^2}{a^2}+\frac{y^2}{b^2}=z^2$

   单叶双曲面：$\frac{x^2}{a^2}+\frac{y^2}{b^2}-\frac{z^2}{c^2}=1$

   双叶双曲面：$\frac{x^2}{a^2}-\frac{y^2}{b^2}-\frac{z^2}{c^2}=1$

   椭圆抛物面：$\frac{x^2}{a^2}+\frac{y^2}{b^2}=z$

   双曲抛物面（马鞍面）：$\frac{x^2}{a^2}-\frac{y^2}{b^2}=z$

### 2.2 线性变换与线性空间

1. 线性组合

   设$\boldsymbol\beta,\boldsymbol\alpha_1,\cdots,\boldsymbol\alpha_m$都是$n$维向量，若存在一组实数$\lambda_1,\cdots,\lambda_m$使得

   $$\boldsymbol\beta=\lambda_1\boldsymbol\alpha_1+\cdots+\lambda_m\boldsymbol\alpha_m$$

   则称向量$\boldsymbol\beta$可由$\boldsymbol\alpha_1,\cdots,\boldsymbol\alpha_m$线性表示，或称向量$\boldsymbol\beta$是向量组$\boldsymbol\alpha_1,\cdots,\boldsymbol\alpha_m$的线性组合。

2. 线性相关

   设有$n$维向量组$\boldsymbol\alpha_1,\cdots,\boldsymbol\alpha_m$，若存在一组不全为零的实数$\lambda_1,\cdots,\lambda_m$使得

   $$\lambda_1\boldsymbol\alpha_1+\cdots+\lambda_m\boldsymbol\alpha_m=\boldsymbol{0}$$

   则称向量组$\boldsymbol\alpha_1,\cdots,\boldsymbol\alpha_m$线性相关；否则称它们线性无关

   线性相关的推论

   $n$个$n$维向量$\boldsymbol\alpha_1,\cdots,\boldsymbol\alpha_n$线性相关的充要条件是行列式$|\boldsymbol\alpha_1,\cdots,\boldsymbol\alpha_n|=0$。

   向量组部分线性相关则整体线性相关；向量组整体线性无关则部分线性相关。

   向量组$\boldsymbol\alpha_1,\cdots,\boldsymbol\alpha_m$线性相关的充要条件是存在一个向量可由其余$m-1$个向量线性表示。

   若有$m$个$n$维向量$\boldsymbol\alpha_1,\cdots,\boldsymbol\alpha_n$且$m>n$，则该向量组线性相关。

   若向量组$\boldsymbol\alpha_1,\cdots,\boldsymbol\alpha_m$线性无关，且添加$\boldsymbol\beta$后线性相关，则$\boldsymbol\beta$可由向量组$\boldsymbol\alpha_1,\cdots,\boldsymbol\alpha_m$线性表示，且表示法唯一。

3. 等价向量组

   设有两个$n$维向量组

   $$A:\boldsymbol\alpha_1,\cdots,\boldsymbol\alpha_r\quad B:\boldsymbol\beta_1\cdots,\boldsymbol\beta_s$$

   如果$A$中的每个向量组都能由向量组$B$线性表示，则称向量组$A$能由向量组$B$线性表示。如果向量组$A,B$能够相互线性表示，则称向量组$A$与$B$等价。

   大数定理：若$A$可由$B$线性表示，且向量组$A$线性无关，则$r\le s$。

4. 极大线性无关组

   若一个向量组$A$中的部分组$\boldsymbol\alpha_1,\cdots,\boldsymbol\alpha_r$满足下列两个条件：$\boldsymbol\alpha_1,\cdots,\boldsymbol\alpha_r$线性无关；向量组$A$中的任一向量都可由$\boldsymbol\alpha_1,\cdots,\boldsymbol\alpha_r$线性表示，则称$\boldsymbol\alpha_1,\cdots,\boldsymbol\alpha_r$为向量组$A$的一个极大线性无关组。

   向量组与它的任一极大线性无关组等价。

5. 向量组的秩

   向量组$A$的极大线性无关组所含向量的个数，称为该向量组的秩，记作$R(A)$。

   若向量组$A$可由向量组$B$线性表示，则$R(A)\le R(B)$，等价向量组有相同的秩。

   矩阵的秩可看作是矩阵各行组成行向量组的秩，也可以看作是矩阵各列组成列向量组的秩。

6. 齐次线性方程组的基础解系

   设向量$\boldsymbol\xi_1,\cdots,\boldsymbol\xi_t$是齐次线性方程组$\boldsymbol{A}\boldsymbol{X}=\boldsymbol{0}$的一组解，如果该向量组线性无关，且可以线性表示方程组的任意一个解，则称向量组$\boldsymbol\xi_1,\cdots,\boldsymbol\xi_t$是齐次线性方程组$\boldsymbol{A}\boldsymbol{X}=\boldsymbol{0}$的一个基础解系。

   若$\boldsymbol\xi_1,\cdots,\boldsymbol\xi_t$是$\boldsymbol{A}\boldsymbol{X}=\boldsymbol{0}$的解，则$k_1\boldsymbol\xi_1+\cdots+k_t\boldsymbol\xi_t$也是$\boldsymbol{A}\boldsymbol{X}=\boldsymbol{0}$的解。

7. 非齐次方程组的解

   若$\boldsymbol\xi$是$\boldsymbol{A}\boldsymbol{X}=\boldsymbol{0}$的解，$\boldsymbol{\eta}$是$\boldsymbol{A}\boldsymbol{X}=\boldsymbol{b}$的解，则$\boldsymbol\xi+\boldsymbol{\eta}$是$\boldsymbol{A}\boldsymbol{X}=\boldsymbol{b}$的解。

   若$\boldsymbol{\eta}_1,\boldsymbol{\eta}_2$是$\boldsymbol{A}\boldsymbol{X}=\boldsymbol{b}$的解，则$\boldsymbol{\eta}_1-\boldsymbol{\eta}_2$是$\boldsymbol{A}\boldsymbol{X}=\boldsymbol{0}$的解。

   若$\boldsymbol{\eta}_1,\cdots,\boldsymbol{\eta}_t$是$\boldsymbol{A}\boldsymbol{X}=\boldsymbol{b}$的解，则$\frac 1t(\boldsymbol{\eta}_1+\cdots+\boldsymbol{\eta}_t)$是$\boldsymbol{A}\boldsymbol{X}=\boldsymbol{b}$的解。

8. 线性方程组相关定理

   线性方程组$\boldsymbol{A}\boldsymbol{X}=\boldsymbol{b}$有解的充要条件是$R(\boldsymbol{A})=R(\boldsymbol{A},\boldsymbol{b})$。

   若$R(\boldsymbol{A},\boldsymbol{b})=R(\boldsymbol{A})=r$，$\boldsymbol{A}$的列数为$n$，则方程组$\boldsymbol{A}\boldsymbol{X}=\boldsymbol{b}$在$r=n$时有唯一解，$r<n$时有无穷多解。

   设$\boldsymbol{A}_{m\times n}$秩为$r$，若$r<n$，则$\boldsymbol{A}\boldsymbol{X}=\boldsymbol{0}$有基础解系，且基础解系所含向量个数为$n-r$。

   设$\boldsymbol\xi_1,\cdots,\boldsymbol\xi_{n-r}$是$\boldsymbol{A}\boldsymbol{X}=\boldsymbol{0}$的一个基础解系，则$\boldsymbol{A}\boldsymbol{X}=\boldsymbol{0}$的通解为

   $$\boldsymbol{X}=k_1\boldsymbol\xi_1+\cdots+k_{n-r}\boldsymbol\xi_{n-r}$$

   设$\boldsymbol\xi_1,\cdots,\boldsymbol\xi_{n-r}$是$\boldsymbol{A}\boldsymbol{X}=\boldsymbol{0}$的一个基础解系，$\boldsymbol{\eta}$是$\boldsymbol{A}\boldsymbol{X}=\boldsymbol{b}$的一个特解，则$\boldsymbol{A}\boldsymbol{X}=\boldsymbol{b}$的通解为

   $$\boldsymbol{X}=\boldsymbol{\eta}+k_1\boldsymbol\xi_1+\cdots+k_{n-r}\boldsymbol\xi_{n-r}$$

   $Cramer$法则：若$|\boldsymbol{A}_{n\times n}|\ne0$，则方程组$\boldsymbol{A}\boldsymbol{X}=\boldsymbol{b}$有唯一解$x_j=\frac{|\boldsymbol{A}_j|}{|\boldsymbol{A}|}(j=1,\cdots,n)$。

   方程组$\boldsymbol{A}_{m\times n}\boldsymbol{X}=\boldsymbol{0}$有非零解$\Leftrightarrow R(\boldsymbol{A})<n$。

9. 线性空间

   若对于非空集合$V$和数域$F$，对任意$\boldsymbol{a},\boldsymbol{b},\boldsymbol{c}\in V,\lambda,\mu\in F$满足以下八条性质，则称$V$是一个线性空间

   $$\begin{aligned}
     &(1)\boldsymbol{a}+\boldsymbol{0}=\boldsymbol{a}\\
     &(2)\boldsymbol{a}+(-\boldsymbol{a})=\boldsymbol{0}\\
     &(3)1\cdot\boldsymbol{a}=\boldsymbol{a}\\
     &(4)\boldsymbol{a}+\boldsymbol{b}=\boldsymbol{b}+\boldsymbol{a}\\
     &(5)\boldsymbol{a}+(\boldsymbol{b}+\boldsymbol{c})=(\boldsymbol{a}+\boldsymbol{b})+\boldsymbol{c}\\
     &(6)(\lambda\mu)\boldsymbol{a}=\lambda(\mu\boldsymbol{a})\\
     &(7)(\lambda+\mu)\boldsymbol{a}=\lambda\boldsymbol{a}+\mu\boldsymbol{a}\\
     &(8)\lambda(\boldsymbol{a}+\boldsymbol{b})=\lambda\boldsymbol{a}+\lambda\boldsymbol{b}
     \end{aligned}$$

10. 线性空间的基与坐标

    若向量组$\boldsymbol\varepsilon_1,\cdots,\boldsymbol\varepsilon_n$线性无关，且能线性表示线性空间$V$中的所有向量，则称为线性空间$V$的一组基。

    若$V$中的向量$\boldsymbol\alpha=a_1\boldsymbol\varepsilon_1+\cdots+a_n\boldsymbol\varepsilon_n=\begin{bmatrix}\boldsymbol\varepsilon_1,\cdots,\boldsymbol\varepsilon_n\end{bmatrix}\begin{bmatrix}a_1\\\vdots\\a_n\end{bmatrix}$，则称$\begin{bmatrix}a_1\\\vdots\\a_n\end{bmatrix}$为$\boldsymbol\alpha$在基$\boldsymbol\varepsilon_1,\cdots,\boldsymbol\varepsilon_n$下的坐标。

11. 过渡矩阵与坐标变换公式

    若两组基$\boldsymbol{S}=\begin{bmatrix}\boldsymbol\varepsilon_1,\cdots,\boldsymbol\varepsilon_n\end{bmatrix},\boldsymbol{T}=\begin{bmatrix}\boldsymbol{\eta}_1,\cdots,\boldsymbol{\eta}_n\end{bmatrix}$满足基变换公式$\boldsymbol{T}=\boldsymbol{S}\boldsymbol{P}$，则称$\boldsymbol{P}$是从$\boldsymbol{S}$到$\boldsymbol{T}$的过渡矩阵。

    设向量$\boldsymbol\alpha$在$\boldsymbol{S},\boldsymbol{T}$下的坐标分别为$\boldsymbol{X},\boldsymbol{Y}$，则满足坐标变换公式$\boldsymbol{X}=\boldsymbol{P}\boldsymbol{Y}$。

12. 线性变换矩阵

    对于一组基$\boldsymbol\xi_1,\cdots,\boldsymbol\xi_n$，若存在矩阵$A$使得线性变换$\sigma$满足$\sigma(\boldsymbol\xi_1,\cdots,\boldsymbol\xi_n)=(\boldsymbol\xi_1,\cdots,\boldsymbol\xi_n)\boldsymbol{A}$，则称矩阵$\boldsymbol{A}$为线性变换$\sigma$在基$\boldsymbol\xi_1,\cdots,\boldsymbol\xi_n$下所对应的矩阵。

    若线性空间$V$的线性变换$\sigma$在两组基$\boldsymbol\xi_1,\cdots,\boldsymbol\xi_n$以及$\boldsymbol{\eta}_1,\cdots,\boldsymbol{\eta}_n$下对应的矩阵分别为$\boldsymbol{A},\boldsymbol{B}$，$\boldsymbol\xi_1,\cdots,\boldsymbol\xi_n$到$\boldsymbol{\eta}_1,\cdots,\boldsymbol{\eta}_n$的过渡矩阵为$\boldsymbol{P}$，则有$\boldsymbol{B}=\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}$。

13. 解空间

    $\boldsymbol{A}\boldsymbol{X}=\boldsymbol{0}$的解空间记为$V_A$，其维数$\dim V_A=n-R(\boldsymbol{A})$

14. 维数公式

    $$\dim(W_1+W_2)=\dim W_1+\dim W_2-\dim (W_1\cap W_2)$$

    其中$W_1+W_2=\{w_1+w_2:w_1\in W_1,w_2\in W_2\}$

### 2.3 矩阵的行列式与代数运算

1. 行列式的定义

   定义逆序数$\tau(i_1\cdots i_n)$为排序$i_1\cdots i_n$中满足$(p-q)(i_p-i_q)<0$所有实数对$(i_p,i_q)$的数目，其中$(i_p,i_q)$ 称为一个逆序。

   定义$\delta(i_1\cdots i_n)=(-1)^{\tau(i_1\cdots i_n)}$，从而可以定义行列式

   $$\det \boldsymbol{A}=\begin{vmatrix}a_{11}&\cdots&a_{1n}\\\vdots&\ddots&\vdots\\a_{n1}&\cdots&a_{nn}\end{vmatrix}=\sum_{(i_1\cdots i_n)}\delta(i_1\cdots i_n)a_{i_1}\cdots a_{i_n}$$

2. 余子式和代数余子式

   行列式中去掉第$i$行和第$j$列得到的行列式称为余子式，记作$M_{ij}$。

   代数余子式需要考虑位置关系：$A_{ij}=(-1)^{i+j}M_{ij}$。

3. 行列式展开定理

   $$\sum_{i=1}^na_{ik}A_{ij}=\begin{cases}0(k\ne j)\\|A|(k=j)\end{cases}或\sum_{j=1}^na_{kj}A_{ij}=\begin{cases}0(k\ne i)\\|A|(k=j)\end{cases}$$

4. 行列式运算性质

   $$\begin{aligned}
     &(1)\det(a_1,\cdots,b+c,\cdots,a_n)=\det(a_1,\cdots,b,\cdots,a_n)+\det(a_1,\cdots,c,\cdots,a_n)\\
     &(2)\det(a_1,\cdots,\lambda a_i,\cdots,a_n)=\lambda\det(a_1,\cdots,a_i,\cdots,a_n)\\
     &(3)\det(a_1,\cdots,a_i,\cdots,a_j,\cdots,a_n)=-\det(a_1,\cdots,a_j,\cdots,a_i,\cdots,a_n)\\
     &(4)\det(a_1,\cdots,a_i,\cdots,a_j,\cdots,a_n)=0,若a_i=\lambda a_j\\
     &(5)\det(a_1,\cdots,a_i,\cdots,a_j,\cdots,a_n)=0,若a_i=\boldsymbol{0}\\
     &(6)\det(a_1,\cdots,a_i,\cdots,a_j,\cdots,a_n)=\det(a_1,\cdots,a_i+\lambda a_j,\cdots,a_j,\cdots,a_n)\\
     &(7)\det(a_1,,\cdots,a_n)=\det(a_1,,\cdots,a_n)^T
     \end{aligned}$$

5. 伴随矩阵

   将原矩阵对应元素用对应代数余子式替代，得到的矩阵进行转置后得到伴随矩阵

   $$若\boldsymbol{A}=\begin{bmatrix}a_{11}&\cdots&a_{1n}\\\vdots&\ddots&\vdots\\a_{n1}&\cdots&a_{nn}\end{bmatrix},则\boldsymbol{A}^*=\begin{bmatrix}A_{11}&\cdots&A_{n1}\\\vdots&\ddots&\vdots\\A_{1n}&\cdots&A_{nn}\end{bmatrix}$$

   两个计算要点：乘以位置系数$(-1)^{i+j}$，取转置。

6. 逆矩阵

   对于矩阵$\boldsymbol{A}$ ，若存在$\boldsymbol{B}$使得$\boldsymbol{A}\boldsymbol{B}=\boldsymbol{B}\boldsymbol{A}=\boldsymbol{E}$，$\boldsymbol{E}$为单位阵，则称$\boldsymbol{B}$为$\boldsymbol{A}$的逆矩阵。

   设$\boldsymbol{A},\boldsymbol{B}$均为$n$阶可逆矩阵，$k$是非零常数，则

   $$(\boldsymbol{A}\boldsymbol{B})^{-1}=\boldsymbol{B}^{-1}\boldsymbol{A}^{-1},\quad(k\boldsymbol{A})^{-1}=\frac 1k \boldsymbol{A}^{-1},\quad(\boldsymbol{A}^T)^{-1}=(\boldsymbol{A}^{-1})^T$$

7. 抽象矩阵的行列式计算

   $$\begin{aligned}
     &(1)|k\boldsymbol{A}|=k^n|\boldsymbol{A}|,其中k为常数,\boldsymbol{A}为n阶矩阵\\
     &(2)\begin{vmatrix}\boldsymbol{A}&\boldsymbol{O}\\\boldsymbol{C}&\boldsymbol{B}\end{vmatrix}=\begin{vmatrix}\boldsymbol{A}&\boldsymbol{D}\\\boldsymbol{O}&\boldsymbol{B}\end{vmatrix}=|\boldsymbol{A}||\boldsymbol{B}|,其中\boldsymbol{A}和\boldsymbol{B}
     均为方阵,可以不同阶\\
     &(3)\begin{vmatrix}\boldsymbol{O}&\boldsymbol{A}\\\boldsymbol{B}&\boldsymbol{C}\end{vmatrix}=\begin{vmatrix}\boldsymbol{D}&\boldsymbol{A}\\\boldsymbol{B}&\boldsymbol{O}\end{vmatrix}=(-1)^{mn}|\boldsymbol{A}||\boldsymbol{B}|,其中\boldsymbol{A}为m阶方阵,\boldsymbol{B}为n阶方阵\\
     &(4)\boldsymbol{A}\boldsymbol{A}^*=\boldsymbol{A}^*\boldsymbol{A}=|\boldsymbol{A}|\boldsymbol{E}\\
     &(5)|\boldsymbol{A}^*|=|\boldsymbol{A}|^{n-1},其中\boldsymbol{A}为n阶方阵\\
     &(6)(\boldsymbol{A}^*)^*=|\boldsymbol{A}|^{n-2}\boldsymbol{A},其中\boldsymbol{A}为n阶方阵\\
     &(7)|\boldsymbol{A}^{-1}|=|\boldsymbol{A}|^{-1},若\boldsymbol{A}可逆
     \end{aligned}$$

8. 矩阵的加法和数乘

   若$\boldsymbol{A}=(a_{ij})_{m\times n},\boldsymbol{B}=(b_{ij})_{m\times n}$，则$\boldsymbol{A}\pm\boldsymbol{B}=(a_{ij}\pm b_{ij})_{m\times n}$。

   若$\boldsymbol{A}=(a_{ij})_{m\times n}$，若$\lambda\boldsymbol{A}=(\lambda a_{ij})_{m\times n}$。

9. 矩阵的乘法

   若$\boldsymbol{A}=(a_{ij})_{m\times s},\boldsymbol{B}=(b_ij)_{s\times n}$，则$\boldsymbol{A}\boldsymbol{B}=\boldsymbol{C}$，其中$\boldsymbol{C}=(c_{ij})_{m\times n},c_{ij}=\sum\limits_{k=1}^sa_{ik}b_{kj}$。

10. 矩阵的转置运算

    $$\begin{aligned}
      &(1)(\boldsymbol{A}^T)^T=\boldsymbol{A}\\
      &(2)(\boldsymbol{A}+\boldsymbol{B})^T=\boldsymbol{A}^T+\boldsymbol{B}^T\\
      &(3)(\lambda\boldsymbol{A})^T=\lambda \boldsymbol{A}^T\\
      &(4)(\boldsymbol{A}\boldsymbol{B})^T=\boldsymbol{B}^T\boldsymbol{A}^T
      \end{aligned}$$

    设$\boldsymbol{A}$为$n$阶矩阵，若$\boldsymbol{A}^T=\boldsymbol{A}$则称$\boldsymbol{A}$为对称矩阵，若$\boldsymbol{A}^T=-\boldsymbol{A}$则称$\boldsymbol{A}$为反对称矩阵。

11. 初等方阵与初等变换

    对矩阵的以下三种变换称为初等变换：

    （1）交换矩阵的任意两行（列）；

    （2）用一个非零数去乘矩阵某一行（列）的所有元素；

    （3）将一行（列）元素任意倍加到另一行（列）去。

    由单位矩阵经过一次初等变换得到的矩阵称为初等方阵。

    左乘初等矩阵相当于对原始矩阵进行行变换，右乘初等矩阵相当于对原始矩阵进行列变换。

    三种变换均不改变矩阵的秩，但如果原矩阵为方阵，只有第三种变换不改变矩阵的行列式。

12. 矩阵的等价

    设$\boldsymbol{A},\boldsymbol{B}$均为$m\times n$矩阵，若$\boldsymbol{A}$可以经过有限次初等变换化为$\boldsymbol{B}$，则称$\boldsymbol{A}$和$\boldsymbol{B}$等价。

    $\boldsymbol{A}$和$\boldsymbol{B}$等价的充要条件是：存在$m$阶可逆阵$\boldsymbol{P}$和$n$阶可逆阵$\boldsymbol{Q}$，使得$\boldsymbol{P}\boldsymbol{A}\boldsymbol{Q}=\boldsymbol{B}$。

13. $n$阶方阵的秩相关结论

    $$\begin{aligned}
      &(1)R(\boldsymbol{A})=n\Leftrightarrow R(\boldsymbol{A}^*)=n\\
      &(2)R(\boldsymbol{A})=n-1\Leftrightarrow R(\boldsymbol{A}^*)=1\\
      &(3)R(\boldsymbol{A})<n-1\Leftrightarrow R(\boldsymbol{A}^*)=0
      \end{aligned}$$

14. 矩阵秩相关的其他结论

    $$\begin{aligned}
      &(1)R(\boldsymbol{A}+\boldsymbol{B})\le R[(\boldsymbol{A},\boldsymbol{B})]\le R(\boldsymbol{A})+R(\boldsymbol{B})\\
      &(2)R(\boldsymbol{A}\boldsymbol{B})\le\min\{R(\boldsymbol{A}),R(\boldsymbol{B})\}\\
      &(3)若\boldsymbol{A}_{m\times n}\boldsymbol{B}_{n\times p}=\boldsymbol{O}_{n\times p},则R(\boldsymbol{A})+R(\boldsymbol{B})\le n
      \end{aligned}$$

15. 矩阵的标准形

    设矩阵$\boldsymbol{A}$是秩为$r$的$m\times n$矩阵，则存在$m$阶可逆矩阵$\boldsymbol{P}$和$n$阶可逆矩阵$\boldsymbol{Q}$，使得

    $$\boldsymbol{P}\boldsymbol{A}\boldsymbol{Q}=\begin{bmatrix}\boldsymbol{E}_r&\boldsymbol{O}\\\boldsymbol{O}&\boldsymbol{O}\end{bmatrix}_{m\times n}$$

    称$\begin{bmatrix}\boldsymbol{E}_r&\boldsymbol{O}\\\boldsymbol{O}&\boldsymbol{O}\end{bmatrix}_{m\times n}$为矩阵$\boldsymbol{A}$的标准形。

### 2.4 矩阵特征值分解与二次型

1. 特征值与特征向量

   设$\boldsymbol{A}$是$n$阶矩阵，若对实数$\lambda$存在非零向量$\boldsymbol\alpha$，使得$\boldsymbol{A}\boldsymbol\alpha=\lambda\boldsymbol\alpha$，则称$\lambda$是$\boldsymbol{A}$的特征值，$\boldsymbol\alpha$是$\boldsymbol{A}$的对应特征值$\lambda$的特征向量。称$|\lambda\boldsymbol{E}-\boldsymbol{A}|$为$\boldsymbol{A}$的特征多项式，$|\lambda\boldsymbol{E}-\boldsymbol{A}|=0$的全部解即为$\boldsymbol{A}$的全部特征值。

   $\boldsymbol{A}$对角线元素之和称为迹，记作$tr(\boldsymbol{A})$，且$tr(\boldsymbol{A})=\lambda_1+\cdots+\lambda_n$。

2. 矩阵的相似

   设$\boldsymbol{A},\boldsymbol{B}$为$n$阶矩阵，若存在可逆矩阵$\boldsymbol{P}$，使得$\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{B}$，则称矩阵$\boldsymbol{A}$与$\boldsymbol{B}$相似。

   若$\boldsymbol{A}$与$\boldsymbol{B}$相似，则

   $$\begin{aligned}
     &(1)|\lambda\boldsymbol{E}-\boldsymbol{A}|=|\lambda\boldsymbol{E}-\boldsymbol{B}|\\
     &(2)|\boldsymbol{A}|=|\boldsymbol{B}|,tr(\boldsymbol{A})=tr(\boldsymbol{B}),R(\boldsymbol{A})=R(\boldsymbol{B})\\
     &(3)\boldsymbol{A}^T与\boldsymbol{B}^T相似,\boldsymbol{A}^m与\boldsymbol{B}^m相似,f(\boldsymbol{A})与f(\boldsymbol{B})相似\\
     &(4)当\boldsymbol{A}可逆时,\boldsymbol{A}^{-1}与\boldsymbol{B}^{-1}相似,\boldsymbol{A}^*与\boldsymbol{B}^*相似
     \end{aligned}$$

3. 矩阵可相似对角化的第一种充要条件

   $$n阶矩阵\boldsymbol{A}可相似对角化的充要条件是\boldsymbol{A}有n个线性无关的特征向量$$

   推论：若$n$阶矩阵$\boldsymbol{A}$有$n$个不同的特征值，则必可相似对角化，反之不成立。

4. 矩阵可相似对角化的第二种充要条件

   设$n$阶矩阵$\boldsymbol{A}$的不同特征值为$\lambda_1,\cdots,\lambda_s$，其重数分别为$r_1,\cdots.r_s$，且$\sum\limits_{i=1}^sr_i=n$，则$\boldsymbol{A}$可相似对角化的充要条件是对于每一个特征值$\lambda_i$有$R(\lambda_i\boldsymbol{E}-\boldsymbol{A})=n-r_i$，即对应于特征值极大线性无关的特征向量的个数恰好等于其重数$r_i(i=1,\cdots,s)$。

5. 相似对角化的计算方法

   $$\begin{aligned}
     &(1)计算矩阵\boldsymbol{A}的特征值\lambda_1,\cdots,\lambda_n\\
     &(2)计算对应特征值的对应特征向量\boldsymbol{p}_1,\cdots,\boldsymbol{p}_n\\
     &(3)记\boldsymbol{P}=[\boldsymbol{p}_1,\cdots,\boldsymbol{p}_n],则\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\begin{bmatrix}\lambda_1&&\\&\ddots\\&&\lambda_n\end{bmatrix}
     \end{aligned}$$

6. 向量的内积与正交性

   若$\boldsymbol\alpha=(a_1,\cdots,a_n)^T,\boldsymbol\beta=(b_1,\cdots,b_n)^T$，则记$\boldsymbol\alpha$与$\boldsymbol\beta$的内积为：

   $$(\boldsymbol\alpha,\boldsymbol\beta)=\boldsymbol\alpha^T\boldsymbol\beta=\boldsymbol\beta^T\boldsymbol\alpha=a_1b_1+\cdots+a_nb_n$$

   若$(\boldsymbol\alpha,\boldsymbol\beta)=0$，则称$\boldsymbol\alpha$与$\boldsymbol\beta$正交。

7. $Schimidt$正交化方法

   若有$n$个线性无关的向量$\boldsymbol\alpha_1,\cdots,\boldsymbol\alpha_n$，则过程分为正交化和单位化

   正交化过程

   $$\boldsymbol\beta_k=\boldsymbol\alpha_k-\sum_{i=1}^{k-1}\frac{(\boldsymbol\beta_i,\boldsymbol\alpha_k)}{(\boldsymbol\beta_i,\boldsymbol\beta_i)}\boldsymbol\beta_i,\quad k=1,\cdots,n$$

   单位化过程

   $$\boldsymbol{\eta}_k=\frac{\boldsymbol\beta_k}{||\boldsymbol\beta_k||},\quad k=1,\cdots,n$$

   从而得到一组单位正交向量$\boldsymbol{\eta}_1\cdots,\boldsymbol{\eta}_n$。

8. 正交矩阵

   若$\boldsymbol{A}\boldsymbol{A}^T=\boldsymbol{E}$或者$\boldsymbol{A}^T=\boldsymbol{A}^{-1}$，则称矩阵$\boldsymbol{A}$为正交矩阵。

9. 实对称矩阵的正交相似对角化

   （1）实对称矩阵的特征值均为实数；

   （2）实对称矩阵对应不同特征值的特征向量相互正交；

   （3）实对称矩阵必定可以相似对角化；

   （4）若$\boldsymbol{A}$是$n$阶实对称矩阵，且特征值为$\lambda_1,\cdots,\lambda_n$，则存在正交矩阵$\boldsymbol{Q}$，使得

   $$\boldsymbol{Q}^T\boldsymbol{A}\boldsymbol{Q}=\begin{bmatrix}\lambda_1&&\\&\ddots\\&&\lambda_n\end{bmatrix}$$

   （5）若$\boldsymbol{A}$和$\boldsymbol{B}$均为$n$阶实对称矩阵，则$\boldsymbol{A}$和$\boldsymbol{B}$相似的充要条件是$\boldsymbol{A}$和$\boldsymbol{B}$有相同的特征值。

10. 二次型

    $n$个变量$x_1,\cdots,x_n$的二次齐次实系数函数

    $$f(x_1,\cdots,x_n)=\sum_{i=1}^na_{ii}x_i^2+\sum_{i<j}^n2a_{ij}x_ix_j$$

    称为$n$元实二次型，可以表示为$\boldsymbol{X}^T\boldsymbol{A}\boldsymbol{X}$，其中

    $$\boldsymbol{A}=\begin{bmatrix}a_{11}&\cdots&a_{1n}\\\vdots&\ddots&\vdots\\a_{n1}&\cdots&a_{nn}\end{bmatrix},\boldsymbol{X}=\begin{bmatrix}x_1\\\vdots\\x_n\end{bmatrix}$$

    且$a_{ij}=a_{ji}(i,j=1,\cdots,n)$。

11. 二次型的标准形与规范性

    若存在可逆矩阵$\boldsymbol{C}$以及$\boldsymbol{X}=\boldsymbol{C}\boldsymbol{Y}$，使得

    $$f=\boldsymbol{X}^T\boldsymbol{A}\boldsymbol{X}=\boldsymbol{Y}^T\begin{bmatrix}k_1&&\\&\ddots&\\&&k_n\end{bmatrix}\boldsymbol{Y}$$

    则称$f=k_1y_1^2+\cdots+k_ny_n^2$为$f$的标准形

    进一步，根据$k_i$的正负号可写为$f=z_1^2+\cdots+z_p^2-z_{p+1}^2-\cdots-z_r^2$的形式，称为$f$的规范形。

    其中$r$是$f$的秩，$p$为$f$的正惯性指数，$r-p$为$f$的负惯性指数。

12. 矩阵的相合

    设$\boldsymbol{A}$和$\boldsymbol{B}$是$n$阶矩阵，若存在可逆矩阵$\boldsymbol{P}$，使得$\boldsymbol{P}^T\boldsymbol{A}\boldsymbol{P}=\boldsymbol{B}$，则称$\boldsymbol{A}$与$\boldsymbol{B}$相合。

    任何实对称矩阵$\boldsymbol{A}$必和如下对角阵合同

    $$\Lambda=\begin{bmatrix}\boldsymbol{E}_p&&\\&-\boldsymbol{E}_{r-p}&\\&&\boldsymbol{O}\end{bmatrix}$$

13. 正定二次型与正定矩阵

    设$f=\boldsymbol{X}^T\boldsymbol{A}\boldsymbol{X}$为$n$元二次型，若对任意$n$维维非零向量$\boldsymbol\alpha$均有$\boldsymbol\alpha^T\boldsymbol{A}\boldsymbol\alpha>0$，则称$f$为正定二次型，同时称矩阵$\boldsymbol{A}$为正定矩阵。

    若$n$维矩阵$\boldsymbol{A}$是正定矩阵，则

    （1）$\boldsymbol{A}$是实对称矩阵；

    （2）$\boldsymbol{A}$正惯性指数为$n$，所有特征值均为正；

    （3）$\boldsymbol{A}$与单位阵合同；

    （4）$\boldsymbol{A}$的各阶顺序主子式大于零；

    （5）存在可逆矩阵$\boldsymbol{P}$使得$\boldsymbol{A}=\boldsymbol{P}^T\boldsymbol{P}$。

## 第三章 概率统计

### 3.1 概率与分布

1. 事件及其运算

   和事件：$A+B=A\cup B$

   积事件：$AB=A\cap B$

   差事件：$A-B=A\cap\overline{B}$

2. 事件的概率及其运算

   $A$与$B$对立（$B=\overline{A}$）：$P(A+B)=P(A)+P(B)=1,P(AB)=0$

   $A$与$B$互斥（互不相容）：$P(A+B)=P(A)+P(B),P(AB)=0$

   $A$与$B$独立：$P(A)=P(A|B)=P(A|\overline{B}),P(AB)=P(A)P(B)$

3. 概率模型

   古典概型、几何概型：强调概率相等性。

4. 概率的加法公式（容斥原理）

   两个事件：$P(A+B)=P(A)+P(B)-P(AB)$

   三个事件：$P(A+B+C)=P(A)+P(B)+P(C)-P(AB)-P(BC)-P(CA)+P(ABC)$

5. 条件概率

   若事件$B$的概率非零，则在$B$发生的条件下，$A$发生的概率称为条件概率，记作

   $$P(A|B)=\frac{P(AB)}{P(B)}$$

6. 乘法公式

   若$P(B)>0$，则$P(AB)=P(B)P(A|B)$

   若$P(A_1\cdots A_{n-1})>0$，则$P(A_1\cdots A_n)=P(A_1)P(A_2|A_1)\cdots P(A_n|A_1\cdots A_{n-1})$

7. 全概率公式

   若事件$B_1,\cdots,B_n$是样本空间或全事件集的一组划分，且$P(B_i)>0$，则

   $$P(A)=\sum_{i=1}^nP(AB_i)=\sum_{i=1}^nP(B_i)P(A|B_i)$$

   特别地

   $$P(A)=P(B)P(A|B)+P(\overline{B})P(A|\overline{B})$$

8. 贝叶斯公式

   若事件$B_1,\cdots,B_n$是样本空间或全事件集的一组划分，且$P(B_i)>0,P(A)>0$，则

   $$P(B_i|A)=\frac{P(AB_i)}{P(A)}=\frac{P(B_i)P(A|B_i)}{\sum\limits_{j=1}^nP(B_j)P(A|B_j)}$$

   更在意后验概率、关注前提条件的思维模式

9. 随机变量的分布函数

   给定随机变量$X$，对任意实数$x$，定义随机变量$X$的分布函数为：$F(x)=P(X\le x)$

   分布函数的基本性质：

   $(1)$单调不减，$F(x+t)\ge F(x),\forall t>0$

   $(2)$有界，$0\le F(x)\le1,F(-\infty)=0,F(+\infty)=1$

   $(3)$右连续，$\lim\limits_{t\to 0^+}F(x+t)=F(x)$

   $(4)P(a<x\le b)=F(b)-F(a)$

10. 离散随机变量的分布列（分布律）

    设离散随机变量$X$的可能取值为：$x_1,x_2,\cdots,x_n,\cdots$，则称$p_i=P(X=x_i),i=1,2,\cdots$为$X$的分布列

    满足非负性$p_i\ge0$和正则性$\sum p_i=1$（或称为概率的归一化条件）

11. 连续随机变量的概率密度函数

    设随机变量$X$的分布函数为$F(x)$，若存在非负可积函数$p(x)$，使得$F(x)=\int_{-\infty}^xp(x)dx$，则

    称$X$是连续随机变量，称$p(x)$为概率密度函数，简称密度函数。

    满足非负性$p(x)\ge0$和正则性$\int_{-\infty}^{+\infty}p(x)dx=1$（或称为概率的归一化条件）

    对于连续随机变量，$P(X=x)=0$，其概率密度函数可以定义为

    $$p(x)=\begin{cases}F'(x),&F在x处可导\\0,&F在x处不可导\end{cases}$$

    特别地，$F$处的不可导点处的$p(x)$也可以定义为其他有限值，因为不改变$p(x)$的积分值

12. 离散随机变量的数学期望

    设离散随机变量$X$的分布列为$P(X=x_n)=p_n,n=1,2,\cdots$，若级数$\sum\limits_{i=1}^{\infty}x_ip_i$绝对收敛，则称该级数为$X$的数学期望，记为

    $$E(X)=\sum\limits_{i=1}^{\infty}x_ip_i$$

13. 连续变量的数学期望

    设连续随机变量$X$的密度函数为$p(x)$，若积分$\int_{-\infty}^{+\infty}xp(x)dx$绝对收敛，则称该积分为$X$的数学期望，记为

    $$E(X)=\int_{-\infty}^{+\infty}xp(x)dx$$

14. 随机变量函数的期望

    设$Y=g(X)$是随机变量$X$的函数，若$E(g(X))$存在，则

    $$E(g(X))=\sum_{i=1}^\infty g(x_i)P(X=x_i)或者E(g(X))=\int_{-\infty}^{+\infty}g(x)p(x)dx$$

15. 数学期望的性质

    $$\begin{aligned}
      (1)&E(c)=c\\
      (2)&E(aX)=aE(X)\\
      (3)&E(g_1(X)+g_2(X))=E(g_1(X))+E(g_2(X))
      \end{aligned}$$

    第三条性质意味着——独立性不影响随机变量和的期望展开计算

16. 随机变量的方差

    给定随机变量$X$，若$E(X-E(X))^2$存在，则称$E(X-E(X))^2$为$X$的方差，记为

    $$Var(X)=D(X)=E(X-E(X))^2$$

    方差具有如下性质

    $$\begin{aligned}
      (1)&Var(X)=E(X^2)-[E(X)]^2\\
      (2)&Var(c)=0\\
      (3)&Var(aX+b)=a^2Var(X)
      \end{aligned}$$

17. 随机变量的标准化

    设$Var(X)>0$，令

    $$Y=\frac{X-EX}{\sqrt{Var(X)}}$$

    则有$E(Y)=0,Var(Y)=1$，称$Y$为$X$的标准化。

18. 二项分布

    $n$重伯努利试验中成功的次数记作$X$，则$X$满足分布律：

    $$P(X=k)=\begin{pmatrix}n\\k\end{pmatrix}p^k(1-p)^{n-k},k=0,1,\cdots,n$$

    记作$X\sim B(n,p)$，其期望和方差分别为：$E(X)=np,Var(X)=np(1-p)$

19. 泊松分布

    若随机变量$X$的分布律满足：

    $$P(X=k)=\frac{\lambda^k}{k!}e^{-\lambda},k=0,1,2,\cdots$$

    则称$X$服从参数为$\lambda$的泊松分布，记为$X\sim P(\lambda)$，其期望和方差分别为：$E(X)=\lambda,Var(X)=\lambda$

20. 超几何分布

    $N$个产品中有$M$个不合格品，从中抽取$n$个，不合格品的个数为$X$，则$X$满足分布律：

    $$P(X=k)=\frac{\begin{pmatrix}M\\k\end{pmatrix}\begin{pmatrix}N-M\\n-k\end{pmatrix}}{\begin{pmatrix}N\\n\end{pmatrix}}$$

    记作$X\sim h(n,N,M)$

21. 几何分布

    若随机变量$X$为独立重复伯努利试验中首次成功时的试验次数，则$X$满足分布律：

    $$P(X=k)=(1-p)^{k-1}p,k=1,2,\cdots$$

    记作$X\sim Ge(p)$，其期望和方差分别为：$E(X)=1/p,Var(X)=(1-p)/p^2$

    几何分布具有无记忆性，即

    $$P(X>m+n|X>m)=P(X>n)$$

22. 负二项分布

    若随机变量$X$为独立重复伯努利试验中第$r$次成功时的试验次数，则$X$满足分布律：

    $$P(X=k)=\begin{pmatrix}k-1\\r-1\end{pmatrix}(1-p)^{k-r}p^r,k=r,r+1,\cdots$$

    记为$X\sim Nb(r,p)$

    可以表示成$r$个独立同分布几何分布随机变量之和

23. 正态分布

    若随机变量$X$的概率密度函数为

    $$p(x)=\frac{1}{\sqrt{2\pi}\sigma}exp\{-\frac{(x-\mu)^2}{2\sigma^2}\}$$

    记作$X\sim N(\mu,\sigma^2)$，其期望和方差分别为：$E(X)=\mu,Var(X)=\sigma^2$

24. 标准正态分布

    若$X\sim N(0,1)$，则称$X$服从标准正态分布，其密度函数记为$\varphi(x)$，分布函数记为$\Phi(x)$

    标准正态分布函数满足：$\Phi(0)=1/2,\Phi(-x)=1-\Phi(x)$。

    若$P(X\le z_\alpha)=\Phi(z_\alpha)=\alpha$，则称$z_\alpha$为标准正态分布的$\alpha$分位点

25. 一般正态分布的标准化

    若$X\sim N(\mu,\sigma^2)$，则

    $$\frac{X-\mu}\sigma\sim N(0,1),F(x)=\Phi(\frac{x-\mu}\sigma)$$

26. 均匀分布

    若随机变量的概率密度函数满足

    $$p(x)=\begin{cases}1/(b-a),&a<x<b\\0,&otherwise\end{cases}$$

    则称$X$服从均匀分布，记作$X\sim U(a,b)$

    其期望和方差分别为$E(X)=(a+b)/2,Var(X)={(b-a)^2}/{12}$

27. 指数分布

    若随机变量的概率密度函数满足

    $$p(x)=\begin{cases}\lambda e^{-\lambda x},&x>0\\0,&x\le 0\end{cases}$$

    则称$X$服从指数分布，记作$X\sim Exp(\lambda),\lambda>0$

    其期望和方差分别为：$E(X)=1/\lambda,Var(X)=1/{\lambda^2}$

28. $\Gamma$分布

    若随机变量的概率密度函数满足

    $$p(x)=\frac{\lambda^\alpha}{\Gamma(\alpha)}x^{\alpha-1}e^{-\lambda x},x\ge0$$

    则称$X$服从$\Gamma$分布，记作$X\sim Ga(\alpha,\lambda),\alpha>0,\lambda>0$

    其期望为$E(X)=\alpha/\lambda$

    称$\Gamma(\alpha)=\int_0^{+\infty}x^{\alpha-1}e^{-x}dx$为$\Gamma$函数

    一些性质

    $$\begin{aligned}
      &(1)\Gamma(1)=1,\Gamma(\frac 12)=\sqrt\pi,\Gamma(n+1)=n!\\
      &(2)Ga(1,\lambda)=Exp(\lambda),Ga(\frac n2,\frac 12)=\chi^2(n)\\
      &(3)X\sim Ga(\alpha,\lambda)\Rightarrow kX\sim Ga(\alpha,\lambda/k)(k>0)
      \end{aligned}$$

29. $Beta$分布

    若随机变量的概率密度函数满足

    $$p(x)=\frac{1}{B(a,b)}x^{a-1}(1-x)^{b-1},0<x<1$$

    则称$X$服从$Beta$分布，记作$X\sim Be(a,b),a>0,b>0$

    其期望为$E(X)=a/(a+b)$

    称$B(a,b)=\int_0^1x^{a-1}(1-x)^{b-1}dx$为$Beta$函数

    一些性质

    $$\begin{aligned}
      (1)&B(a,b)=B(b,a)\\
      (2)&B(a,b)=\frac{\Gamma(a)\Gamma(b)}{\Gamma(a+b)}\\
      (3)&Be(1,1)=U(0,1)
      \end{aligned}$$

30. 离散随机变量函数的分布

    当$X$为离散随机变量时，$Y=g(X)$为离散随机变量

    将$g(x_i)$一一列出，再将相等的值合并即可

31. 连续随机变量函数的分布

    设$X$的概率密度函数为$p_X(x)$，$y=g(x)$是$x$的严格单调函数，且值域为$(a,b)$，则$y=g(x)$存在反函数$x=h(y)$，且$h(y)$连续可导，则$Y=g(X)$的密度函数为

    $$p_Y(y)=\begin{cases}p_X(h(y))|h'(y)|,&a<y<b\\0,&otherwise\end{cases}$$

32. 正态变量的线性不变性

    设$X\sim N(\mu,\sigma^2),a\ne0$，则$aX+b\sim N(a\mu+b,a^2\sigma^2)$

33. 各种分布随机数的产生

    若随机变量$X$的分布函数为$F_X(x)$，若$F_X(x)$连续且严格单调递增，则$Y=F_X(x)\sim U(0,1)$

34. $k$阶原点矩和中心距

    $k$阶原点矩：$\mu_k=E(X^k)$

    $k$阶中心矩：$v_k=E[X-E(X)]^k$

35. 变异系数

    称$C_V=\sqrt{Var{X}}/E(X)$为$X$的变异系数

36. 偏度系数

    设随机变量$X$的前三阶矩存在，则比值

    $$\beta_S=\frac{v_3}{v_2^{\frac 32}}=\frac{E(X-EX)^3}{[Var(X)]^{\frac 32}}$$

37. 峰度系数

    设随机变量$X$的前四阶矩存在，则比值

    $$\beta_k=\frac{v_4}{v_2^2}-3=\frac{E(X-EX)^4}{[Var(X)]^2}-3$$

38. 二维随机变量的联合分布

    给定随机变量$X$和$Y$，对任意实数$x$和$y$，称$F(x,y)=P(X\le x,Y\le y)$为$(X,Y)$的联合分布函数

    联合分布函数的性质

    $$\begin{aligned}
      (1)&F(x,y)关于x和y分别单调不减\\
      (2)&0\le F(x,y)\le 1,F(-\infty,y)=F(x,-\infty)=0,F(+\infty,+\infty)=1\\
      (3)&F(x,y)关于x和y分别右连续\\
      (4)&P(a<X\le b,c<Y\le d)=F(b,d)-D(b,c)-F(a,d)+F(a,c)\ge 0
      \end{aligned}$$

39. 二维离散随机变量

    若$(X,Y)$的可能取值为可列对，则称$(X,Y)$为二维离散随机变量，其分布列（分布律）为：

    $$p_{ij}=P(X=x_i,Y=y_j)\quad i,j=1,2,\cdots$$

    所有的$p_{ij}$满足非负性和归一化

40. 二维连续随机变量

    设二维随机变量$(X,Y)$的分布函数为$F(x,y)$，若存在非负可积函数$p(x,y)$，使得

    $$F(x,y)=\int_{-\infty}^x\int_{-\infty}^yp(u,v)dudv$$

    则称$(X,Y)$为二维连续随机变量，称$p(x,y)$为联合概率密度，满足非负性和归一化

    特别地

    $$P\{(X,Y)\in D\}=\iint\limits_Dp(x,y)dxdy$$

41. 边缘分布函数（边际分布函数）

    已知$(X,Y)$的联合分布函数为$F(x,y)$，则

    $X$的（边缘）分布函数为：$F_X(x)=F(x,+\infty)$

    $Y$的（边缘）分布函数为：$F_Y(y)=F(+\infty,y)$

42. 边缘分布律（边际分布列）

    已知$(X,Y)$的联合分布律为$p_{ij}=P(X=x_i,Y=y_j)$

    $X$的（边缘）分布律为：$p_i=P(X=x_i)=\sum\limits_{j=1}^\infty p_{ij}=p_{i\cdot}$

    $Y$的（边缘）分布律为：$p_j=P(Y=y_j)=\sum\limits_{i=1}^\infty p_{ij}=p_{\cdot j}$

43. 边缘密度函数（边际密度函数）

    已知$(X,Y)$的联合密度函数为$p(x,y)$，则

    $X$的（边缘）密度函数为：$p_X(x)=\int_{-\infty}^{+\infty}p(x,y)dy$

    $Y$的（边缘）密度函数为：$p_Y(y)=\int_{-\infty}^{+\infty}p(x,y)dx$

44. 随机变量的独立性

    若随机变量$X$和$Y$满足以下之一

    $$\begin{aligned}
      (1)&F(x,y)=F_X(x)F_Y(y)\\
      (2)&p_{ij}=p_ip_j\\
      (3)&p(x,y)=p_X(x)p_Y(y)
      \end{aligned}$$

    则称$X$与$Y$是独立的

    $X$与$Y$独立的本质应该回到概率的定义上：对任意实数$a,b,c,d$有

    $$P(a<X<b,c<Y<d)=P(a<X<b)P(c<Y<d)$$

    若$X$与$Y$是独立的，则$g(X)$与$h(Y)$也是独立的

45. 多维随机变量函数的分布

    已知$(X,Y)$的联合分布函数为$F(x,y)$，若$Z=\max(X,Y)$，则

    $$\begin{aligned}
      F_Z(z)&=P(\max(X,Y)\le z)\\
      &=P(X\le z且Y\le z)\\
      &=F(z,z)
      \end{aligned}$$

    若$Z=\min(X,Y)$，则

    $$\begin{aligned}
      F_Z(z)&=P(\min(X,Y)\le z)\\
      &=P(X\le z或Y\le z)\\
      &=1-P(X>z,Y>z)\\
      &=F(+\infty,z)+F(z,+\infty)-F(z,z)
      \end{aligned}$$

    $Z$的概率密度为$p_Z(z)=F_Z'(z)$

46. 连续场合的卷积公式

    设连续随机变量$X$与$Y$独立， 则$Z=X+Y$的密度函数为

    $$\begin{aligned}p_Z(z)&=\int_{-\infty}^{+\infty}p_X(x)p_Y(z-x)dx\\
      &=\int_{-\infty}^{+\infty}p_X(z-y)p_Y(y)dy
      \end{aligned}$$

47. 离散场合的卷积公式

    设离散随机变量$X$与$Y$独立， 则$Z=X+Y$的分布列为

    $$\begin{aligned}
      P(Z=z_l)&=\sum_{i=1}^\infty P(X=x_i)P(Y=z_l-x_i)\\
      &=\sum_{j=1}^\infty P(X=z_l-y_j)P(Y=y_j)
      \end{aligned}$$

48. 二项分布的可加性

    若$X\sim B(n_1,p),Y\sim B(n_2,p)$，且独立，则$Z=X+Y\sim B(n_1+n_2,p)$

49. 泊松分布的可加性

    若$X\sim P(\lambda_1),Y\sim P(\lambda_2)$，且独立，则$Z=X+Y\sim P(\lambda_1+\lambda_2)$

50. 正态分布的可加性

    若$X_i\sim N(\mu_i,\sigma_i^2),i=1,2,\cdots,n$，且$X_i$间相互独立，实数$a_1,\cdots,a_n$不全为零，则

    $$\sum_{i=1}^na_iX_i+b_i\sim N(\sum_{i=1}^na_i\mu_i+b_i,\sum_{i=1}^na_i^2\sigma_i^2)$$

51. $\Gamma$分布的可加性

    若$X\sim Ga(\alpha_1,\lambda),Y\sim Ga(\alpha_2,\lambda)$，且独立，则$Z=X+Y\sim Ga(\alpha_1+\alpha_2,\lambda)$

52. $\chi^2$分布的可加性

    若$X\sim \chi^2(n_1),Y\sim\chi^2(n_2)$，且独立，则$Z=X+Y\sim\chi^2(n_1+n_2)$

53. 多维随机变量的数学期望

    设$(X,Y)$是二维随机变量，$Z=g(X,Y)$，则

    $$\begin{aligned}E(Z)=E[g(X,Y)]&=
      \sum_i\sum_jg(x_i,y_j)p_{ij},&(X,Y)离散\\
      或者&=\int_{-\infty}^{+\infty}\int_{-\infty}^{+\infty}g(x,y)p(x,y)dxdy,&(X,Y)连续
      \end{aligned}$$

    一些性质

    $$\begin{aligned}
      (1)&E(X+Y)=E(X)+E(Y)\\
      (2)&若X与Y独立,则E(XY)=E(X)E(Y)
      \end{aligned}$$

54. 方差展开式

    $$\begin{aligned}
      (1)&Var(X\pm Y)=Var(X)+Var(Y)\pm 2E[X-E(X)][Y-E(Y)]\\
      (2)&E[X-E(X)][Y-E(Y)]=E(XY)-E(X)E(Y)\\
      (3)&当X与Y独立时,E[X-E(X)][Y-E(Y)]=0\\
      (4)&当X与Y独立时,Var(X\pm Y)=Var(X)+Var(Y)
      \end{aligned}$$

55. 协方差与相关系数

    定义$Cov(X,Y)=E[X-E(X)][Y-E(Y)]$为$X$与$Y$的协方差

    一些其他性质

    $$\begin{aligned}
      (1)&Cov(X,Y)=Cov(Y,X)\\
      (2)&Cov(X,a)=0\\
      (3)&Cov(aX,bY)=abCov(X,Y)\\
      (4)&Cov(X+Y,Z)=Cov(X,Z)+Cov(Y,Z)\\
      (5)&Cov(X,X)=Var(X)
      \end{aligned}$$

    定义以下这个式子为$X$与$Y$的相关系数：

    $$Corr(X,Y)=\frac{Cov(X,Y)}{\sqrt{Var(X)}\sqrt{Var(Y)}}$$

    若$Corr(X,Y)=0$，则称$X$与$Y$不相关

56. 二维正态分布的特征数

    若$(X,Y)\sim N(\mu_1,\mu_2,\sigma_1^2,\sigma_2^2,\rho)$，则

    $$\begin{aligned}
      (1)&X\sim N(\mu_1,\sigma_1^2),Y\sim N(\mu_2,\sigma_2^2)\\
      (2)&参数\rho为X与Y的相关系数\\
      (3)&X,Y独立\Leftrightarrow\rho=0\\
      (4)&不相关与独立等价
      \end{aligned}$$

57. 协方差矩阵

    记$\boldsymbol{X}=\begin{bmatrix}X_1&\cdots&X_n\end{bmatrix}^T$，则$E\boldsymbol{X}=\begin{bmatrix}EX_1&\cdots&EX_n\end{bmatrix}^T$，称

    $$Cov(\boldsymbol{X})=\begin{bmatrix}Cov(X_1,X_1)&\cdots&Cov(X_1,X_n)\\
      \vdots&\ddots&\vdots\\
      Cov(X_n,X_1)&\cdots&Cov(X_n,X_n)\end{bmatrix}$$

    为$\boldsymbol{X}$的协方差矩阵，记为$Cov(\boldsymbol{X})$，或$\boldsymbol{\Sigma}$，是一个实对称半正定矩阵。

58. 多元正态分布

    设$n$维随机变量$\boldsymbol{X}$的协方差矩阵为$\boldsymbol{\Sigma}=Cov(\boldsymbol{X})$，数学期望$E\boldsymbol{X}=\boldsymbol{\mu}$，若$n$维概率密度为

    $$p(x_1,\cdots,x_n)=p(\boldsymbol{x})=(2\pi)^{-\frac n2}|\boldsymbol{\Sigma}|^{-\frac 12}exp\{-\frac 12(\boldsymbol{x}-\boldsymbol{\mu})^T\boldsymbol{\Sigma}^{-1}(\boldsymbol{x}-\boldsymbol{\mu})\}$$

    则称$\boldsymbol{X}$满足$n$元正态分布，记作$\boldsymbol{X}\sim N(\boldsymbol{\mu},\boldsymbol{\Sigma})$

59. 相关矩阵

    称$\boldsymbol{X}$的相关矩阵为

    $$R=\begin{bmatrix}\rho_{11}&\cdots&\rho_{1n}\\\vdots&\ddots&\vdots\\\rho_{n1}&\cdots&\rho_{nn}\end{bmatrix}$$

60. 条件分布

    条件分布列：$p_{i|j}=P(X=x_i|Y=-y_j)=p_{ij}/p_{\cdot j}$

    条件密度函数：$p(x|y)=p(x,y)/p(y)$

61. 条件分布函数

    $$\begin{aligned}
      F(x|y)=P(X\le x|Y=y)&=\sum_{x_i\le x}P(X=x_i|Y=y)&X离散\\
      或者&=\int_{-\infty}^xp(t|y)dt&X连续
      \end{aligned}$$

62. 条件数学期望

    $$\begin{aligned}
      E(X|Y=y)&=\sum_ix_iP(X=x_i|Y=y)&X离散\\
      或者&=\int_{-\infty}^{+\infty}xp(x|y)dx&X连续
      \end{aligned}$$

    注意：$E(X|Y=y)$是$y$的函数

63. 重期望公式

    $$E(X)=E(E(X|Y))$$

### 3.2 大数定律与中心极限定理

1. 依概率收敛

   若对任意的$\varepsilon>0$，有$\lim\limits_{n\to\infty}P\{|Y_n-Y|<\varepsilon\}=1$，则称随机变量序列$\{Y_n\}$依概率收敛于$Y$，记为

   $$Y_n\ce{->[\quad P\quad]}Y$$

   依概率收敛的性质，若$X_n\ce{->[\quad P\quad]}a,Y_n\ce{->[\quad P\quad]}b$，则

   $\{X_n\}$和$\{Y_n\}$的加减乘除依概率收敛到$a$与$b$的加减乘除

2. 按分布收敛、弱收敛

   若在$F(x)$的连续点上都有$\lim\limits_{n\to\infty}F_n(x)=F(x)$，则称$\{F_n(x)\}$弱收敛于$F(x)$，记为

   $$F_n(x)\ce{->[\quad W\quad]}F(x)$$

   相应地，称$\{X_n\}$按分布收敛于$X$，记为

   $$X_n\ce{->[\quad L\quad]}X$$

3. 依概率收敛和按分布收敛的关系

   $$X_n\ce{->[\quad P\quad]}X\Rightarrow X_n\ce{->[\quad L\quad]}X\\
     X_n\ce{->[\quad P\quad]}a\Leftrightarrow X_n\ce{->[\quad L\quad]}a$$

4. 特征函数

   设$X$是一随机变量，称$\varphi(t)=E(e^{itX})$为$X$的特征函数，特征函数必定存在。

   当$X$离散时

   $$\varphi(t)=\sum_{k=1}^\infty e^{itx_k}p_k$$

   当$X$连续时

   $$\varphi(t)=\int_{-\infty}^{+\infty}e^{itx}p(x)dx$$

   连续的情况可以看作是$p(x)$的傅里叶变换

5. 常用分布的特征函数：略

6. 特征函数的性质

   $$\begin{aligned}
     &(1)|\varphi(t)|\le\varphi(0)=1\\
     &(2)\varphi(-t)=\overline{\varphi(t)}\\
     &(3)\varphi_{aX+b}(t)=e^{ibt}\varphi_X(at)\\
     &(4)若X与Y独立,则\varphi_{X+Y}(t)=\varphi_X(t)\varphi_Y(t)\\
     &(5)\varphi^{(k)}(0)=i^kE(X^k)
     \end{aligned}$$

   特征函数具有一致连续性和非负定性（对应我们学的是指半正定性）

7. 逆转公式

   设$F(x)$和$\varphi(x)$分别为随机变量$X$的分布函数和特征函数，则对$F(x)$的任意两个连续点$x_1<x_2$，有

   $$F(x_2)-F(x_1)=\lim_{T\to\infty}\frac 1{2\pi}\int_{-T}^T\frac{e^{-itx_1}-e^{-itx_2}}{it}\varphi(t)dt$$

8. 唯一性定理

   对$F(x)$的每一个连续点$x$，当$y$沿着$F(x)$的连续点趋于$-\infty$时，由逆转公式得

   $$F(x)=\lim_{y\to-\infty}\lim_{T\to\infty}\frac 1{2\pi}\int_{-T}^T\frac{e^{-ity}-e^{-itx}}{it}\varphi(t)dt$$

   因此特征函数唯一确定分布函数

   当$X$为连续随机变量且密度函数为$p(x)$时，有

   $$p(x)=\frac 1{2\pi}\int_{-\infty}^{+\infty}e^{-itx}\varphi(t)dt$$

9. 特征函数判断弱收敛

   $$X_n\ce{->[\quad L\quad]}X\quad\Leftrightarrow\quad\varphi_{X_n}(t)\to\varphi_X(t)$$

   分布函数序列的弱收敛性与相应特征函数序列的逐点收敛性是等价的

10. 特征函数与矩的关系：略

11. 马尔可夫不等式

    若随机变量$X$的$k$阶绝对矩存在，则对任意$\varepsilon>0$，有

    $$P\{|X|\ge\varepsilon\}\le\frac{E|X|^k}{\varepsilon^k}$$

12. 切比雪夫不等式

    若随机变量$X$的$2$阶矩存在，则对任意$\varepsilon>0$，有

    $$P\{|X-EX|\ge\varepsilon\}\le\frac{DX}{\varepsilon^2}$$

13. 伯努利大数定律

    设$\mu_n$是$n$重伯努利试验中事件$A$出现的次数，每次试验中$P(A)=p$，则对任意$\varepsilon>0$有

    $$\lim_{n\to\infty}P\{|\frac{\mu_n}n-p|<\varepsilon\}=1$$

14. 大数定律的一般形式

    若随机变量序列$\{X_n\}$满足

    $$\lim_{n\to\infty}P\{|\frac 1n\sum_{i=1}^nX_i-\frac 1n\sum_{i=1}^nEX_i|<\varepsilon\}=1$$

    则称$\{X_n\}$服从大数定律

15. 切比雪夫大数定律

    若随机变量序列$\{X_n\}$两两不相关，且$X_n$方差存在，有共同的上界，则$\{X_n\}$服从大数定律

16. 马尔可夫大数定律

    若随机变量序列$\{X_n\}$满足

    $$\lim_{n\to\infty}\frac 1{n^2}Var(\sum_{i=1}^nX_i)=0$$

    则$\{X_n\}$服从大数定律

17. 辛钦大数定律

    若随机变量序列$\{X_n\}$独立同分布，且$X_n$的数学期望存在，则$\{X_n\}$服从大数定律

18. 林德贝格——勒维中心极限定理

    若随机变量序列$\{X_n\}$独立同分布，数学期望为$\mu$，方差为$\sigma^2>0$，有

    $$\lim_{n\to\infty}P\{\frac{\sum\limits_{i=1}^nX_i-n\mu}{\sigma\sqrt n}\le y\}=\Phi(y)$$

19. 棣莫弗——拉普拉斯中心极限定理

    设$\mu_n$为服从二项分布$B(n,p)$的随机变量，则

    $$\lim_{n\to\infty}P\{\frac{\mu_n-np}{\sqrt{np(1-p)}}\le y\}=\Phi(y)$$

20. 独立不同分布下的中心极限定理：略

21. 泊松极限定理的特例

    在$n$重伯努利试验中，记$p_n$为一次实验中成功的概率，若$np_n\to\lambda$，$S_n$为成功次数，则

    $$S_n\ce{->[\quad L\quad]}P(\lambda)$$

    这也解释了可以用泊松分布近似表示二项分布的原因

### 3.3 参数估计与假设检验

### 3.4 随机过程

### 3.5 一致最优估计

### 3.6 一致最优功效检验

### 3.7 线性回归分析

### 3.8 多元正态分布

### 3.9 线性判别函数与主成分分析

## 第四章 数理逻辑

### 4.1 命题逻辑

1. 简单的基础概念

   命题、联结词

   命题变元、原子公式、由联结词集合生成的公式

   真值赋值、永真式、可满足式、永假式、真值表、替换

   等值演算、对偶定理

   文字、简单合取式（析取式）、合取（析取）范式、主合取（析取）范式

   逻辑推论

2. 对偶定理

   设$A$是由$\{0,1,\urcorner,\wedge,\vee\}$生成的公式，将$A$中的$\wedge$和$\vee$互换，$0$和$1$互换得到$A^*$，称$A^*$与$A$互为对偶式。

   若真值赋值$v_1,v_2$满足：对每个命题变元$p$，$p^{v_1}\neq p^{v_2}$，则称$v_1,v_2$是相反的真值赋值。

   设$A$是由$\{0,1,\urcorner,\wedge,\vee\}$生成的公式，$A^*$与$A$互为对偶式，$v$和$v'$是箱单的真值赋值，则$v(A^*)=\urcorner v'(A)$。

   对偶定理：设$A,B$是$\{0,1,\urcorner,\wedge,\vee\}$生成的公式，$A$与$A^*$互为对偶式，$B$与$B^*$互为对偶式，则

   $$如果A\Leftrightarrow B,那么A^*\Leftrightarrow B^*$$

3. 完全集和极小完全集

   设$S$是联结词集合。如果每个$n(n\ge1)$元联结词都可由$S$定义，则称$S$为完全集。

   若从完全集$S$中去掉任意一个联结词就成为不完全的了，则称$S$为极小完全集。

   若完全集$S_1$中的每个联结词都可由联结词集合$S_2$定义，则$S_2$也是完全集。

4. 永真式与永假式的主范式

   出现$n$个命题变元的公式$A$为永真式，与以下两个条件均等价：

   $(1)A$的主析取范式中包含所有$2^n$个极小项。

   $(2)A$的主合取范式中不包含任何极大项。

   出现$n$个命题变元的公式$A$为永假式，与以下两个条件均等价：

   $(1)A$的主析取范式不包含任何极小项。

   $(2)A$的主合取范式中包含所有$2^n$个极大项。

5. 逻辑推论

   若真值赋值$v$满足公式集合$\Gamma$中的每个公式，则称$v$满足$\Gamma$。

   设$A$是公式，若每个满足$\Gamma$的真值赋值都满足$A$，则称$A$是$\Gamma$的逻辑推论，记为$\Gamma\vDash A$。

6. 逻辑推论相关定理

   设$A$是公式则$\vDash A$当且仅当$A$是永真式。

   设$A_1,\cdots,A_n,B$是公式，则$A_1,\cdots,A_n\vDash B$，当且仅当$A_1\wedge\cdots\wedge A_n\to B$是永真式。

   设$A,B$是公式，则$A\Leftrightarrow B$，当且仅当$A\vDash B$且$B\vDash A$。

   设$\Gamma$是公式集，$A,B$是公式，则$\Gamma\cup\{A\}\vDash B$，当且仅当$\Gamma\vDash A\to B$。

   设$n$是正整数，则公式集$\{A_1,\cdots A_n\}$是可满足的，当且仅当$A_1\wedge\cdots\wedge A_n$是可满足式。

   设$\Gamma$是公式集，则$\Gamma$是不可满足的，当且仅当每个公式都是$\Gamma$的逻辑推论。

### 4.2 谓词逻辑

1. 简单的基础概念

   谓词、量词、论域

   变元、常元、函数符号、谓词符号、一阶谓词逻辑、二阶谓词逻辑、项、公式

   自由变元、约束变元、辖域、基项、语句、开公式、代换、可代入的、闭包

   解释、赋值、永真式、判定问题、半可解的、半可判定的

   等值演算、逻辑推论

2. 存在与全称的表达

   如果存在$x$满足$P(x)$的同时满足$Q(x)$，则记作：$\exists x(P(x)\wedge Q(x))$

   如果所有$x$满足$P(x)$的同时满足$Q(x)$，则记作：$\forall x(P(x)\to Q(x))$

3. 等值演算公式

   若$A,B$是任意公式，$x$是任意变元，$y$不是$A$的自由变元且对于$A$中的$x$是可代入的，则

   $$\begin{aligned}
     &(1)\urcorner\forall xA\Leftrightarrow\exists x\urcorner A\\
     &(2)\urcorner\exist xA\Leftrightarrow\forall x\urcorner A\\
     &(3)\forall xA\Leftrightarrow\forall yA_y^x\\
     &(4)\exist xA\Leftrightarrow\exist yA_y^x
     \end{aligned}$$

   若$A,B$是任意公式，$x$不是$B$的自由变元，则

   $$\begin{aligned}
     &(1)\forall x(A\wedge B)\Leftrightarrow\forall xA\wedge B\\
     &(2)\forall x(A\vee B)\Leftrightarrow\forall xA\vee B\\
     &(3)\forall x(A\to B)\Leftrightarrow\exist xA\to B\\
     &(4)\forall x(B\to A)\Leftrightarrow B\to\forall xA\\
     &(5)\exist x(A\wedge B)\Leftrightarrow\exist xA\wedge B\\
     &(6)\exist x(A\vee B)\Leftrightarrow\exist xA\vee B\\
     &(7)\exist x(A\to B)\Leftrightarrow\forall xA\to B\\
     &(8)\exist x(B\to A)\Leftrightarrow B\to\exist xA
     \end{aligned}$$

   若$A,B$是任意公式，则

   $$\begin{aligned}
     &(1)\forall x(A\wedge B)\Leftrightarrow\forall xA\wedge\forall xB\\
     &(2)\exist x(A\vee B)\Leftrightarrow\exist xA\vee \exist xB
     \end{aligned}$$

4. 逻辑推论相关定理

   命题逻辑部分定理均在谓词逻辑部分适用

   设$A,B$是任意公式，则$\forall xA\vee\forall xB\vDash\forall x(A\vee B)$。

   设$A$是任意公式，则$\forall x\forall yA\vDash\forall xA_x^y$，其中$x$对于$A$中的$y$是可代入的。

   设$\Gamma$是公式集合，$A$是公式，变元$x$不是$\Gamma$中任何公式的自由变元，则$\Gamma\vDash A\Rightarrow\Gamma\vDash \forall xA$

### 4.3 公理系统

1. 命题逻辑的公理系统

   （1）符号

   （2）公式

   （3）公理

   $$\begin{aligned}
     &A\to (B\to A)&\mathcal{A}_1\\
     &(A\to(B\to C))\to((A\to B)\to(A\to C))&\mathcal{A}_2\\
     &(\urcorner A\to\urcorner B)\to(B\to A)&\mathcal A_3
     \end{aligned}$$

   （4）推理规则

   $$MP规则:从A和A\to B推出B$$

2. 谓词逻辑的公理系统

   （1）符号

   （2）项和公式

   （3）公理

   $$\begin{aligned}
     &A\to (B\to A)&\mathcal{A}_1\\
     &(A\to(B\to C))\to((A\to B)\to(A\to C))&\mathcal{A}_2\\
     &(\urcorner A\to\urcorner B)\to(B\to A)&\mathcal{A}_3\\
     &\forall x_iA\to A_t^{x^i},其中项t对于A中的x_i可代入&\mathcal{A}_4\\
     &\forall x_i(A\to B)\to(A\to\forall x_iB),其中x_i不是A的自由变元&\mathcal{A}_5
     \end{aligned}$$

   （4）推理规则

   $$\begin{aligned}
     &MP规则:从A和A\to B推出B\\
     &UG规则:从A推出\forall x_iA
     \end{aligned}$$

3. 协调性

   当公理系统可靠且完备时，如果对于每个公式$A$，$\Gamma\vdash A$，则称公式集$\Gamma$是不协调的，否则称$\Gamma$是协调的。

   $\Gamma$协调，当且仅当$\Gamma$可满足。

4. 可靠性

   可靠性定理：若$\Gamma\vdash A$，则$\Gamma\vDash A$。

   公理系统可靠，当且仅当公理系统满足可靠性定理。

5. 完备性

   完备性定理：若$\Gamma\vDash A$，则$\Gamma\vdash A$。

   公理系统完备，当且仅当公理系统满足完备性定理。

6. 紧致性定理

   第一种形式：若$\Gamma\vDash A$，则有$\Gamma$的有穷子集$\Gamma_1$，使得$\Gamma_1\vDash A$。

   第二种形式：若$\Gamma$不可满足，则有$\Gamma$的有穷子集不可满足。

   紧致性定理是一阶逻辑的重要性质，对于二阶逻辑，紧致性定理不再成立。

## 第五章 集合论

### 5.1 集合

### 5.2 二元关系

### 5.3 函数

### 5.4 自然数

## 第六章 图论

### 6.1 图的基本概念

### 6.2 欧拉图与哈密顿图

### 6.3 树的基本概念

### 6.4 图论算法

## 第七章 组合数学

### 7.1 计数原理

1. 加法原理：分类计数；乘法原理：分步计数；减法原理：求补计数。

2. 常用计数公式

   $$\begin{aligned}
     &从n个元素中选取k个,满足以下条件:\\
     &(1)可重排列:n^k\\
     &(2)无重排列:P(n,k)=\frac{n!}{(n-k)!}\\
     &(3)可重组合:\begin{pmatrix}n+k-1\\k\end{pmatrix}=\frac{(n+k-1)!}{(n-1)!k!}\\
     &(4)无重组合:\begin{pmatrix}n\\k\end{pmatrix}=\frac{n!}{(n-k)!k!}\\
     &(5)圆周排列:\frac 1kP(n,k)\\
     &(6)项链排列:\frac 1{2k}P(n,k)\\
     \end{aligned}$$

3. 不定方程正整数解的个数

   $$x_1+x_2+\cdots+x_k=n的正整数解个数为\begin{pmatrix}n-1\\k-1\end{pmatrix}$$

   若更改为求非负整数解，则通过换元即可求得$\begin{pmatrix}n+k-1\\k-1\end{pmatrix}$

4. 有限多重集排列

   $$对于种类数为k的n个元素,每个种类分别有n_k个元素,其排列数为\frac{n!}{n_1!\cdots n_k!}$$

5. 不相邻组合

   $$在\{1,2,\cdots,n\}中选择k个不相邻的数,方案数为\begin{pmatrix}n-k+1\\k\end{pmatrix}$$

   通过构造双射转化为$\{a_1,\cdots,a_k-(k-1)\}\sub\{1,\cdots,n-k+1\}$的无重组合

6. 有限多重组合

   $$对于种类数为k的n个元素,每个种类分别有n_k个元素,其任意数目的组合数为(n_1+1)\cdots(n_k+1)$$

7. 常用组合恒等式

   $$\begin{aligned}
     &(1)\begin{pmatrix}n\\k\end{pmatrix}=\begin{pmatrix}n-1\\k\end{pmatrix}+\begin{pmatrix}n-1\\k-1\end{pmatrix}\\
     &(2)k\begin{pmatrix}n\\k\end{pmatrix}=n\begin{pmatrix}n-1\\k-1\end{pmatrix}\\
     &(3)\begin{pmatrix}n\\k\end{pmatrix}\begin{pmatrix}k\\r\end{pmatrix}=\begin{pmatrix}n\\r\end{pmatrix}\begin{pmatrix}n-r\\k-r\end{pmatrix}\\
     &(4)\begin{pmatrix}m+n\\k\end{pmatrix}=\sum_{i=0}^k\begin{pmatrix}m\\i\end{pmatrix}\begin{pmatrix}n\\k-i\end{pmatrix}\\
     &(5)\begin{pmatrix}m+n\\m\end{pmatrix}=\sum_{i=0}^m\begin{pmatrix}m\\i\end{pmatrix}\begin{pmatrix}n\\i\end{pmatrix}\\
     &(6)\begin{pmatrix}n+1\\k+1\end{pmatrix}=\sum_{i=k}^n\begin{pmatrix}i\\k\end{pmatrix}\\
     &(7)\begin{pmatrix}2n\\n\end{pmatrix}=\sum_{i=0}^n\begin{pmatrix}n\\i\end{pmatrix}^2\\
     &(8)2^n=\sum_{i=0}^n\begin{pmatrix}n\\i\end{pmatrix}
     \end{aligned}$$

8. 排列生成算法

   递归生成算法、邻位对换算法、逆序生成算法

   逆序数$b_1b_2\cdots b_n$，其中$b_k$表示比$k$大但在$k$前面的数字的个数

9. 组合生成算法

   二进制算法、反射$Gray$码

   二进制算法：用二进制数$\overline{a_{n-1}\cdots a_1a_0}$表示$\{x_{n-1},\cdots,x_1,x_0\}$中的组合，第$k$个组合即为$k$的二进制记数所对应的集合

10. $r$子集生成算法

    $r$子集的字典序：若$A\cup B/A\cap B$的最小整数属于$A$，则称$A$先于$B$

    从$12\cdots r$开始，依次列出直接后继，即可生成所有$r$子集

11. 二项式定理

    $$(x+y)^n=\sum_{k=0}^n\begin{pmatrix}n\\k\end{pmatrix}x^{n-k}y^k$$

12. 链与反链

    设集合$S$含有$n$个元素

    若$T\sub\rho(S)$为$S$上的一个反链，则$\forall A,B\in T,(A\nsubseteq B\wedge B\nsubseteq A)$

    最大反链含有$\begin{pmatrix}n\\\lfloor n/2\rfloor\end{pmatrix}$个子集，且各子集元素个数相同

    若$T\sub\rho(S)$为$S$上的一个链，则$\forall A,B\in T,(A\sub B\vee B\sub A)$

    最大链含有$n+1$个子集

    $S$上的一条反链最多只能包含$S$的任意一条链中的一个子集

    $S$上的一条链最多只能包含$S$的任意一条反链中的一个子集

13. 多项式定理

    $$(x_1+\cdots+x_k)^n=\sum_{n_1+\cdots+n_k=n}\frac{n!}{n_1!\cdots n_k!}x_1^{n_1}\cdots x_k^{n_k}$$

14. 牛顿二项式定理

    $$(x+y)^\alpha=\sum_{n=0}^\infty\frac{\alpha(\alpha-1)\cdots(\alpha-n+1)}{n!}x^ny^{\alpha-n}$$

15. 负二项式定理

    $$\frac 1{(1-x)^k}=\sum_{n=0}^\infty \begin{pmatrix}n+k-1\\n\end{pmatrix}x^n,x\in(-1,1)$$

### 7.2 递推关系与生成函数

1. $Fibonacci$数列

   $$\begin{cases}
     &f_n=f_{n-1}+f_{n-2}(n\ge 2)\\
     &f_0=0,f_1=1
     \end{cases}$$

   通项公式

   $$f_n=\frac 1{\sqrt5}(\frac{1+\sqrt5}2)^n-\frac 1{\sqrt5}(\frac{1-\sqrt5}2)^n(n\ge0)$$

   其他性质

   $$\begin{aligned}
     &(1)s_n=f_0+f_1+\cdots+f_n=f_{n+2}-1\\
     &(2)2|f_n\Leftrightarrow 3|n\\
     &(3)3|f_n\Leftrightarrow 4|n\\
     &(4)4|f_n\Leftrightarrow 6|n\\
     &(5)\lim_{n\to\infty}\frac{f_n}{f_{n+1}}=\frac{\sqrt 5-1}2
     \end{aligned}$$

2. 生成函数

   序列$h_0,h_1,\cdots,h_n,\cdots$唯一确定生成函数

   $$G(x)=\sum_{n=0}^\infty h_nx^n$$

3. 指数生成函数

   序列$h_0,h_1,\cdots,h_n,\cdots$唯一确定指数生成函数

   $$G_e(x)=\sum_{n=0}^\infty h_n\frac{x^n}{n!}$$

4. 线性常系数递推式求解

   $$\begin{aligned}
     &特征方程:类比微分方程\\
     &基础解系:(a_kn^k+\cdots+a_0)\alpha^n,若\alpha是k重根\\
     &非齐次特解:若非齐次部分b_n=P_m(n)d^n,P_m(n)是n的m次多项式,则\\
     &特解形式为:h_n^*=n^kd^nA_m(n),其中k为d在特征方程中根的重数
     \end{aligned}$$

5. $Catalan$数

   $$\begin{aligned}
     &递推公式:\begin{cases}&C_n=C_0C_{n-1}+C_1C_{n-2}+\cdots+C_{n-1}C_0\\
     &C_0=1\end{cases}\\
     &通项公式:C_n=\frac 1{n+1}\begin{pmatrix}2n\\n\end{pmatrix}\\
     &其他性质:\frac{C_n}{C_{n-1}}=\frac{4n-2}{n+1}\\
     \end{aligned}$$

6. 拟$Catalan$数

   定义$C_n^*=n!C_{n-1}(n\ge1)$，则有$C_n^*=(4n-6)C_{n-1}^*(n\ge2),C_1^*=1$

7. 差分序列

   该课程中采用后向差分：$\Delta^ph_n=\Delta^{p-1}h_{n+1}-\Delta^{p-1}h_n$

   根据差分表可以得出通项公式

   $$h_n=\sum_{k=0}^\infty\Delta^kh_0\begin{pmatrix}n\\k\end{pmatrix}$$

   同时也能得出部分和的通项公式

   $$\sum_{k=0}^nh_k=\sum_{k=0}^\infty\Delta^kh_0\begin{pmatrix}n+1\\k+1\end{pmatrix}$$

   注意到，$\Delta^kh_0$一般只有有限项非零，所以同通项公式实际上是一个部分和的形式。

8. 第二类$Stirling$数

   记$[n]_k=k!\begin{pmatrix}n\\k\end{pmatrix}=n(n-1)\cdots(n-k+1)$，则

   $$h_n=n^p=\sum_{k=0}^p\frac{c(p,k)}{k!}[n]_k=\sum_{k=0}^pS(p,k)[n]_k$$

   上式中的系数$S(p,k)$称为第二类$Striling$数

   $$\begin{aligned}
     &第二类Stirling数的性质\\
     &(1)S(p,0)=\begin{cases}1,p=0\\0,p\ge 1\end{cases}\\
     &(2)S(p,p)=1,p\ge 1\\
     &(3)S(p,1)=1,p\ge 1\\
     &(4)S(p,k)=kS(p-1,k)+S(p-1,k-1),1\le k\le p-1\\
     &(5)S(p,2)=2^{p-1}-1\\
     &(6)S(p,p-1)=\begin{pmatrix}p\\2\end{pmatrix}
     \end{aligned}$$

   组合解释：$S(p,k)$表示把$p$元素集合划分到$k$个不可区分的盒子且没有空盒的划分个数。

   若盒子可区分，则方案数为$k!S(p,k)$，记作$S^\#(p,k)$

9. $Bell$数

   $Bell$数为把$p$元素集合划分到$k$个不可区分的盒子且允许有空盒的划分个数。

   $$B_p=\sum_{k=0}^pS(p,k)$$

   $Bell$数满足以下递推关系

   $$B_p=\sum_{k=0}^{p-1}\begin{pmatrix}p-1\\k\end{pmatrix}B_k$$

10. 第一类$Stirling$数

    $$[n]_p=\sum_{k=0}^p(-1)^{p-k}s(p,k)n^k$$

    上式中的系数$s(p,k)$称为第一类$Striling$数

    $$\begin{aligned}
      &第一类Stirling数的性质\\
      &(1)s(p,0)=0,p\ge 1\\
      &(2)s(p,1)=1,p\ge 0\\
      &(3)s(p,k)=(p-1)s(p-1,k)+s(p-1,k-1),1\le k\le p-1
      \end{aligned}$$

    组合解释：将$p$个物品排成$k$个非空循环排列的方法数

11. 将$n$个球放入$m$个盒子的问题分类讨论

    | () 球有无区别 | 盒子有无区别 | 是否允许空盒 | 方案数或母函数                        |
    | :------------ | :----------- | :----------- | :------------------------------------ |
    | () 有         | 有           | 有           | $m^n$                                 |
    | 有            | 有           | 无           | $m!S(n,m)$                            |
    | 有            | 无           | 有           | $S(n,1)+S(n,2)+\cdots+S(n,\min(m,n))$ |
    | 有            | 无           | 无           | $S(m,n)$                              |
    | 无            | 有           | 有           |                                       |
    | m-1           |              |              |                                       |
    | 无            | 有           | 无           |                                       |
    | m-1           |              |              |                                       |
    | 无            | 无           | 有           | $G(x)=\frac1{(1-x)\cdots(1-x^m)}$     |
    | 无            | 无           | 无           | $G(x)=\frac{x^m}{(1-x)\cdots(1-x^m)}$ |
    | ()            |              |              |                                       |

12. 整数的拆分

    将正整数$n$拆分为$1,2\cdots$之和，允许重复

    $$G_1(x)=\sum_{n=1}^\infty\frac 1{1-x^n}$$

    将正整数$n$拆分为$1,2\cdots$之和，不允许重复

    $$G_2(x)=\sum_{n=1}^\infty(1+x^n)$$

    将正整数$n$拆分为$1,2\cdots$之和，允许重复

    $$G_3(x)=\sum_{n=1}^\infty\frac 1{1-x^{2n-1}}$$

    在上式中，有$G_2(x)=G_3(x)$

13. $Ferrers$图像

    靠左的上三角图像，上一行不少于下一行，左一列不少于右一列，从上到下表示分拆方案

14. 共轭$Ferrers$图像

    分拆$\lambda$对应的$Ferrers$图像进行转置，则得到$\lambda$的共轭分拆$\lambda^*$对应的$Ferrers$图像

    组合解释：设$m\le n$，则$n$拆分为最多$m$个数的和的拆分数等于将$n$拆分为最大数不超过$m$的拆分数

    自共轭$Ferrers$图像：$\lambda=\lambda^*$或图像关于对角线对称

### 7.3 容斥原理与鸽巢原理

1. 鸽巢原理

   将$n+1$个物体放入$n$个盒子，则至少有一个盒子包含至少两个物体。

2. 鸽巢原理的加强形式

   将$q_1+q_2+\cdots+q_n-n+1$个物体放进$n$个盒子里，则或者第$1$个盒子至少含$q_1$个物体，或者第$2$个盒子至少含$q_2$个物体，$\cdots$，或者第$n$个盒子至少含$q_n$个物体。

3. 鸽巢原理的推广

   将$n(r-1)+1$个物体放入$n$个盒子，则至少有一个盒子包含至少$r$个物体。

4. 平均值原理

   若$n$个非负整数的平均数大于$r-1$，则至少有一个非负整数大于等于$r$。

5. $Ramsey$问题

   对完全图$K_r$进行红蓝二染色，对任何染色都存在红色$K_m$或蓝色$K_N$的最小图的阶$a_{min}$记作$r(m,n)$，且满足以下性质

   $$\begin{aligned}
     &(1)r(m,n)=r(n,m)\\
     &(2)r(m,2)=m,r(3,3)=6,r(3,4)=9,r(3,3,3)=17\\
     &(3)对于m,n\ge 2,有r(m,n)\le r(m-1,n)+r(m,n-1)
     \end{aligned}$$

6. 容斥原理

   $$|A\cup B|=|A|+|B|-|A\cap B|$$

   $$|A\cup B\cup C|=|A|+|B|+|C|-|A\cap B|-|A\cap C|-|B\cap C|+|A\cap B\cap C|$$

   以上规律可以推广到$n$个集合

   以及可以考虑德摩根律求解$|A\cap B\cap C|$等

7. 错位排列

   $$D_n=n!\sum_{k=0}^n\frac{(-1)^k}{k!}$$

   错位排列满足一定的递推关系

   $$\begin{cases}
     &D_n=(n-1)(D_{n-1}+D_{n-2})(n\ge 3)\\
     &D_n=nD_{n-1}+(-1)^n\\
     &D_1=0,D_2=1
     \end{cases}$$

8. 非攻击型车的禁区排列数

   记$r_i$为有$i$个棋子布置到禁区的方案数，则放置$n$个相同的非攻击性车到$n\times n$棋盘上的方案数为

   $$n!-r_1(n-1)!+r_2(n-2)!-\cdots+(-1)^nr_n$$

   如果非攻击性车是可区分的，还应乘对应的排列数。

9. 容斥原理的一般公式

   设$p_k$为至少有$k$种性质的元素个数，$q_k$为恰有$k$种性质的元素个数，则

   $$q_k=p_k-\begin{pmatrix}k+1\\1\end{pmatrix}p_{k+1}+\begin{pmatrix}k+2\\2\end{pmatrix}p_{k+2}+\cdots+(-1)^{n-k}\begin{pmatrix}n\\n-k\end{pmatrix}p_n$$

10. 记$Q_n$为$\{1,\cdots,n\}$中不出现$12,23,\cdots,(n-1)n$这些模式的排列数，则

    $$Q_n=n!-\begin{pmatrix}n-1\\q\end{pmatrix}(n-1)!+\begin{pmatrix}n-2\\2\end{pmatrix}(n-2)!+\cdots+(-1)^{n-1}\begin{pmatrix}n-1\\n-1\end{pmatrix}1!$$

    且$Q_n=D_n+D_{n-1}$

### 7.4 $P\acute olya$定理

1. $P\acute olya$定理

   设$\bar G$是$n$个对象上的置换群，用$m$种颜色给这$n$个对象染色，则不同染色方案数为

   $$l=\frac 1{|\bar G|}\left[m^{c(\bar a_1)}+m^{c(\bar a_2)}+\cdots+m^{c(\bar a_g)}\right]$$

   其中$\bar G=\{\bar a_1,\bar a_2,\cdots \bar a_g\}$，$c(\bar a_k)$为置换$\bar a_k$的循环节数

2. $P\acute olya$定理的母函数形式

   设$c(\bar a_k)$为置换$\bar a_k$的循环节数，$c_i(\bar a_k)$为置换$\bar a_k$中的$i$阶循环因子的节数，用$m$种颜色$b_1,b_2,\cdots,b_m$对$1,2,\cdots,n$中的元素染色，则将

   $$m^{c(\bar a_i)}=(b_1+\cdots+b_m)^{c_a(\bar a_i)}\times\cdots\times(b_1^n+\cdots b_m^n)^{c_n(\bar a_i)},i=1,\cdots,g$$

   代入

   $$l=\frac 1{|\bar G|}\left[m^{c(\bar a_1)}+m^{c(\bar a_2)}+\cdots+m^{c(\bar a_g)}\right]$$

   得到以$b_1,\cdots,b_m$为变元的$n$次对称多项式$P(b_1,\cdots,b_m)$即为染色方案数的母函数

## 第八章 算法设计

### 8.1 分治算法

### 8.2 动态规划

### 8.3 贪心算法

### 8.4 $NP$问题

## 第九章 复变函数与积分变换

### 9.1 解析函数

### 9.2 复变函数的积分

### 9.3 复变函数级数

### 9.4 留数定理

### 9.5 $Fourier$变换

### 9.6 $Laplace$变换

### 9.7 $Z$变换

## 第十章 最优化理论

### 10.1 线性规划

### 10.2 凸集与凸函数

### 10.3 最优性条件

## 第十一章 矩阵分析

### 11.1 线性空间与线性变换

### 11.2 内积空间

### 11.3 矩阵的相似标准型

### 11.4 矩阵分解

### 11.5 矩阵分析

## 第十二章 数值分析

### 12.1 范数

### 12.2 线性方程组

### 12.3 矩阵的特征值与特征向量

### 12.4 非线性方程组的迭代算法

### 12.5 插值与逼近

### 12.6 数值积分
