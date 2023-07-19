## Tech of integration
let $h(x)=f(x)g(x)$，$h'(x)=f'(x)g(x)+f(x)g'(x)$，
$$
\int h'(x)dx=\int f'(x)g(x)dx+\int f(x)g'(x)dx\\
\int f(x)dg(x)=f(x)g(x)-\int g(x)df(x)
$$
### several part integrals
$$
\int xsinxdx=-xcosx+sinx+C\\
\int xcosxdx=xsinx+cosx+C\\
\int xe^xdx=e^x(x-1)+C\\
\int lnxdx=x(lnx-1)+C\\
\int log_bxdx=\dfrac{x}{lnb}(lnx-1)+C\\
\int xlnxdx=\dfrac{1}{2}x^2lnx-\int \dfrac{1}{2}xdx=\dfrac{1}{2}x^2(lnx-\dfrac{1}{2})+C
$$
### 反三角函数积分
$$
\begin{aligned}
\int arcsinxdx&=xarcsinx(x)-\int x\dfrac{1}{\sqrt{1-x^2}}dx\\
&=xarcsinx(x)-\int d(-\sqrt{1-x^2})\\
&=xarcsinx(x)+\sqrt{1-x^2}+C\\
\end{aligned}\\
\begin{aligned}
\int arccosxdx&=xarccosx-\int x\dfrac{-1}{\sqrt{1-x^2}}dx\\
&=xarccosx+\int d(-\sqrt{1-x^2})\\
&=xarccosx-\sqrt{1-x^2}+C\\
\end{aligned}\\
\begin{aligned}
\int acrtanxdx&=xarctanx-\int x\dfrac{1}{1+x^2}dx\\
&=xarctanx-\int \dfrac{1}{2}d(ln(1+x^2))\\
&=xarctanx-\dfrac{1}{2}ln(1+x^2)+C\\
\end{aligned}\\
\begin{aligned}
\int acrtcotxdx&=xarccotx+\int x\dfrac{1}{1+x^2}dx\\
&=xarccotx+\int \dfrac{1}{2}d(ln(1+x^2))\\
&=xarccotx+\dfrac{1}{2}ln(1+x^2)+C\\
\end{aligned}\\
\begin{aligned}
\int arcsecxdx&=xarcsecx-\int x\dfrac{1}{x\sqrt{x^2-1}}dx\\
&=xarcsecx-ln\vert x+\sqrt{x^2-1}\vert +C\\
\end{aligned}\\
\begin{aligned}
\int arccscxdx&=xarccscx+\int x\dfrac{1}{x\sqrt{x^2-1}}dx\\
&=xarccscx+ln\vert x+\sqrt{x^2-1}\vert +C\\
\end{aligned}\\
$$
### 反双曲积分
$$
\begin{aligned}
\int arcsinhxdx&=xarcsinhx-\int x\dfrac{1}{\sqrt{x^2+1}}dx\\
&=xarcsinhx-\sqrt{x^2+1}+C\\
\end{aligned}\\
\begin{aligned}
\int arccoshxdx&=xarccoshx-\int x\dfrac{1}{\sqrt{x^2-1}}dx\\
&=xarcsinhx-\sqrt{x^2-1}+C\\
\end{aligned}\\
\begin{aligned}
\int arctanhxdx&=xarctanhx-\int x\dfrac{1}{1-x^2}dx\\
&=xarctanhx+\dfrac{1}{2}ln(1-x^2)+C,(x\in (-1,1))\\
\end{aligned}\\
\begin{aligned}
\int arccothxdx&=xarccothx-\int x\dfrac{1}{1-x^2}dx\\
&=xarccothx+\dfrac{1}{2}ln(x^2-1)+C,(x\in (-\infin,-1)\cup(1,\infin))\\
\end{aligned}\\
\begin{aligned}
\int arcsechxdx&=xarcsechx+\int x\dfrac{1}{x\sqrt{1-x^2}}dx\\
&=xarcsechx-arcsinx+C,(x\in(0,1))\\
\end{aligned}\\
\begin{aligned}
\int arccschxdx&=xarccschx+\int x\dfrac{1}{\vert x\vert\sqrt{x^2+1}}dx\\
&=\begin{cases}
xarccschx+ln(x+\sqrt{x^2+1})+C,(x>0)\\
xarccschx-ln(x+\sqrt{x^2+1})+C,(x<0)\\
\end{cases}
\end{aligned}\\
$$
### 三角积分
$$
\int sin^2xdx=\dfrac{1}{2}x-\dfrac{1}{4}sin(2x)+C\\
\int cos^2xdx=\dfrac{1}{2}x+\dfrac{1}{4}sin(2x)+C
$$
积分$\int sin^ixcos^jxdx$，如果i或者j有奇数就凑，没有奇数用二倍角公式展开
### 积化和差
$$
sin(ax)sin(bx)=\dfrac{1}{2}cos((a-b)x)-\dfrac{1}{2}cos((a+b)x)\\
sin(ax)cos(bx)=\dfrac{1}{2}sin((a-b)x)+\dfrac{1}{2}sin((a+b)x)\\
cos(ax)cos(bx)=\dfrac{1}{2}cos((a-b)x)+\dfrac{1}{2}cos((a+b)x)
$$
### 练习
$$
\int sec^3xtan^5xdx\\
\int tan^6sec^4xdx\\
\int tan^3xdx\\
\int sec^3xdx\\
$$
### tanxsecx递推公式
一个分布积分，一个展开
$$
\int sec^nxdx=\int sec^{n-2}dtanx=\dfrac{1}{n-1}sec^{n-2}xtanx+\dfrac{n-2}{n-1}\int sec^{n-2}xdx\\
\int tan^ndx=\int tan^{n-2}x(sec^2x-1)dx=\dfrac{1}{n-1}tan^{n-1}x-\int tan^{n-2}xdx
$$
### 三角双曲代换
#### $\sqrt{a^2-x^2}$代$x=asin\theta,\theta\in[-\dfrac{\pi}{2},\dfrac{\pi}{2}]$
$$
dx=dasin\theta=acos\theta d\theta\\
\vert cos\theta\vert=cos\theta\geq0\\
\sqrt{a^2-x^2}=a\vert cos\theta\vert=acos\theta\\
\theta=arcsin\dfrac{x}{a}
$$
#### $\sqrt{a^2-x^2}$代$x=atanh\theta,\theta\in R$
$$
1-tanh^2\theta=sech^2\theta\\
dx=datanh\theta=asech^2\theta d\theta\\
sech\theta>0,\theta\in R\\
\sqrt{a^2-x^2}=a\vert sech\theta\vert=asech\theta\\
\theta=arctanh\dfrac{x}{a}
$$
#### $\sqrt{a^2+x^2}$代$x=atan\theta,\theta\in[-\dfrac{\pi}{2},\dfrac{\pi}{2}]$
$$
dx=datan\theta=asec^2\theta d\theta\\
sec\theta>0\\
\sqrt{a^2+x^2}=asec\theta\\
\theta=arctan\dfrac{x}{a}
$$
#### $\sqrt{a^2+x^2}$代$x=asinh\theta,\theta\in R$
$$
1+sinh^2\theta=cosh^2\theta\\
dx=dasinh\theta=acosh\theta d\theta\\
cosh\theta >0,\theta\in R\\
\sqrt{a^2+x^2}=acosh\theta\\
\theta=arcsinh\dfrac{x}{a}
$$
#### $\sqrt{x^2-a^2}$代$x=sec\theta,\theta\in [0,\dfrac{\pi}{2})\cup(\dfrac{\pi}{2},\pi]$
$$
dx=dasex\theta=asec\theta tan\theta d\theta\\
\sqrt{x^2-a^2}=
\begin{cases}
atan\theta,\theta\in [0,\dfrac{\pi}{2})\\
\\
-atan\theta,\theta\in (\dfrac{\pi}{2},\pi]
\end{cases}\\
\theta=arcsec\dfrac{x}{a}
$$
#### $\sqrt{x^2-a^2}$代$x=coth\theta,\theta\neq 0$
$$
coth^2\theta-1=csch^2\theta\\
dx=dacoth\theta=-acsch^2\theta d\theta\\
\sqrt{x^2-a^2}=a\vert csch\theta\vert=
\begin{cases}
acsch\theta,\theta\in (0,+\infin)\\
\\
-acsch\theta,\theta\in (-\infin,0)
\end{cases}\\
\theta=arccoth\dfrac{x}{a}
$$
### 长除法
https://en.wikipedia.org/wiki/Polynomial_long_division
### Nonrepeated linear factors
如果积分$\int \dfrac{P(x)}{Q(x)}dx$中，分母的最高次比分子高，且能够分解成**不相同不重复的因式**的乘积$Q(x)=(a_1x+b_1)(a_2x+b_2)...(a_nx+b_n)$，那么$\dfrac{P(x)}{Q(x)}$就一定能写成
$$
\dfrac{P(x)}{Q(x)}=\dfrac{A_1}{a_1x+b_1}+...+\dfrac{A_n}{a_nx+b_n}
$$
其中$A_i$为常数
### Repeated linear factors
如果积分$\int \dfrac{P(x)}{Q(x)}dx$中，分母的最高次比分子高，且包含**相同重复的因式**的乘积$(a_ix+b_i)^i$，那么$\dfrac{P(x)}{Q(x)}$的分解一定包含
$$
\dfrac{P(x)}{Q(x)}=不重复部分的分解+\dfrac{A_1}{a_ix+b_i}+\dfrac{A_2}{(a_ix+b_i)^2}+...+\dfrac{A_i}{(a_ix+b_i)^i}
$$
其中$A_i$为常数
### 分解因子的次数
当分母不可再分时
$$
...+\dfrac{Ax+B}{ax^2+bx+c}+...\\
\
\\
\Delta <0
$$
### 立方和差
$$
a^3x^3+b^3=(ax+b)(a^2x^2-abx+b^2)\\
a^3x^3-b^3=(ax-b)(a^2x^2+abx+b^2)
$$
### exercise
$$
\int \dfrac{1}{x^3-8}dx\\
\int \dfrac{x^2+3x+1}{(x+2)(x-3)^2(x^2+4)^2}dx\\
\
\\
\dfrac{A}{x+2}+\dfrac{B}{x-3}+\dfrac{C}{(x-3)^2}+\dfrac{Dx+E}{x^2+4}+\dfrac{Fx+G}{(x^2+4)^2}
$$
### 反常积分$\infin$
Let f (x) be continuous over an interval of the form $[a, +∞)$. Then
$$
\int_a^{+\infin}f(x)dx=\lim_{t\rightarrow +\infin}\int_a^tf(x)dx
$$
Let f (x) be continuous over an interval of the form $(−∞, b]$. Then
$$
\int_{-\infin}^bf(x)dx=\lim_{t\rightarrow -\infin}\int_t^bf(x)dx
$$
**provided this limit exists.**
Let f (x) be continuous over $(−∞, +∞)$. Then
$$
\int_{-\infin}^{+\infin}f(x)dx=\int_{-\infin}^af(x)dx+\int_a^{+\infin}f(x)dx
$$
provided that $\int_{-\infin}^af(x)dx$ and $\int_a^{+\infin}f(x)dx$ both converge.If either of these two integrals diverge, then $\int_{-\infin}^{+\infin}f(x)dx$ diverge
### example
$$
\int_1^{+\infin}\dfrac{1}{x}dx\\
\int_{-\infin}^0\dfrac{1}{x^2+4}dx\\
\int_{-\infin}^{+\infin}xe^xdx\\
$$
### 反常积分$x\rightarrow b$
Let f (x) be continuous over $[a, b)$. Then,
$$
\int_a^bf(x)dx=\lim_{t\rightarrow b^-}\int_a^tf(x)dx
$$
Let f (x) be continuous over $(a, b]$. Then,
$$
\int_a^b f(x)dx=\lim_{t\rightarrow a^+}\int_t^b f(x)dx
$$
In each case, if the limit exists, then the improper integral is said to converge. If the limit does not exist, then the improper integral is said to diverge.
If f(x) is continuous over $[a, b]$ except at a point c in $(a, b)$, then
$$
\int_a^b f(x)dx=\int_a^cf(x)dx+\int_c^bf(x)dx
$$
provided both converge.
### Comparison Theorem
consider two continuous functions f(x) and g(x) satisfying $0 ≤ f (x) ≤ g(x)$ for $x ≥ a $,  we may view integrals of these functions over intervals of the form $[a, t]$ as areas, so we have the relationship
$$
0\leq\int_a^tf(x)dx\leq\int_a^tg(x)dx
$$
thus, if
$$
\int_a^{+\infin}f(x)dx=\lim_{t\rightarrow +\infin}\int_a^tf(x)dx=+\infin
$$
then,
$$
\int_a^{+\infin}g(x)dx=+\infin
$$
on the other hand, if
$$
\int_a^{+\infin}g(x)dx=\lim_{t\rightarrow +\infin}\int_a^tg(x)dx=L
$$
then,
$$
\int_a^{+\infin}f(x)dx\leq L
$$
## 微分方程
The order of a differential equation is the highest order of any derivative of the unknown function that appears in the equation.
### 初值问题
待定常数的个数和方程的最高阶数相同
### 方向场
对于一阶微分方程$y'=f(x,y)$可以通过带入任意点$(x_0,y_0),(x_1,y_1),...$来计算在该点解的斜率，形成一个斜率方向场
方向场能告诉我们通过该点的解的走向
考虑
$$
y'=2x+3
$$
的方向场，其斜率与y无关，在$x=0$时，所有解的切线斜率都是3
### 平衡解
Consider the differential equation $y′ = f (x, y)$. An equilibrium solution is any solution to the differential equation of the form $y = c$, where c is a constant.
### 渐进稳定解、渐进非稳定解和渐进半稳定解
在平衡解中：
Consider the differential equation $y′ = f (x, y)$, and assume that all solutions to this differential equation are defined for $x ≥ x_0$(让$x_0$为解的初值). Let $y = k$ be an equilibrium solution to the differential equation.
1. 当解的初值无论设定在$y=k$上下一个区间内的哪个值时，都有$x\rightarrow +\infin,y\rightarrow k$，则解$y=k$就是渐进稳定解$(\lim_{x\rightarrow +\infin}y(x)=k)$
2. 当解的初值无论设定在$y=k$上下一个区间内的哪个值时，都**没有**$x\rightarrow +\infin,y\rightarrow k$，则解$y=k$就是渐进非稳定解$(\lim_{x\rightarrow +\infin}y(x)\neq k)$
3. 当解$y=k$既不是渐进稳定解，又不是渐进非稳定解的时候，就是渐进半稳定解(有可能当初值$f(x_0)\in(\epsilon,k)$时候$\lim_{x\rightarrow +\infin}y(x)=k$，而$f(x_0)\in(k,\epsilon)$时$\lim_{x\rightarrow +\infin}y(x)\neq k$)
### example
$$
y'=(x-2)^2(y^2-2y-3)\\
$$
两个平衡解$y=3,y=-1$，$(x-2)^2>0,x\rightarrow +\infin$，
当初值$(x,y_{ini})$中$y_{ini}\in (-1,3)$，$y'<0$，
当初值$(x,y_{ini})$中$y_{ini}\in (-\infin,-1)$，$y'>0$，
解在$y=-1$上面单调下降，在$y=-1$下面单调递增，所以$y=-1$是渐进平衡解
当初值$(x,y_{ini})$中$y_{ini}\in (3,+\infin)$，$y'>0$，
解在$y=3$下面单调下降，在$y=3$上面单调递增，所以$y=3$是渐进非平衡解
### 可分离方程
A separable differential equation is any equation that can be written in the form
$$
y'=f(x)g(y)
$$
solve the equation
$$
\dfrac{dy}{g(y)}=f(x)dx
$$
### example
对常数C的处理
$$
y'=(2x+3)(y^2-4)
$$
解：
$$
\dfrac{dy}{y^2-4}=(2x+3)dx\\
\int\dfrac{1}{y^2-4}dy=\int(2x+3)dx\\
\int\dfrac{1}{4}\bigg(\dfrac{1}{y-2}-\dfrac{1}{y+2}\bigg)dy=\int(2x+3)dx\\
左边=\dfrac{1}{4}ln\vert y-2\vert -\dfrac{1}{4}ln\vert y+2\vert+C_1\\
右边=x^2+3x+C_2\\
有：ln\vert y-2\vert-ln\vert y+2\vert=4x^2+12x+C_3\\
即：ln\dfrac{\vert y-2\vert}{\vert y+2\vert}=4x^2+12x+C_3\\
e^{ln\dfrac{\vert y-2\vert}{\vert y+2\vert}}=e^{4x^2+12x+C_3}\\
\dfrac{\vert y-2\vert}{\vert y+2\vert}=e^{4x^2+12x+C_3}\\
令C_4=e^{C_3},\dfrac{\vert y-2\vert}{\vert y+2\vert}=C_4e^{4x^2+12x}\\
摘掉绝对值：令C_5=\pm C_4,\dfrac{ y-2}{ y+2}=C_5e^{4x^2+12x}\\
y-2=yC_5e^{4x^2+12x}+2C_5e^{4x^2+12x}\\
y(1-C_5e^{4x^2+12x})=2(1+C_5e^{4x^2+12x})\\
y=\dfrac{2(1+C_5e^{4x^2+12x})}{(1-C_5e^{4x^2+12x})}----->e^{4x^2+12x}\geq e^{-9}
\begin{cases}
C_5=0,y=2\\
C_5\rightarrow \infin,y=-2
\end{cases}
$$
### example2
find solution
$$
y'=(2x+1)(y^2-2y-8)
$$
解：
$$
\dfrac{dy}{(y-4)(y+2)}=(2x+1)dx\\
\int\dfrac{dy}{(y-4)(y+2)}=\dfrac{1}{6}\int\dfrac{1}{y-4}-\dfrac{1}{y+2}dy=\dfrac{1}{6}ln\vert y-4\vert-\dfrac{1}{6}ln\vert y+2\vert +C_1\\
\int 2x+1dx=x^2+x+C_2\\
\dfrac{1}{6}ln\vert y-4\vert-\dfrac{1}{6}ln\vert y+2\vert=x^2+x+C_3\\
ln\dfrac{\vert y-4\vert}{\vert y+2\vert}=6x^2+6x+C_4\\
\dfrac{\vert y-4\vert}{\vert y+2\vert}=e^{6x^2+6x+C_4}=C_5e^{6x^2+6x}\\
\dfrac{y-4}{ y+2}=C_6e^{6x^2+6x}\\
y(1-C_6e^{6x^2+6x})=2C_6e^{6x^2+6x}+4\\
y=\dfrac{2C_6e^{6x^2+6x}+4}{1-C_6e^{6x^2+6x}}----->\begin{cases}
C_6=0,y=4\\
C_6\rightarrow \infin,y=-2\\
\end{cases}
$$
### logistic equation
方程
$$
\dfrac{dy}{dt}=r(1-\dfrac{y}{Limit})y
$$
为logistic equation
其中，r为增长系数，Limit为物种数量上限
设其初值为(0,P_0)，则
$$
y(t)=\dfrac{P_0Limite^{rt}}{(Limit-P_0)+P_0e^{rt}}
$$
拐点与增长率最高点
$$
y''=0\\
解得t=\dfrac{1}{r}ln\dfrac{Limit-P_0}{P_0}\\
带入y得到y=\dfrac{Limit}{2}\\
$$
即得到，在人口$y$达到$Limit$一半时，其增长率(导数)最大。
### threshold population
$$
y'=r(1-\dfrac{y}{Limit})(\dfrac{y}{Threshold}-1)y
$$
物种数量不能少于threshold，否则无法存活
三个平衡解:
$$
y=0\\
y=Limit\\
y=Threshold\\
\begin{cases}
当y\in (0,Threshold),y'<0\\
当y\in (Threshold,Limit),y'>0\\
当y\in (Limit,+\infin),y'<0
\end{cases}
$$
故$y=Threshold$是渐进非稳定解，$y=0$是渐进稳定解
### first-order equations
#### first-order linear equation
A first-order differential equation is linear if it can be written in the form
$$
a(x)y'+b(x)y=c(x)
$$
where a(x), b(x), and c(x) are arbitrary functions of x.
and its standard form is 
$$
y'+p(x)y=q(x)
$$
#### 求解
左右两边同时乘以$u(x)$
$$
u(x)y'+u(x)p(x)y=q(x)u(x)
$$
我们需要找到这样一个$u(x)$，使得$u'(x)=u(x)p(x)$，这样就有
$$
u(x)y'+u(x)p(x)y=u(x)y'+u'(x)y=[u(x)y]'
$$
原方程就可以改写为
$$
[u(x)y]'=q(x)u(x)
$$
解这个方程得到
$$
u(x)y=\int q(x)u(x)dx+C
$$
所以
$$
y=\dfrac{\int q(x)u(x)dx+C}{u(x)}
$$
为了找到$u(x)$，求解方程$u'(x)=u(x)p(x)$
$$
\int \dfrac{1}{u}du=\int p(x)dx\\
ln\vert u\vert+C_1=P(x)+C_2\\
ln\vert u\vert=P(x)+C_3\\
\vert u\vert=C_4e^{P(x)}\\
u=C_5e^{P(x)}
$$
**此处$P(x)$为任意原函数**
带入原方程有
$$
y=\dfrac{\int q(x)C_5e^{P(x)}dx+C}{C_5e^{P(x)}}=\dfrac{\int q(x)e^{P(x)}dx+C}{e^{P(x)}}
$$
#### example
求解
$$
xy'+3y=4x^2-3x,x>0
$$
写成标准式子
$$
y'+\dfrac{3}{x}y=4x-3
$$
求解$u(x)$:
$$
u(x)=e^{P(x)}=e^{\int {\dfrac{3}{x}dx}}=e^{3ln\vert x\vert}=\vert x\vert^3=x^3
$$
求解$\int q(x)u(x)dx$
$$
\int (4x-3)x^3dx=\int 4x^4-3x^3dx=\dfrac{4}{5}x^5-\dfrac{3}{4}x^4+C
$$
故原方程得解为
$$
y=\dfrac{\dfrac{4}{5}x^5-\dfrac{3}{4}x^4+C_1}{x^3}=\dfrac{4}{5}x^2-\dfrac{3}{4}x+C_1x^{-3}(x>0)
$$
#### example2
解方程
$$
y'+3y=2x-1,y(0)=3
$$
解：
$$
u(x)=e^{\int 3dx}=e^{3x}\\
\begin{aligned}
\int q(x)u(x)dx&=\int (2x-1)e^{3x}dx\\
&=\int \dfrac{1}{3}\dfrac{2}{3}\dfrac{3}{2}2xe^{3x}d3x-\int \dfrac{1}{3}e^{3x}d3x\\
&=\dfrac{2}{9}e^{3x}(3x-1)-\dfrac{1}{3}e^{3x}\\
\end{aligned}\\
y=\dfrac{\dfrac{2}{9}e^{3x}(3x-1)-\dfrac{1}{3}e^{3x}+C}{e^{3x}}=\dfrac{2}{9}(3x-1)-\dfrac{1}{3}+\dfrac{C}{e^{3x}}\\
y(0)=3--->C-\dfrac{5}{9}=3--->C=\dfrac{32}{9}
$$
## Sequence
### 等差
$$
a_i = c,a_n=a_{n-1}+d\\
a_n=dn+(c-d),n=i,i+1,...\\
\sum_i^n a_j=\dfrac{(a_i+a_n)(n-i+1)}{2}
$$
### 等比
$$
a_i = c,a_n=qa_{n-1}\\
a_n=q^{n-i}c,n=i,i+1,...\\
\sum_i^n a_j=\dfrac{a_i(1-q^{n-i+1})}{1-q}
$$
### The limit of sequence
A sequence $\{a_n\}$ converges to a real number L if for all $ε > 0$, there exists an integer N such that $|an − L| < ε$ if $n ≥ N$. The number L is the limit of the sequence and we write
$$
\lim_{n\rightarrow \infin}a_n=L
$$
### Limit of a Sequence Defined by a Function
Consider a sequence $\{an\}$ such that $a_n = f (n)$ for all $n ≥ 1$. If there exists a real number L such that
$$
\lim_{x\rightarrow \infin}f(x)=L
$$
then $\{a_n\}$ converges and
$$
\lim_{n\rightarrow \infin}a_n=L
$$
反之不成立
### several conclusions
$$
r^n\rightarrow 0,-1<r<1,n\rightarrow \infin\\
r^n\rightarrow 1,r=1,n\rightarrow \infin\\
r^n\rightarrow \infin,r\in (-\infin,-1)\cup(1,+\infin),n\rightarrow \infin\\
$$
### 数列极限运算法则
Given sequences $\{an\}$ and $\{bn\}$ and any real number c, if there exist constants A and B such that $\lim_{n→ ∞}a_n = A$ and $\lim_{n→ ∞} b_n = B$, then
$$
\lim_{n\rightarrow \infin}c=c\\
\lim_{n\rightarrow \infin}ca_n=cA\\
\lim_{n\rightarrow \infin}(a_n\pm b_n)=A\pm B\\
\lim_{n\rightarrow \infin}(a_n\times b_n)=AB\\
\lim_{n\rightarrow \infin}(\dfrac{a_n}{b_n})=\dfrac{A}{B},provided\quad B\neq 0\quad and\quad each\quad b_n\neq 0
$$
### Continuous functions defined on convergent sequences
Consider a sequence $\{an\}$ and suppose there exists a real number L such that the sequence $\{an\}$ converges to L. Suppose f is a continuous function at L. Then there exists an integer N such that f is defined at all values an for $n ≥ N$, and the sequence $f (a_n)$ converges to $f (L)$
### example
find the limits
$$
\{cos(\dfrac{3}{n^2})\},\lim_{x\rightarrow 0^+}cosx\\
\{cos((-1)^n\dfrac{3}{n^2})\},\lim_{x\rightarrow 0}cosx\\
\
\\
\{\sqrt{\dfrac{2n+1}{3n+5}}\}
$$
### 数列夹逼准则
Consider sequences $\{an\}$,$\{bn\}$, and $\{cn\}$. Suppose there exists an integer N such that
$$
a_n\leq b_n\leq c_n,n\geq N
$$
and if 
$$
\lim_{n\rightarrow \infin}a_n=L=\lim_{n\rightarrow \infin}c_n
$$
then
$$
\lim_{x\rightarrow \infin}b_n=L
$$
### example
$$
\lim_{n\rightarrow \infin}\dfrac{2n-sinn}{n}
$$
### Bounded sequences
A sequence $\{an\}$ is bounded above if there exists a real number M such that
$$
a_n\leq M
$$
for all positive integers n.
A sequence $\{an\}$ is bounded below if there exists a real number M such that
$$
M\leq a_n
$$
for all positive integers n.
A sequence $\{an\}$ is a **bounded sequence** if it is bounded above and bounded below.
### example
$$
\{\dfrac{1}{n}\}\\
\{2^n\}
$$
### 收敛数列必有界
### Monotone(单调) sequence
if sequence
$$
a_n\geq a_{n-1}
$$
or
$$
a_n\leq a_{n-1}
$$
for all $n\geq N_0$
then $\{a_n\}$is a monotone sequence
### 单调收敛定理
如果数列有界并对$n\geq N_0$后都单调，那么数列收敛
### 通过递推公式求数列极限
1. 审敛并求极限
$$
a_n=\dfrac{4^n}{n!}
$$
数列$a_n$当$n\geq 5$时，有
$$
a_n=\dfrac{4}{n}a_{n-1}<a_{n-1}
$$
因此数列递减，并且有下界0，故数列收敛，所以有
$$
\lim_{n\rightarrow \infin}a_n=\lim_{n\rightarrow \infin}a_{n-1}=L
$$
故$n\rightarrow \infin$时
$$
L=\dfrac{4}{n}L=0
$$
2. 审敛并求极限
$$
a_1=2,a_{n+1}=\dfrac{a_n}{2}+\dfrac{1}{2a_n}
$$
## infinite Sequence(无穷级数)
An infinite series is a sum of infinitely many terms and is written in the form
$$
\sum^\infin  a_n=a_1+a_2+...+a_n
$$
For each positive integer k, the sum
$$
S_k=\sum^ka_n=a_1+...+a_k
$$
is called the kth **partial sum** of the infinite series. The partial sums form a sequence $\{S_k\}$.If the sequence of partial sums converges to a real number S, the infinite series converges. If we can describe the convergence of a series to S, we call S the sum of the series, and we write
$$
\sum_\infin a_n=S
$$
If the sequence of partial sums diverges, we have the divergence of a series.
### 角标代换
给定数列$\{a_n\}$，$n=a,a+1,...$
现要将角标$n$的范围改为$n=b,b+1,b+2,...$
$$
a_n=f(n),n=0,1,2,3,...\Rightarrow a_n=f(n-b),n=b,b+1,b+2,...\\
S_n=f(n),n=a,a+1,a+2,...\Rightarrow S_n=f(n+a-b),n=b,b+1,b+2,...\\
$$
### 连和角标代换
$$
令m=n-a+b=b\\
\sum_{n=a}^\infin f(n)=\sum ^\infin_{n=m+a-b}f(n)=\sum_{n=b}^\infin f(n+a-b)
$$
### example
$$
\sum_5^\infin \dfrac{1}{2^{n-5}}=\sum_1^\infin \dfrac{1}{2^{n+5-1-5}}=\sum_1^\infin \dfrac{1}{2^{n-1}}\\
\sum_{22}^\infin (-1)^n\dfrac{n^2-3}{n!}=\sum_1^\infin (-1)^{n+22-1}\dfrac{(n+22-1)^2-3}{(n+22-1)!}=\sum_1^\infin (-1)^{n+21}\dfrac{(n+21)^2-3}{(n+21)!}\\
$$
### algebraic properties of convergent series
let $\sum^\infin a_n$ and $\sum^\infin b_n$ be convergent series. Then the following algebraic properties hold.
1. $\sum^\infin (a_n\pm b_n)$ **converges** and $\sum^\infin (a_n\pm b_n)=\sum^\infin a_n\pm \sum^\infin b_n$
2. $\sum^\infin ca_n$ **converges** and $\sum^\infin ca_n=c\sum^\infin a_n$
### 两个无穷级数
$$
\sum_1 \dfrac{1}{n(n+1)}=1\\
\sum_1 q^{n-1}=\dfrac{1}{1-q},\vert q\vert<1
$$
### example
$$
\sum_1^\infin \dfrac{(-3)^{n+1}}{4^{n-1}}\\
\sum_1^\infin (\dfrac{2}{3})^{2n}
$$
### 计算Koch 雪花
假设边长为a
大三角形面积为$S=\dfrac{\sqrt{3}}{4}a^2$
设数列$\{F_n\}$，$n=1,2,3,...$为面积增量
$$
F_1=(\dfrac{a}{3})^2\dfrac{\sqrt{3}}{{4}}\times \overbrace{3}^{新增小三角个数}\\
F_2=(\dfrac{a}{3^2})^2\dfrac{\sqrt{3}}{{4}}\times 3*4\\
F_3=(\dfrac{a}{3^3})^2\dfrac{\sqrt{3}}{{4}}\times 3*4*4\\
\vdots\\
F_n=(\dfrac{a}{3^n})^2\dfrac{\sqrt{3}}{{4}}\times 3*4^{n-1}
$$
故总面积为
$$
\begin{aligned}
S&=\dfrac{\sqrt{3}}{4}a^2+\sum^\infin_1 F_n\\
&=\dfrac{\sqrt{3}}{4}a^2+3\dfrac{\sqrt{3}}{4}a^2\sum^\infin_1\dfrac{4^{n-1}}{3^{2n}}\\
&=\dfrac{\sqrt{3}}{4}a^2+3\dfrac{\sqrt{3}}{4}a^2\sum_1^\infin (\dfrac{4}{3^2})^{n-1}\dfrac{1}{3^2}\\
&=\dfrac{\sqrt{3}}{4}a^2+\dfrac{3\sqrt{3}}{20}a^2\\
&=\dfrac{2\sqrt{3}}{5}a^2
\end{aligned}\\
$$
### 伸缩级数
设有数列$\{bn\}$
$$
\sum^k [b_n-b_{n+1}]=b_1-b_{k+1}\\
\begin{aligned}
\sum^k [b_n-b_{n+c}]&=b_1-b_{c+1}+...+b_k-b_{c+k}\\&=b_1+b_2+...+b_{c}-b_{c+k-c+1}-b_{c+k-c+2}-...-b_{c+k}\\
&=\sum^c_1 b_n-\sum^k_{k-c+1}b_{n+c}(展开的正项前c个-负项后c个)
\end{aligned}\\
$$
当$k\rightarrow \infin$时
$$
\sum^\infin [b_n-b_{n+c}]=\sum^cb_n
$$
### example
$$
\sum \dfrac{1}{n(n-1)}=1\\
\
\\
\begin{aligned}
\sum \dfrac{1}{n(n-2)}&=\dfrac{1}{2}\sum \bigg(\dfrac{1}{n-2}-\dfrac{1}{n}\bigg)\\&=\dfrac{1}{2}\sum (b_{n-2}-b_n)\\&=\dfrac{1}{2}\sum_1(b_{n+3-1-2}-b_{n+3-1})\\&=\dfrac{1}{2}\sum_1(b_{n}-b_{n+2})\\&=\dfrac{1}{2}(b_1+b_2)=\dfrac{3}{4}\\
\end{aligned}
$$
$$
\sum \dfrac{1}{n(n\pm b)}=\sum\dfrac{1}{b}\bigg(
\begin{cases}
\dfrac{1}{n\pm b}-\dfrac{1}{n}，n\pm b<n\\
\\
\dfrac{1}{n}-\dfrac{1}{n\pm b}，n\pm b>n\
\end{cases}
\bigg)=\dfrac{1}{b}\sum_{i=1}^b\dfrac{1}{i}\\
$$
### 欧拉常数
$$
\lim_{k\rightarrow \infin}T_k=\lim_{k\rightarrow \infin}\sum^k_{n=1}(\dfrac{1}{n})-lnk=\gamma=\int_1^\infin \bigg(\dfrac{1}{\lfloor x\rfloor}-\dfrac{1}{x}\bigg)dx
$$
page 473
证明$T_k-\gamma\leq \dfrac{1}{k}$
1. 证明$ln(k+1)-lnk\leq \dfrac{1}{k}$
$$
ln(k+1)-lnk=(ln(\xi))'(k+1-k)=\dfrac{1}{\xi}<\dfrac{1}{k},\xi\in (k,k+1)
$$
2. 证明对于任意整数k
$$
T_k-T_{k+1}<\dfrac{1}{k}-\dfrac{1}{k+1}
$$
证明：
$$
\begin{aligned}
\sum^k(\dfrac{1}{n})-lnk-\sum^{k+1}(\dfrac{1}{n})+ln(k+1)&=-\dfrac{1}{k+1}-[lnk-ln(k+1)]\\
&<-\dfrac{1}{k+1}-(\dfrac{1}{-k})\\
&=\dfrac{1}{k}-\dfrac{1}{k+1}
\end{aligned}
$$
3. 对任意大于k的整数j，有
$$
\begin{aligned}
T_k-T_j&=T_k-T_{k+1}+T_{k+1}-T_{k+2}+...+T_{j-1}+T_j\\
&<\dfrac{1}{k}-\dfrac{1}{k+1}+\dfrac{1}{k+1}-\dfrac{1}{k+2}+...+\dfrac{1}{j-1}-\dfrac{1}{j}\\
&=\dfrac{1}{k}-\dfrac{1}{j}
\end{aligned}
$$
4. 当$j\rightarrow \infin$，有
$$
T_k-T_j=T_k-\gamma \leq \dfrac{1}{k}(<一定\leq)
$$
## 发散测试和积分审敛
### Divergence test
if $\lim_{n\rightarrow \infin}a_n=c\neq 0$ or $\lim_{n\rightarrow \infin}a_n$ does not exist, then the series $\sum_{n=1}^\infin a_n$ diverges.
It is important to note that the converse of this theorem is not true. (that is if $\lim_{n\rightarrow \infin}a_n= 0$, we can not say $\sum_{n=1}^\infin a_n$ converge)
### integral test
This test, called the integral test, **compares an infinite sum to an improper integral**.
It is important to note that this test can only be applied when we are considering a series whose terms **are all positive**.
### example
$$
\begin{aligned}
\sum_1^k  \dfrac{1}{n}&=\sum_1^k (\dfrac{1}{n}\times 1)\\&=1*1+\dfrac{1}{2}*1+...+\dfrac{1}{k}*1\\&=S_{[1',2]}+S_{[2',3]}+...+S_{[k',k+1]}\\&>\int_1^{k+1}\dfrac{1}{x}dx\\&=lnx\vert^{k+1}_1\\&=ln(k+1)
\end{aligned}
$$
### example 2
$$
\sum_1^k\dfrac{1}{n^2}=S_{[1',2]}+S_{[2',3]}+...+S_{[k',k+1]}>\int_1^{k+1}\dfrac{1}{x^2}dx=1-\dfrac{1}{k+1}\\
\sum_1^k\dfrac{1}{n^2}=1+S_{[1,2']}+S_{[2,3']}+...+S_{[k-1,k']}<1+\int_1^k\dfrac{1}{x^2}dx=2-\dfrac{1}{k}
$$
### 积分审敛
suppose $\sum_1^\infin a_n$ is a series with positive terms an such that there exists a **continuous**, **positive**, **decreasing** function f where $f(n)=a_n$ for all positive integers. Then
$$
S_k=a_1+a_2+...+a_k>\int_1^{k+1}f(x)dx
$$
此时取f的左端点值
and also
$$
S_k=a_1+a_2+...+a_k<a_1+\int_1^kf(x)dx
$$
此时取f的右端点值
当$k\rightarrow \infin$时
$$
\lim_{k\rightarrow \infin}S_k>\lim_{k\rightarrow \infin}\int_1^{k+1}f(x)dx=\int_1^\infin f(x)dx>\infin
$$
$S_k$发散
$$
\lim_{k\rightarrow \infin}S_k<a_1+\lim_{k\rightarrow \infin}\int_1^k f(x)dx=a_1+\int_1^\infin f(x)dx=L
$$
$S_k$收敛
因此有
$$
\int_1^\infin f(x)dx收敛，S_k收敛\\
\int_1^\infin f(x)dx发散，S_k发散\\
$$
### 积分审敛定义
suppose $\sum_{n=1}^\infin a_n$ is a series with positive terms $a_n$. Suppose there exists a function f and a positive integer N such that the following three conditions are satisfied
1. f is continuous
2. f is decreasing
3. $f(n)=a_n$ for all integers $n\geq N$

then
$$
\sum_{n=1}^\infin a_n\quad and\quad\int_N^\infin f(x)dx
$$
both converge and diverge
这里的$N$只需要小于等于1并且连续即可，如果$f(x)$在$x=0$上连续，则
$$
\sum_{n=1}^\infin a_n\quad and\quad\int_0^\infin f(x)dx
$$
both converge and diverge
### p级数
For any real number p, the series
$$
\sum_{n=1}^\infin\dfrac{1}{n^p}
$$
is called a p-series.
$$
\sum_{n=1}^\infin\dfrac{1}{n^p}
\begin{cases}
converges,p>1\\
diverges,p\leq 1
\end{cases}
$$
### estimating the value
Suppose $a_n$ converges and we want to use $\sum_1^N a_n$ to approximate $\sum_1^\infin a_n$, $R_N=\sum_1^\infin a_n-\sum_1^N a_n=\sum_{N+1}^\infin a_n$ serve as an index to judge how is the approximation going
We are able to use the ideas from the integral test to estimate $R_N$ if $a_n$ is **positive and decreasing**
Suppose there exists a function f satisfying the following three conditions:
1. f is continuous
2. f is decreasing
3. $f(n)=a_n$ for $n\geq 1$

then
$$
S_N+\int_{N+1}^\infin f(x)dx<\sum_1^\infin a_n<S_N+\int_N^\infin f(x)dx\\
\int_{N+1}^\infin f(x)dx<R_N<\int_N^\infin f(x)dx
$$
级数大的取左值，级数小的取右值
## 比较审敛
Suppose there exists an integer N such that $0 ≤ a_n ≤ b_n$ for all $n ≥ N$. if $\sum_1^\infin b_n$  converges, then $\sum_1^\infin a_n$ converges.
Suppose there exists an integer N such that $a_n ≥ b_n ≥ 0 $ for all $n ≥ N$. if $\sum_1^\infin b_n$  diverges, then $\sum_1^\infin a_n$ diverges.
### 极限比较测试
 Consider two series $\sum a_n$ and $\sum b_n$ with positive $a_n$ and $b_n$ and evaluate
$$
\lim_{n\rightarrow \infin}\dfrac{a_n}{b_n}
$$
if
$$
\lim_{n\rightarrow \infin}\dfrac{a_n}{b_n}=L\neq 0
$$
then for n sufficiently large, $a_n \approx Lb_n$. Therefore, 
$$
\sum^\infin a_n=\sum^N a_n+\sum^\infin_{N+1} a_n\approx \sum^N a_n + \sum^\infin_{n+1} Lb_n
$$
thus, either both converge or both diverge.
**definition**
Let $a_n, b_n ≥ 0$ for all $n ≥ 1$.
1. $\lim_{n\rightarrow \infin}\dfrac{a_n}{b_n}=L\neq 0$, then$\sum^\infin a_n$ and $\sum^\infin b_n$ both converge or diverge.
2. $\lim_{n\rightarrow \infin}\dfrac{a_n}{b_n}= 0$ and $\sum^\infin b_n$ converges, then $\sum^\infin a_n$ converges.
3. $\lim_{n\rightarrow \infin}\dfrac{a_n}{b_n}= \infin$ and $\sum^\infin b_n$ diverges then $\sum^\infin a_n$ diverges.
### example
$$
\sum \dfrac{1}{\sqrt{n}+1}\\
\sum \dfrac{ln(n)}{n^2}
$$
### Alternating series test
Any series whose terms alternate between positive and negative values is called an alternating series. An alternating series can be written in the form
$$
\sum_1^\infin (-1)^{n+1}b_n=b_1-b_2+b_3-b_4+...\\
\sum_1^\infin (-1)^{n}b_n=-b_1+b_2-b_3+b_4+...\\
$$
Where $b_n ≥ 0$ for all positive integers n.
### Alternating harmonic series
$$
\sum_1^\infin \dfrac{(-1)^{n+1}}{n}=1-\dfrac{1}{2}+\dfrac{1}{3}-\dfrac{1}{4}+...
$$
证明alternating调和级数收敛
对所有奇数项和
$$
\begin{aligned}
S_{2k+1}&=1-\dfrac{1}{2}+\dfrac{1}{3}-\dfrac{1}{4}+...-\dfrac{1}{2k}+\dfrac{1}{2k+1}\\
&=1-\dfrac{1}{2}+\dfrac{1}{3}-\dfrac{1}{4}+...-\dfrac{1}{2k-2}+\dfrac{1}{2k-1}-\dfrac{1}{2k}+\dfrac{1}{2k+1}\\
&=S_{2k-1}-\dfrac{1}{2k}+\dfrac{1}{2k+1}\\
&<S_{2k-1}
\end{aligned}
$$
therefore,$\{S_{2k+1}\}$ is a decreasing sequence, also
$$
S_{2k+1}=(1-\dfrac{1}{2})+(\dfrac{1}{3}-\dfrac{1}{4})+...+(\dfrac{1}{2k-1}-\dfrac{1}{2k})+\dfrac{1}{2k+1}>0
$$
therefore, $\{S_{2k+1}\}$ is bounded below.
对所有偶数项和
$$
\begin{aligned}
S_{2k}&=1-\dfrac{1}{2}+\dfrac{1}{3}-\dfrac{1}{4}+...+\dfrac{1}{2k-1}-\dfrac{1}{2k}\\
&=\dfrac{1}{2}+\dfrac{1}{3}-\dfrac{1}{4}+...+\dfrac{1}{2k-3}-\dfrac{1}{2k-2}+\dfrac{1}{2k-1}-\dfrac{1}{2k}\\
&=S_{2k-2}+\dfrac{1}{2k-1}-\dfrac{1}{2k}\\
&>S_{2k-2}
\end{aligned}
$$
therefore,$\{S_{2k}\}$ is a increasing sequence, also
$$
S_{2k}=1-[(\dfrac{1}{2}-\dfrac{1}{3})+(\dfrac{1}{4}-\dfrac{1}{5})...+(\dfrac{1}{2k}-\dfrac{1}{2k-1})]-\dfrac{1}{2k}<1
$$
Therefore, by the Monotone Convergence Theorem, the sequence $S_{2k}$ also converges.
since
$$
S_{2k+1}=S_{2k}+\dfrac{1}{2k+1}
$$
let $k\rightarrow \infin$
$$
\lim_{k\rightarrow \infin}S_{2k+1}=\lim_{k\rightarrow  \infin}S_{2k}+\lim_{k\rightarrow \infin}\dfrac{1}{2k+1}\\
$$
thus
$$
\lim_{k\rightarrow \infin}S_{2k+1}=\lim_{k\rightarrow  \infin}S_{2k}
$$
因此所有奇数和和偶数和收敛于同一值，因此整个数列收敛
参考数列
$$
a_{2n-1}=2^n\\
a_{2n}=-2^n\\
\
\\
S_{2k-1}=2^n\\
S_{2k}=0
$$
级数$\sum^\infin a_n=S_n$不存在
### Alternating Series Test
An alternating series of the form $\sum_1^\infin (-1)^{n+1}b_n$ and $\sum_1^\infin (-1)^{n}b_n$ converges if
1. $0\leq b_{n+1}\leq b_n$ for all $n\geq 1$
2. $\lim_{n\rightarrow \infin}b_n = 0$

This is known as the alternating series test.
### Remainder of an alternating series
Consider an alternating series of the form $\sum_1^\infin (-1)^{n+1}b_n$ and $\sum_1^\infin (-1)^nb_n$ that satisfies the hypotheses of the alternating series test. Then
$$
R_N=\lim_{k\rightarrow \infin}\sum_1^k (-1)^{n+1}b_n-\sum_1^N(-1)^nb_n=S-S_N
$$
依据图，每加下一项都会“超过”收敛值，因此有
$$
\vert R_N\vert = \vert S-S_N\vert\leq b_{N+1}
$$
page 506
### 绝对和条件收敛
A series $\sum_1^\infin a_n$ exhibits **absolute convergence** if $\sum_1^\infin \vert a_n\vert$ converges.
A series $\sum_1^\infin a_n$ exhibits **conditional convergence** if $\sum_1^\infin a_n$ converges but $\sum_1^\infin \vert a_n\vert$ diverges.
### 绝对收敛implies convergence
if $\sum_1^\infin \vert a_n\vert$ converges, then $\sum_1^\infin a_n$ converges.
### Rearrangement of alternating series
$$
\sum^\infin (-1)^{n+1}\dfrac{1}{n}=ln2\\
\sum_{n=1}^\infin \dfrac{1}{2}a_n=\dfrac{1}{2}-\dfrac{1}{4}+\dfrac{1}{6}-...=\dfrac{1}{2}\sum_{n=1}^\infin a_n =\dfrac{ln2}{2}\\
$$
introduce $\sum b_n$ that
$$
b_n=\begin{cases}
\dfrac{a_n}{2},n=2k,k=1,2,3,...\\
0,n=2k-1,k=1,2,3,...\\
\end{cases}
$$
thus
$$
\sum_{n=1}^\infin b_n=0+\dfrac{1}{2}+0+\dfrac{1}{4}+0+...=\dfrac{ln2}{2}
$$
therefore,
$$
\sum_{n=1}^\infin(a_n+b_n)=\sum_1^\infin a_n+\sum_1^\infin b_n=ln2+\dfrac{ln2}{2}=\dfrac{3ln2}{2}
$$
expand the series we get
$$
\sum^\infin (a_n+b_n)=1+(-\dfrac{1}{2}+\dfrac{1}{2})+(\dfrac{1}{3}+0)+...=1+\dfrac{1}{3}-\dfrac{1}{2}+\dfrac{1}{5}+\dfrac{1}{7}-\dfrac{1}{4}+...=\dfrac{3ln(2)}{2}
$$
## Ratio and root test
From our earlier discussion and examples, we know that $\lim_{n\rightarrow \infin}a_n = 0$ is not a sufficient condition for the series to converge. Not only do we need $a_n → 0$, but we need $a_n → 0$ quickly enough. 
### Ratio test
Let $\sum_{n=1}^\infin a_n$ be a series with **nonzero**(有除法，要做分母) terms. Let
$$
\rho =\lim_{n\rightarrow \infin}\vert \dfrac{a_{n+1}}{a_n}\vert
$$
1. if $0\leq\rho\leq 1$, then $\sum_{n=1}^\infin a_n $**converges absolutely**.
2. if $\rho> 1 $, then $\sum_{n=1}^\infin a_n$ diverges.
3. if $\rho = 1$, the test does not provide any information.

Proof
**for sufficiently large N, $a_{N+1}\approx a_{N}\times \rho$**
**Part 1**
Since $0 ≤ ρ < 1$, there exists R such that $0 ≤ ρ < R < 1$. Let $ε = R − ρ > 0$. By the definition of limit of a sequence, there exists some integer N such that
$$
\vert\vert\dfrac{a_{n+1}}{a_n}\vert-\rho\vert<ε，n\geq N\\
\vert\vert\dfrac{a_{n+1}}{a_n}\vert\vert-\vert \rho\vert\leq \vert\vert\dfrac{a_{n+1}}{a_n}\vert-\rho\vert<ε\\
\vert\dfrac{a_{n+1}}{a_n}\vert< ε+\rho=R
$$
therefore,
$$
\vert a_{N+1}\vert\leq R\vert a_N\vert\\
\vert a_{N+2}\vert\leq R\vert a_{N+1}\vert\leq R^2\vert a_N\vert\\
\vdots\\
$$
since $R<1$,
$$
\sum_N \vert a_n\vert<R\vert a_N\vert + R^2\vert a_{N}\vert+R^3\vert a_{N}\vert+...
$$
thus $\sum_N^\infin \vert a_n\vert $converge
therefore $\sum^\infin \vert a_n\vert =\sum^N \vert a_n\vert+\sum^\infin_{N+1}\vert a_n\vert$ converges, $\sum^\infin a_n$ converge.
**Part 2**
since $\rho >1$, there exists R such that $ρ > R > 1$. Let $ε = ρ − R > 0$.  By the definition of the limit of a sequence, there exists an integer N such that
$$
\vert\vert\dfrac{a_{n+1}}{a_n}\vert-\rho\vert<ε，n\geq N\\
-\vert\vert\dfrac{a_{n+1}}{a_n}\vert-\rho\vert>ε\\
\vert\vert\dfrac{a_{n+1}}{a_n}\vert\vert-\vert \rho\vert\geq -\vert\vert\dfrac{a_{n+1}}{a_n}\vert-\rho\vert>ε\\
\vert\dfrac{a_{n+1}}{a_n}\vert>ε+\rho>\rho-ε=R
$$
thus
$$
\vert R_{N+1}\vert >R\vert a_N\vert\\
\vert R_{N+2}\vert >R\vert a_{N+1}\vert>R^2\vert a_N\vert\\
\vdots\\
\sum_N\vert a_n\vert>R\vert a_N\vert + R^2\vert a_{N}\vert+R^3\vert a_{N}\vert+...
$$
since $R>1$, $\sum^\infin_N\vert a_n\vert$ diverges
if all $a_n$ are positive, then $\sum^\infin_1 a_n$ is diverge. Otherwise, let $f(n)=\begin{cases}1\\-1\end{cases}$, then $\sum^\infin_1 a_n=\sum_1^\infin f(n)\vert a_n\vert$ for $\vert R_{N}\vert<\vert R_{N+1}\vert<\vert R_{N+2}\vert<...$, thus $\sum_1^\infin a_n$ diverge.

The ratio test is particularly useful for series whose terms contain **factorials** or **exponentials**.
### Root test
Consider series $\sum_{n-1}^\infin a_n$. Let
$$
\rho = \lim_{n\rightarrow \infin}\sqrt[n]{\vert a_n\vert}
$$
1. if $0 ≤ ρ < 1$, then $\sum^\infin a_n $ **converges absolutely**
2. If $ρ > 1$ or $ρ = ∞$, then $\sum^\infin a_n $ diverges.
3. If $ρ = 1$, the test does not provide any information.

Proof
The approach of the root test is similar to that of the ratio test.
if for series $\sum^\infin a_n$ has $\rho = \lim_{n\rightarrow \infin}\sqrt[n]{\vert a_n\vert}$ for real numbers, then for sufficiently large N, $\vert a_N\vert\approx \rho^N$, then
$$
\vert a_N\vert + \vert a_{N+1}\vert+\vert a_{N+2}\vert+...\approx \rho^N+\rho^{N+1}+...
$$
thus if $0 ≤ ρ < 1$, $\sum^\infin \rho^n$ converges, therefore $\sum^\infin a_n$ converges
if $ρ > 1$ or $ρ = ∞$, $\sum^\infin \rho^n$ diverges, therefore $\sum^\infin \vert a_n\vert$ diverges, for $\vert a_N\vert<\vert a_{N+1}\vert<...$, $\sum^\infin a_n$ diverges.
## Strategy to choose test
page 522
1. 熟悉的级数——等比
2. alternating？alternating test
3. comparison test and limit comparison test
4. if contain factorial or power, ratio test
5. if contain n power, root test
6. divergence test
7. integral test

## Power Series
A series of the form
$$
\sum_{n=0}^\infin c_nx^n = c_0+c_1x+c_2x^2+...
$$
is a power series centered at $x = 0$. A series of the form
$$
\sum_{n=0}^\infin c_n(x-a)^n=c_0+c_1(x-a)+c_2(x-a)^2+...
$$
is a power series centered at $x = a$.
**把x看成一个定值**
### convergence of a power series
Consider the power series $\sum_{n=0}^\infin c_n(x-a)^n$. The series satisfies **exactly one** of the following properties:
1. The series converges at $x=a$ and diverges for all $x\neq a$
2. The series converges for all real numbers x.
3. There exist a real number $R>0$ such that the series converges if $\vert x-a\vert<R$ and diverges if \vert x-a\vert >R. At the values x where $\vert x-a\vert =R$, the series may converge or diverge.

**引理**
If there exists a real number d ≠ 0 such that $\sum_0^\infin c_nd^n$ converges, then the series $\sum_0^\infin c_nx^n$ converges absolutely for all x such that $\vert x\vert<\vert d\vert$.

Proof
since $\sum_0^\infin c_nd^n$ converges, the $n^{th}$ term $c_nd^n\rightarrow 0$ as $n\rightarrow \infin$. Therefore, there exists an integer N such that $\vert c_nd^n\vert\leq 1$ for all $n\geq N$. We have
$$
\vert c_nx^n\vert = \vert c_nd^n\vert\vert\dfrac{x}{d}\vert^n
$$
thus for all $n\geq N$
$$
\
\vert c_nx^n\vert\leq \vert\dfrac{x}{d}\vert^n
$$
beacuse the series $\sum_N^\infin \vert \dfrac{x}{d}\vert^n$ converges at $\vert \dfrac{x}{d}\vert<1$, thus series $\sum_0^\infin c_nx^n$ converges at all $\vert x\vert<\vert d\vert$
**Proof**
let S be the set of real numbers for which the series converges. Suppose that the set $S = {0}$. Then the series falls under case i. 

Suppose that the set S is the set of all real numbers. Then the series falls under case ii. 

Suppose that $S ≠ {0}$ and S is not the set of real numbers. Then there exists a real number $x^* ≠ 0$ such that the series does not converge. Thus, the series cannot converge for any x such that $|x| > |x * |$. Therefore, the set S must be a bounded set, which means that it must have a smallest upper bound. (This fact follows from the Least Upper Bound Property for the real numbers, which is beyond the scope of this text and is covered in real analysis courses.) Call that smallest upper bound R. Since $S ≠ {0}$, the number $R > 0$. Therefore, the series converges for all x such that $|x| < R$, and the series falls into case iii.
### Radius of convergence
Consider the power series $\sum_{n=0}^\infin c_n(x-a)^n$. The set of real numbers x where the series converges is the **interval of convergence**. if there exists a real number $R > 0$ such that the series converges for $|x − a| < R$ and diverges for $x − a| > R$, then R is the **radius of convergence**.
If the series converges only at $x = a$, we say the radius of convergence is $R = 0$. If the series converges for all real numbers x, we say the radius of convergence is $R = ∞$.
### example
find the interval and radius of the convergence
$$
\sum_0^\infin \dfrac{x^n}{n!}\\
\sum_0^\infin n!x^n\\
\sum_0^\infin \dfrac{(x-2)^n}{(n+1)3^n}
$$
apply the ratio test
$$
\begin{aligned}
\rho &= \lim_{n\rightarrow \infin}\vert\dfrac{x^{n+1}}{(n+1)!}\dfrac{n!}{x^n}\vert\\
&=\lim_{n\rightarrow \infin}\vert\dfrac{x}{n+1}\vert\\
&=\vert x\vert\lim_{n\rightarrow \infin}\dfrac{1}{n+1}(将x看成定值)\\
&=0<1
\end{aligned}
$$
thus no matter what the x is the series $\sum_0^\infin \dfrac{x^n}{n!}$ converges, the radius of the convergence is R.
$$
\begin{aligned}
\rho &= \lim_{n\rightarrow \infin}\vert\dfrac{x^{n+1}(n+1)!}{x^n(n)!}\vert\\
&=\lim_{n\rightarrow \infin}\vert x(n+1)\vert\\
&=\vert x\vert\lim_{n\rightarrow \infin}(n+1)\\
&=\infin
\end{aligned}
$$
thus the series $\sum_0^\infin x^nn!$ only converges at 0, the radius of the convergence is 0.
$$
\begin{aligned}
\rho &= \lim_{n\rightarrow \infin}\vert\dfrac{(x-2)^{n+1}}{(n+2)3^{n+1}}\dfrac{(n+1)3^n}{(x-2)^n}\vert\\
&=\lim_{n\rightarrow \infin}\vert \dfrac{(x-2)}{3}\vert\\
&=\vert\dfrac{(x-2)}{3}\vert\\
\end{aligned}\\
$$
series $\sum_0^\infin \dfrac{(x-2)^n}{(n+1)3^n}$ converges at $\rho<1$, thus $\vert x-2\vert<3$. When $\rho = 1$, $x = 5,-1$, test series $\sum_0^\infin \dfrac{(5-2)^n}{(n+1)3^n}$ diverge and series $\sum_0^\infin \dfrac{(-1-2)^n}{(n+1)3^n}$ converge, combine with $x=2$ the series converge at $0\leq \vert x-2\vert\leq 3,x\neq 5$, the radius of convergence is 3.
### Representing Functions as power series
consider the series $\sum_0^\infin ax^n$
$$
\sum_0^\infin ax^n=a+ax+ax^2+ax^3+...\\
$$
if $\vert x\vert<1$, the series converges at
$$
\sum_0^\infin ax^n=\dfrac{a}{1-x}
$$
thus when $\vert x\vert<1$
$$
f(x)=\dfrac{1}{1-x}=\sum_0^\infin x^n=1+x+x^2+x^3+...
$$
### example
use power series to represent functions
$$
f(x)=\dfrac{1}{1-x^2}\\
f(x)=\dfrac{1}{1+x^3}\\
f(x)=\dfrac{x^2}{4-x^2}
$$
$$
f(x)=\dfrac{1}{1-x^2}=\dfrac{a}{1-q}=\sum^\infin aq^n=\sum^\infin x^{2n}(x\in (-1,1))\\
\
\\
f(x)=\dfrac{1}{1+x^3}=\dfrac{1}{1-(-x^3)}=\sum^\infin (-x^3)^n(x \in(-1,1))\\
\
\\
f(x)=\dfrac{x^2}{4-x^2}=-\dfrac{\dfrac{x^2}{4}}{1-\dfrac{x^2}{4}}=\sum^\infin_0 \dfrac{x^2}{4}(\dfrac{x^2}{4})^n(x \in(-2,2))
$$
**将x看成数**
### example2
use power series to represent functions
$$
f(x)=\dfrac{x^3}{2-x}\\
\
\\
f(x)=\dfrac{\dfrac{x^3}{2}}{1-\dfrac{x}{2}}=\sum^\infin_0\dfrac{x^3}{2}(\dfrac{x}{2})^n
$$
## Properties of Power series
suppose that the two power series $\sum^\infin_0 c_nx^n$ and $\sum_0^\infin d_nx^n$ converge to the functions f and g, respectively, on **the same** interval $I$.
1. the power series $\sum_0^\infin (c_nx^n\pm d_nx^n)$ converges to $f\pm g$ on $I$.
2. For any integer $m ≥ 0$ and any real number $b$, the power series $\sum_0^\infin bx^mc_nx^n$ converges to $bx^mf(x)$ on $I$.
3. For any integer $m ≥ 0$ and any real number $b$, the series $\sum_0^\infin c_n(bx^m)^n$ converges to $f(bx^m)$ for all x such that $bx^m$ is in $I$.

Similar results hold for power series centered at x = a.

### example
suppose the series $\sum_0^\infin a_nx^n$ converges at $(-1,1)$, and series $\sum_0^\infin b_nx^n$ converges at $(-2,2)$.
find the convergence interval of
$$
\sum_0^\infin (a_nx^n+b_nx^n)\\
\sum_0^\infin a_n3^nx^n\\
$$
### example2
find the series of functions
$$
f(x)=\dfrac{3x}{1+x^2}\\
f(x)=\dfrac{1}{(x-1)(x-3)}
$$
$$
f(x)=\dfrac{3x}{1+x^2}=3x*\dfrac{1}{1-(-x^2)}=\sum_0^\infin 3x(-x^2)^n=\sum_0^\infin 3(-1)^nx^{2n+1}\\
f(x)=-\dfrac{1}{2}\bigg(\dfrac{1}{x-1}-\dfrac{1}{x-3}\bigg)=-\dfrac{1}{2}\bigg(-\sum_0^\infin x^n+\sum_0^\infin \dfrac{1}{3}\bigg(\dfrac{x}{3}\bigg)^n\bigg)=\dfrac{1}{2}\sum_0^\infin x^n-\dfrac{1}{6}\sum_0^\infin\bigg(\dfrac{x}{3}\bigg)^n
$$
### Multiplication of power series
Suppose that the power series $\sum_{n=0}^\infin c_nx^n$ and $\sum_0^\infin d_nx^n$ converge to f and g, respectively, on a common interval $I$
Let
$$
e_n = c_0d_n+c_1d_{n-1}+...+c_{n-1}d_1+c_nd_0=\sum_{k=0}^n c_kd_{n-k}\\
\
\\
e_0=c_0d_0\\
e_1=c_0d_1+c_1d_0\\
角标相加等于1\\
e_2=c_0d_2+c_1d_1+c_2d_0\\
角标相加等于2
$$
It appears that the product should satisfy
$$
\begin{aligned}
\bigg(\sum_0^\infin c_nx^n\bigg)\bigg(\sum_0^\infin b_nx^n\bigg)&=(c_0+c_1x+c_2x^2+...)(d_0+d_1x+d_2x^2+...)\\
&=c_0d_0+(c_0d_1+c_1d_0)x+(c_0d_2+c_1d_1+c_2d_0)x^2+...\\
&=\sum_0^\infin e_nx^n
\end{aligned}
$$
and $\sum_0^\infin e_nx^n$ converges to $f(x)*g(x)$ on $I$.
The series $\sum_0^\infin e_nx^n$ is known as the Cauchy product of the series $\sum_0^\infin c_nx^n$ and $\sum_0^\infin b_nx^n$
### example
find the power series
$$
f(x)=\dfrac{1}{(1-x)(1-x^2)}
$$
**method 1**
$$
\dfrac{1}{1-x}=\sum^\infin_0 x^n\\
\dfrac{1}{1+x}=\sum^\infin_0 (-1)^nx^{n}\\
\
\\
\begin{aligned}
f(x)&=\dfrac{1}{1-x}\dfrac{1}{1-x}\dfrac{1}{1+x}\\
&=\sum_0^\infin x^n\sum_0^\infin x^n\sum_0^\infin (-1)^nx^n\\
&=(1+2x+3x^2+4x^3+...)\sum_0^\infin (-1)^nx^n\\
&=\sum_0^\infin (n+1)x^n\sum_0^\infin (-1)^nx^n\\
&=(1+[-1+2]x+[1-2+3]x^2+[-1+2-3+4]x^3+...)\\
&=(1+x+2x^2+2x^3+...)\\
&=\sum_{n=0}^\infin (-1)^n\bigg(\sum_{k=0}^{n}(-1)^{k}(k+1)\bigg)x^n
\end{aligned}
$$
**method 2**
$$
\dfrac{1}{1-x}=\sum^\infin_0 x^n\\
\dfrac{1}{1-x^2}=\sum^\infin_0 x^{2n}\\
\
\\
\begin{aligned}
f(x)&=\dfrac{1}{1-x}\dfrac{1}{1-x^2}\\
&=(1+x+x^2+x^3+x^4+...)(1+x^2+x^4+x^6+x^8+...)\\
&=(1+x^2+x^4+x^6+x^8+...)+(x+x^3+x^5+x^7+x^9+...)+\\&(x^2+x^4+x^6+x^8+x^{10}+...)+(x^3+x^5+x^7+x^9+x^{11}+...)+(x^4+x^6+x^8+x^{10}+x^{12})+...\\
&=1+2x^2+2x^3+3x^4+...
\end{aligned}
$$
要展开到$x^k$，则展开到
$$
(x^m+...+x^p)(x^q+...+x^n)\\
p+q\geq k\\
m+n\geq k\\
$$
thus, expand to x^3
$$
\begin{aligned}
f(x)&=\dfrac{1}{1-x}\dfrac{1}{1-x^2}\\
&=(1+x+x^2+x^3)(1+x^2+x^4)\\
&=(1+x+2x^2+2x^3+...)
\end{aligned}
$$
### Differentiating and integrating Power series
Suppose that the power series $\sum_0^\infin c_n(x-a)^n$ converges on the interval $(a-R,a+R)$ for some $R>0$. Let f be the function defined by the series
$$
\begin{aligned}
f(x)&=\sum_0^\infin c_n(x-a)^{n-1}\\
&=c_0+c_1(x-a)+c_2(x-a)^2+...
\end{aligned}
$$
for $\vert x-a\vert <R$. Then f is **differentiable** on the interval $(a − R, a + R)$ and we can find $f′$ by differentiating the series **term-by-term differentiation**:
$$
f'(x)=\sum_0^\infin \bigg(c_n(x-a)^{n-1}\bigg)'=\sum_1^\infin nc_n(x-a)^{n-1}
$$
for $|x − a| < R$. Also, to find $\int f(x)dx$, we can **integrate the series term-by-term**. The resulting series converges on $(a − R, a + R)$, and we have
$$
\int f(x)dx=C+\sum_0^\infin \int\bigg(c_n(x-a)^{n-1}\bigg)dx=C+\sum_0^\infin c_n\dfrac{(x-a)^{n+1}}{n+1}
$$
for $|x − a| < R$.
Term-by-Term Differentiation and Integration for Power Series guarantees **the same radius of convergence** when a power series is differentiated or integrated term-by-term.
But it says nothing about what happens at the **endpoints**.
### example
find a power series representation for $g(x)=\dfrac{1}{(1-x)^2}$, determine whether the resulting series converges at the endpoints.
$$
g(x)=f'(x)=\bigg(\dfrac{1}{1-x}\bigg)'=\sum_0^\infin (x^n)'=\sum_1^\infin nx^{n-1}=\sum_0^\infin (n+1)x^{n}
$$
for $\vert x\vert <1$. And series diverges at the endpoints of $\pm1$.
### example2
evaluate the series $\sum_0^\infin \dfrac{n+1}{4^n}$
$$
\sum_0^\infin (n+1)(\dfrac{1}{4})^n=\sum_0^\infin (n+1)(4^{-1})^{n}=\dfrac{1}{(1-(\dfrac{1}{4}))^2}=\dfrac{16}{9}
$$
### example3
For each of the following functions f, find a power series representation for f by integrating the power series for $f ′$ and find its interval of convergence.
$$
f(x)=ln(1+x)\\
f'(x)=\dfrac{1}{1+x}=\sum_0^\infin (-1)^nx^n\\
\int f'(x)dx = \sum_0^\infin \int\bigg((-1)^nx^n\bigg)=\sum_0^\infin (-1)^n\dfrac{x^{n+1}}{n+1}+C\\
当x=0时，f(0)=0，C=-\sum_0^\infin (-1)^n\dfrac{0^{n+1}}{n+1}=0\\
故f(x)=\sum_0^\infin (-1)^n\dfrac{x^{n+1}}{n+1}=x-\dfrac{x^2}{2}+\dfrac{x^3}{3}-\dfrac{x^4}{4}+...\\
$$
**check the end point** of $\pm1$, $x=1$ converge to $ln(2)$ while $x=-1$ diverge. Thus the converge interval is $(-1,1]$
$$
f(x)=arctanx\\
f'(x)=\dfrac{1}{1+x^2}=\sum_0^\infin (-1)^nx^{2n}\\
\int f'(x)dx=\sum_0^\infin \int\bigg((-1)^nx^{2n}\bigg)=\sum_0^\infin (-1)^n\dfrac{x^{2n+1}}{2n+1}+C\\
f(0)=0，C=0\\
f(x)=\sum_0^\infin (-1)^n\dfrac{x^{2n+1}}{2n+1}=x-\dfrac{x^3}{3}+\dfrac{x^5}{5}-\dfrac{x^7}{7}+...
$$
**check the end point** of $\pm1$, both converge, Thus the converge interval is $[-1,1]$
### Uniqueness of Power series
Let $\sum_0^\infin c_n(x-a)^n$ and $\sum_0^\infin d_n(x-a)^n$ be two convergent power series such that
$$
\sum_0^\infin c_n(x-a)^n=\sum_0^\infin d_n(x-a)^n
$$
for all x in an open interval containing a. Then $c_n = d_n$ for all $n ≥ 0$.
## Taylor
### 有限增量公式
若$f(x)$在a的某个领域可导，那么
$$
f(x)=f(a)+f'(a)\Delta x+o(\Delta x)
$$
### 引理1
设$f(x)$在$0\leq\vert x-a\vert\leq R$有定义，并且在a点有n阶导数
如果
$$
f(a)=f'(a)=...=f^{(n)}(a)=0
$$
则
$$
f(x)=o((x-a)^{n})=o(\Delta^n x)
$$

Proof
**因为$f(x)$在a点有n阶导数，所以它在a点邻近应该有直到$n-1$阶的导数**．我们可以用洛必达法则求以下极限：
$$
\begin{aligned}
&\lim_{x\rightarrow a}\dfrac{f(x)}{(x-a)^n}(查看f(x)是否是(x-a)^n的高阶无穷小)\\
&=\lim_{x\rightarrow a}\dfrac{f'(x)}{n(x-a)^{n-1}}\\
&=\lim_{x\rightarrow a}\dfrac{f''(x)}{n(n-1)(x-a)^{n-2}}\\
&\qquad\vdots\\
&=\lim_{x\rightarrow a}\dfrac{f^{n-1}(x)}{n!(x-a)}\\
&=\lim_{x\rightarrow a}\dfrac{f^{n-1}(x)-f^{n-1}(a)}{n!(x-a)}\\
&=\dfrac{1}{n!}f^{n}(a)=0
\end{aligned}
$$
因此，$f(x)$是$(x-a)^n$的高阶无穷小
### 引理2
设$f(x)$和$g(x)$在$0\leq\vert x-a\vert\leq R$有定义，并且在a点有n阶导数
如果
$$
f^{k}(a)=g^{k}(a)，k=0,1,...,n
$$
则
$$
f(x)=g(x)+o(\Delta^nx)
$$

Proof
令$h(x)=f(x)-g(x)$，有$h(a)=h'(a)=...=h^{n}(a)=0$，故$h(x)=o((x-a)^{n})$，所以$f(x)=g(x)+o((x-a)^n)$

通过增量的方式来使用级数逼近一个函数的值，而这个级数就要和$\Delta x$有关
Consider a function h that has a power series representation at $x = a$. Then the series has the form
$$
\begin{aligned}
h(x)&=\sum_0^K c_n(x-a)^n = c_0+c_1(x-a)+...+c_K(x-a)^K\\
&=f(a)+\Delta y\\
&=f(a)+\sum_1^K c_n\Delta^n x
\end{aligned}
$$
根据引理，如果要$f(x)=h(x)+o((x-a)^K)$，即$h(x)$和$f(x)$只相差一个高阶无穷小，那么
$$
\bigg(\sum_0^K  c_n(x-a)^n\bigg)^{(k)}\vert_{x=a}=f^k(a)，k=0,1,2,...,K
$$
故有
$$
\bigg(\sum_0^K  c_n(x-a)^n\bigg)^{(0)}\vert_{x=a}=f(a)\\
\bigg(\sum_0^K  c_n(x-a)^n\bigg)'\vert_{x=a}=f'(a)\\
\vdots\\
\bigg(\sum_0^K  c_n(x-a)^n\bigg)^{(K)}\vert_{x=a}=f^{(K)}(a)\\
$$
得到
$$
c_0=f(a)\\
c_1=f'(a)\\
c_2=\dfrac{f''(a)}{2!}\\
\vdots\\
c_K=\dfrac{f^{(K)}(a)}{K!}\\
$$
### Definition
If f has derivatives of all orders at $x = a$, then the Taylor series for the function f at a is
$$
f(x)=\sum_0^\infin \dfrac{f^{(n)}(a)}{n!}(x-a)^n=f(a)+\sum_1^\infin \dfrac{f^{(n)}(a)}{n!}\Delta^n x
$$
The Taylor series for f at 0 is known as the Maclaurin series for f.
### Uniqueness of Taylor Series
If a function f has a power series at a that converges to f on some open interval containing a, then that power series is the Taylor series for f at a.
### Taylor's theorem with Remainder
$$
R_K(x)=f(x)-\sum_0^K \dfrac{f^{(k)}(a)}{k!}(x-a)^k=\dfrac{f^{(K+1)}(c)}{(K+1)!}(x-a)^{K+1}，c在x和a之间
$$
###  Convergence of Taylor Serie
Suppose that f has derivatives of all orders on an interval $I$ containing a. Then the Taylor series
$$
\sum_0^\infin \dfrac{f^{(n)}(a)}{n!}(x-a)^n
$$
converges to $f(x)$ for all x in $I$ if and only if
$$
\lim_{n\rightarrow \infin}R_n(x)=0
$$
for all x in $I$.
### 麦克劳林展开式
$$
f(x)=e^x=1+x+\dfrac{x^2}{2!}+...=\sum_0^\infin \dfrac{x^k}{k!}，x\in R\\
f(x)=sinx=0+x-\dfrac{x^3}{3!}+\dfrac{x^5}{5!}-...=\sum_0^\infin (-1)^k\dfrac{x^{2k+1}}{(2k+1)!}，x\in R\\
f(x)=cosx=(sinx)'=1-\dfrac{1}{2!}x^2+\dfrac{1}{4!}x^4-...=\sum_0^\infin (-1)^k\dfrac{x^{2k}}{(2k)!}，x\in R
$$
### example
evaluate the series
$$
\sum_0^\infin \dfrac{1}{n!}\\
\sum_0^\infin \dfrac{2^n}{n!}\\
\sum_0^\infin (-1)^n\dfrac{(2\pi)^{2n}}{(2n)!}\\
\sum_0^\infin (-1)^n\dfrac{(2\pi)^{2n+1}}{(2n+1)!}\\
$$
### 麦克劳林展开式2
$$
f(x)=\dfrac{1}{1-x}=\sum_0^\infin x^n,x\in(-1,1)\\
\begin{aligned}
f(x)=ln(1+x)&=\sum_1^\infin (-1)^{n+1}\dfrac{x^n}{n},x\in(-1,1]\\
&=x-\dfrac{1}{2}x^2+\dfrac{1}{3}x^3-\dfrac{1}{4}x^4+...
\end{aligned}\\
\begin{aligned}
f(x)=arctanx&=\sum_0^\infin (-1)^n\dfrac{x^{2n+1}}{2n+1},x\in(-1,1]\\
&=x-\dfrac{1}{3}x^3+\dfrac{1}{5}x^5-\dfrac{1}{7}x^7+...
\end{aligned}\\
\begin{aligned}
f(x)=(1+x)^r&=\sum_0^\infin \big(^r_n\big)x^n,x\in(-1,1)\\
&=1+rx+\dfrac{r(r-1)}{2!}x^2+...+\dfrac{r(r-1)...(r-n+1)}{n!}x^n+...
\end{aligned}\\
$$
### example
$$
f(x)=\sqrt{1+x}\\
\sqrt{1+x}=1+\dfrac{1}{2}x+\dfrac{\dfrac{1}{2}\dfrac{-1}{2}}{2!}x^2+\dfrac{\dfrac{1}{2}\dfrac{-1}{2}\dfrac{-3}{2}}{3!}x^3+...\\
=1+\sum_1^\infin \dfrac{(-1)^{n+1}}{n!}\dfrac{1*3*5...*(2n-3)}{2^n}x^n
$$
### 麦克劳林展开式3
$$
tanx=x+\dfrac{1}{3}x^3\\
arcsinx=x+\dfrac{1}{6}x^3
$$
### 使用级数求解微分方程
page 595 