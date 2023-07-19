## Vector calculus
A vector field $\bold{F}$ in $ℝ^2$ is an assignment of a two-dimensional vector $\bold{F}(x, y)$ to each point $(x, y)$ of a subset $D$ of $ℝ^2$ . The subset $D$ is the domain of the vector field.
A vector field $\bold{F}$ in $ℝ^3$ is an assignment of a three-dimensional vector $\bold{F}(x, y, z)$ to each point $(x, y, z)$ of a subset $D$ of $ℝ^3$ . The subset $D$ is the domain of the vector field.

一个向量场很明显是向量值函数，且自变量是点
一个向量场可以表示成为
$$
\bold{F}(x,y)=P(x,y)\bold{i}+Q(x,y)\bold{j}
$$
对比
$$
\bold{r}(t)=P(t)\bold{i}+Q(t)\bold{j}
$$
一个将一维点映射成为一个二维向量
一个将二维点映射成为一个二维向量
### 固定场
$$
\bold{F}(x,y)=a\bold{i}+b\bold{j},a,b\in \R
$$
### 辐射场
1. 向外辐射
$$
\bold{F}(x,y)=ax\bold{i}+by\bold{j},a,b>0
$$
2. 向内辐射
$$
\bold{F}(x,y)=(-a)x\bold{i}+(-b)y\bold{j},a,b>0
$$
对比
$$
\bold{F}(x,y)=-x\bold{i}+(-2y)\bold{j}粒子靠近x轴更快速\\
\bold{F}(x,y)=-2x\bold{i}+(-y)\bold{j}粒子靠近y轴更快速
$$
### 旋场
1. 顺时针
$$
\bold{F}(x,y)=y\bold{i}-x\bold{j}
$$
2. 逆时针
$$
\bold{F}(x,y)=-y\bold{i}+x\bold{j}
$$
### 辐射场与旋场垂直正交
$$
(x\bold{i}+y\bold{j})\cdot (y\bold{i}-x\bold{j})=\bold{0}
$$
### 单位场
$$
\bold{F}(x,y)=\dfrac{P(x,y)}{\Vert\bold{F}\Vert}\bold{i}+\dfrac{Q(x,y)}{\Vert\bold{F}\Vert}\bold{j}
$$
### 梯度场
Recall that if $f$ is a (scalar) function of x and y, then the gradient of $f$ is
$$
grad f=∇ f=f_x(x,y)\bold{i}+f_y(x,y)\bold{j}
$$
Similarly, if $f$ is a function of $x$, $y$, and $z$, then the gradient of $f$ is
$$
grad f=∇ f=f_x(x,y)\bold{i}+f_y(x,y)\bold{j}+f_z(x,y)\bold{k}
$$
A vector field $\bold{F}$ in $ℝ^2$ or in $ℝ^3$ is a gradient field **if there exists a scalar function $ f$** such that $∇ f = \bold{F}$.
### example
find the gradient field of $f(x,y)=x^2y^2$
$$
∇ f=2y^2x\bold{i}+2x^2y\bold{j}
$$
### 保守场
a vector field $\bold{F}$ is a **conservative vector field**, or a gradient field **if there exists a scalar function $f$** such that $∇ f = \bold{F}$.  $f$ is called a **potential function**(势函数) for $\bold{F}$.
The reason such fields are called conservative is that they model forces of physical systems in which energy is conserved.
### example
find the potential function where
$$
\bold{F}(x,y,z)=  (2xyz-ycos(xy))\bold{i}+(x^2z-xcos(xy))\bold{j}+x^2y\bold{k}
$$
$$
f_x=2xyz-ycos(xy)\\
f_y=x^2z-xcos(xy)\\
f_z=x^2y
$$
$$
\int2xyz-ycos(xy)dx=x^2yz-sin(xy)\\
\dfrac{\partial}{\partial y}x^2yz-sin(xy)=x^2z-xcos(xy)\\
\dfrac{\partial}{\partial z}x^2yz-sin(xy)=x^2y\\
$$
thus
$$
f=x^2yz-sin(xy)
$$
### Uniqueness of Potential Functions
Let $F$ be a conservative vector field on an **open and connected** domain and let $f$ and $g$ be functions such that $∇ f = \bold{F}$ and $∇g = \bold{F}$. Then, there is a constant $C$ such that $f = g + C$.

**proof**
Since $f$ and $g$ are both potential functions for $\bold{F}$, then $∇ (f − g) = ∇ f − ∇g = \bold{F} − \bold{F} = \bold{0}$. Let $h = f − g$, then we have $∇h = \bold{0}$. We would like to show that $h$ is a constant function.
Assume $h$ is a function of $x$ and $y$ (the logic of this proof extends to any number of independent variables). Since $∇h = \bold{0}$, we have $h_x = 0$ and $h_y = 0$. The expression $h_x = 0$ implies that $h$ is a constant function with respect to x—that is, $h(x, y) = k_1 (y)$ for some function $k_1$. Similarly, $h_y = 0$ implies $h(x, y) = k_2 (x)$ for some function $k_2$. Therefore, function $h $ depends only on $y$ and also depends only on $x$. Thus, $h(x, y) = C$ for some constant $C$ on the connected domain of F. Note that we really do need connectedness at this point; **if the domain of $\bold{F}$ came in two separate pieces, then $k$ could be a constant $C_1$ on one piece but could be a different constant $C_2$ on the other piece**. Since $f − g = h = C$, we have that $f − g + C$, as desired.
### The Cross-Partial Property of Conservative Vector Fields
Let $\bold{F}$ be a vector field in two or three dimensions such that the component functions of $\bold{F}$ have continuous second- order mixed-partial derivatives on the domain of $\bold{F}$.
if
$$
F(x, y) = 〈 P(x, y), Q(x, y) 〉 
$$
is a conservative vector field in $ℝ^2$
then
$$
\dfrac{\overbrace{\partial P}^{场向量的横坐标}}{\underbrace{\partial y}_{交叉偏导}}=\dfrac{\overbrace{\partial Q}^{场向量的纵坐标}}{\partial x}
$$
if
$$
F(x, y, z) = 〈 P(x, y, z), Q(x, y, z), R(x, y, z) 〉
$$
is a conservative vector field in ℝ^3 , then
$$
\dfrac{\partial P}{\partial y}=\dfrac{\partial Q}{\partial x},\dfrac{\partial P}{\partial z}=\dfrac{\partial R}{\partial x},\dfrac{\partial Q}{\partial z}=\dfrac{\partial R}{\partial y}
$$
**proof**
By Clairaut’s theorem, $fxy = fyx$
**Caution**
The theorem does not say that, if $\bold{F}$ has the cross-partial property, then $\bold{F}$ is conservative.
The conclusion **can only help determine that a field is not conservative**; it does not let you conclude that a vector field is conservative.
## 线积分
###  线标量积
Let $f$ be a function with a domain that includes the smooth curve $C$ that is parameterized by $\vec{r}(t) = 〈 x(t), y(t), z(t) 〉$ , $a ≤ t ≤ b$. The scalar line integral of f along $C$ is
$$
\int_Cf(x,y,z)ds=\lim_{n\rightarrow \infin}\sum^n_{i=1}f(P^*_{[t_{i-1},t_i]})\Delta s_i
$$
In this definition, the arc lengths $Δs1, Δs2 ,…, Δsn$ aren’t necessarily the same
事实上在以前的定义中为了方便将$\Delta$量都定为等分相同，这里的$\Delta s$随着$\Delta t$等分变化很少能等分相同，但是只要最大的趋于0即可$(\Delta t\rightarrow 0,\Delta s\rightarrow 0)$
只要$f$在$C$上可积，则此极限存在    
### geometric meaning
$$
\int_Cf(x,y)ds=\int_{R=C}(f(x,y)-\{z=0\})ds
$$
对于一个二元函数来说，其在$C$上的线积分就类似于在区域$A$上的二重积分一样，表示由曲线$C$到曲面$z=f(x,y)$形成的柱面的面积
###  Evaluating a Scalar Line Integral
Let $f$ be a continuous function with a domain that includes the smooth curve $C$ with parameterization $\bold{r}(t), a ≤ t ≤ b$. Then
$$
\int_Cfds=\int_a^bf(\bold{r}(t))\Vert \bold{r'}(t)\Vert dt
$$
for $f(x,y)$
$$
\int_a^bf(\bold{r}(t))\Vert \bold{r'}(t)\Vert dt=\
\int_a^bf(x(t),y(t))\sqrt{x'^2(t)+y'^2(t)}dt
$$
for $f(x,y,z)$
$$
\int_a^bf(\bold{r}(t))\Vert \bold{r'}(t)\Vert dt=\int_a^bf(x(t),y(t),z(t))\sqrt{x'^2(t)+y'^2(t)+z'^2(t)}dt
$$
**Scalar line integrals are independent of parameterization**, as long as the curve is traversed exactly once by the parameterization.
比较
$$
\bold{r_1}(t)=<cos(t),sin(t),t>,t\in (0,2\pi)\\
\bold{r_2}(t)=<cos(2t),sin(2t),2t>t\in (0,\pi)
$$
$\int_{C_{\bold{r_1}}} fds$和$\int_{C_{\bold{r_2}}}fds$是一样的
### 曲线长度
$Arc=\int_C1ds$
### 线矢量积的模型
假设粒子在三维空间每个位置上受到的力为
$$
\bold{F}(x,y,z)=P(x,y,z)\bold{i}+Q(x,y,z)\bold{j}+R(x,y,z)\bold{k}
$$
并且连续。$C$ 代表粒子在空间中移动的轨迹，轨迹光滑，需要计算力的做功
需要指出的是，力的做功大小和粒子的运动方向有关，因此轨迹$C$为**有向曲线**，一个指定的方向为正向，与其相反的方向为反向
### 线矢量积
Let $\bold{r}(t)$ be a parameterization of $C$ for $a ≤ t ≤ b$ such that the curve is **traversed exactly once**(如果是闭合曲线) by the particle and the particle moves in the **positive direction** along $C$. There is a partition $(a=t_0,t_1,...,t_n=b)$。
在某一点$P_i$的功微元$\Delta W=\bold{F}(P_i)\cdot [\bold{T_C}(P_i)\Delta t]$，其中$\bold{T_C}(P_i)\Delta t$是粒子在该点沿着切线方向的微小移动量，因此
$$
W\approx \sum_1^n\bold{F}(P^*_{[t_{i-1},t_i]})\cdot [\bold{T_C}(P^*_{[t_{i-1},t_i]})\Delta t]
$$
或者，令$\bold{T_C^u}(P_i)$为曲线上点$P_i$的单位切线向量，$ \Delta s_i=V_i\Delta t=\Vert T_C(P^*)\Vert\Delta t$，则$\Delta t=\dfrac{\Delta s}{\Vert T_C(P^*)\Vert}$
$$
W\approx \sum_1^n\bold{F}(P^*_{[t_{i-1},t_i]})\cdot [\bold{T_C^u}(P^*_{[t_{i-1},t_i]})\Delta s_i]
$$
此形式表示，功$W$同样与参数$t$(时间)无关$(\Delta s_i)$，但是与曲线的方向有关
也就是说在一个给定的场$\bold{F}$，在里面绕的快或者慢最后场做的功是一样的，只要路径和方向一样
The vector line integral of vector field F along oriented smooth curve $C $ is
$$
\int_C\bold{F}\cdot \bold{T^u}ds=\int_C\bold{F}(\bold{r}(t))\cdot \bold{T}dt=\int_C\bold{F}\cdot \overbrace{d\bold{r}}^{\Delta \bold{r},\bold{r}(t_i)-\bold{r}(t_{i-1}),\bold{r'}(t)dt}
$$
if $C$ is an oriented curve, then we let $−C$ represent the same curve but with **opposite orientation**.
### examples
Find the value of integral $∫_C\bold{F} · d\bold{r}$, where $C$ is the semicircle parameterized by $\bold{r}(t) = 〈 cos t, sin t 〉$, $0 ≤ t ≤ π$ and $\bold{F} = 〈 −y, x 〉$.
$$
\int_C\bold{F}\cdot d\bold{r}=\int_0^{\pi}-sint(cost)'+cost(sint)'dt=\pi
$$
### example2
Find the value of integral $\int_C\bold{F}\cdot d\bold{r}$ where $C$ is the semicircle parameterized by $\bold{r}(t) = 〈 cos (t + π), sin t $〉 , $0 ≤ t ≤ π$ and $\bold{F} = 〈 −y, x 〉$ .
$$
\bold{F_C}=(-sint,cos(t+\pi))\\
\bold{r'}(t)=\bold{T}(t)=(-sin(t+\pi),cost)\\
\int_C\bold{F}\cdot d\bold{r}=\int_0^\pi -sint(-sin(t+\pi))+(cos(t+\pi))(cost)dt=-\pi
$$
**诱导公式**
$$
sin(t+\pi)=-sint\\
cos(t+\pi)=-cost
$$
### Standard notation
Another standard notation for integral $∫_C\bold{F} · d\bold{r}$ is $∫_CPdx + Qdy + Rdz$. 
$$
\begin{aligned}
∫_C\bold{F} · d\bold{r}&=\int_C(P,Q,R)\cdot(x'(t),y'(t),z'(t))dt\\
&=\int_CP\dfrac{dx}{dt}dt+Q\dfrac{dy}{dt}dt+R\dfrac{dz}{dt}dt\\
&=\int_CPdx+Qdy+Rdz
\end{aligned}
$$
### example
Find the value of integral $\int_Czdx+xdy+ydz$,  where C is the curve parameterized by $\bold{r}(t) = 〈 t^2, t, t 〉$ , $1 ≤ t ≤ 4$.
$$
\bold{F_C}=(t,t^2,t)\\
\begin{aligned}
\int_Czdx+xdy+ydz&=\int_Ctx'(t)dt+t^2y'(t)dt+tz'(t)dt\\
&=\int_1^4t*2tdt+t^2dt+tdt\\
\end{aligned}
$$
### piecewise smooth curve
**分段接续光滑**
curve $C$ is piecewise smooth if $C$ can be written as a union of n smooth curves $C_1, C_2 ,…, C_n$ such that the endpoint of $C_i$ is the starting point of $C_{i + 1} $
### Properties of Vector Line Integrals
Let $F$ and $G$ be continuous vector fields with domains that include the oriented smooth curve $C$. Then
1. 向量的分配律
$$
\int_C(\bold{F}+\bold{G})\cdot d\bold{r}=\int_C\bold{F}\cdot d\bold{r}+\int_C\bold{G}\cdot d\bold{r}\\
$$
2. 向量的数乘
$$
\int_Ck\bold{F}\cdot d\bold{r}=k\int_C\bold{F}\cdot d\bold{r}
$$
3. 曲线有向性
$$
\int_{-C}\bold{F}\cdot d\bold{r}=-\int_C\bold{F}\cdot d\bold{r}
$$
4. 分段接续性
$$
\int_{C}\bold{F}\cdot d\bold{r}=\int_{C_1}\bold{F}\cdot d\bold{r}+\int_{C_2}\bold{F}\cdot d\bold{r}+...
$$
### Flux通量(曲线)
$C$为**速度**场$\bold{F}$内的一个曲线，现要计算穿过该曲线的通过量(单位时间内，流过曲线的量)
Calculating Flux across a Curve
Let F be a vector field and let $C$ be a smooth curve with parameterization $\bold{r}(t) = 〈 x(t), y(t) 〉$ , $a ≤ t ≤ b$. Let $\bold{n_C}(t) = 〈 y'(t), −x'(t) 〉$ . The flux of $\bold{F}$ across $C$ is
$$
\int_C\bold{F}\cdot \bold{N_C^u}ds=\int_C\bold{F}(\bold{r}(t))\cdot \bold{n_C}dt    
$$
### 通量的方向
沿着曲线的正方向，正方向右侧的通量为正
### example
Calculate the flux of $\bold{F} = 〈 2x, 2y 〉$ across a unit circle oriented counterclockwise and clockwise
$$
\bold{r}=<cost,sint>\\
\bold{F}=<2cost,2sint>
$$
for counterclockwise
$$
\bold{r}=<sint,cost>\\
\bold{F}=<2sint,2cost>
$$
for clockwise
Flux for counterclockwise
$$
Flux=\int_0^{2\pi}2costcost+2sintsintdt=4\pi
$$
Flux for clockwise
$$
Flux=\int_0^{2\pi}-2sintsint-2costcostdt=-4\pi
$$
### Flux of standard notation
$$
\int_CPdy-Qdx=\int_C(P,Q)\cdot (dy,-dx)
$$
### circulation(环量)
The line integral of vector field F along an oriented **closed** curve is called the circulation of $\bold{F}$ along $C$.
$$
\oint_C\bold{F}\cdot \bold{T_C}dt
$$
The value of the circulation  measures the tendency of the fluid to move **in the direction of $C$**.
沿着该曲线做的功越多，环量就越大，该曲线的效率就越高
### example
Calculate the circulation of
$$
\bold{F}=<-\dfrac{y}{x^2+y^2},\dfrac{x}{x^2+y^2}>
$$
along a unit circle oriented counterclockwise.
$$
\bold{r}(t)=<cost,sint>\\
\bold{F}=<-sint,cost>\\
\oint_C\bold{F}\cdot \bold{T}dt=\int_0^{2\pi}sin^2t+cos^2tdt=2\pi
$$
## 保守场
### 简单闭环曲线
Curve $C$ is a closed curve if there is a parameterization $\bold{r}(t)$, $a ≤ t ≤ b$ of $C$ such that the parameterization traverses the curve exactly once and $\bold{r}(a) = \bold{r}(b)$. Curve $C$ is a simple curve if C does not cross itself. That is, $C$ is **simple** if there exists a parameterization $ \bold{r}(t)$, $a ≤ t ≤ b$ of $C$ such that $\bold{r}$ is one-to-one over $(a, b)$. It is possible for $\bold{r}(a) = \bold{r}(b)$, meaning that the simple curve is also **closed**.
### example
Is the curve with parameterization $\bold{r}(t)=<cost,\dfrac{sin(2t)}{2}>,0\leq t\leq 2\pi$ a simple closed curve?
Note that $\bold{r}(0) = 〈 1, 0 〉 = \bold{r}(2π)$; 首尾相连
Note that $\bold{r}(\dfrac{\pi}{2})=<0,0>=\bold{r}(\dfrac{3\pi}{2})$; 交叉
### 简单区域
A region $D$ is a connected region if, for any two points $P_1$ and $P_2$, there is a path from $P_1$ to $P_2$ with a trace contained entirely inside $D$. A region $D$ is a **simply connected** region if $D$ is connected for any simple closed curve $C$ that lies inside $D$, and curve $C$ can be shrunk continuously to a point while staying entirely inside $D$. In two dimensions, a region is simply connected if it is connected and has no holes.
简单连通区域没有洞
### Fundamental Theorem for Line Integrals
类比
$$
\int_a^bf(x)dx=F(b)-F(a)
$$
如果有$f=f(x,y)$
$$
∇f=(f_x,f_y)=\bold{F}
$$
那么场$\bold{F}$就是一个保守场
$$
\int_C\bold{F}\cdot \overbrace{\bold{T}dt}^{就是向量(dx,dy)}=f(P_{t_{end}})-f(P_{t_{start}})
$$
在保守场内场所做的功**与路径无关**，只与起始点和终点的位置有关
**proof**
曲线$C$由向量值函数$\bold{r}(t)=<x(t),y(t)>$给出
$$
\dfrac{df(x,y)}{dt}=f_xx'(t)+f_yy'(t)=∇f\cdot \bold{T}\\
$$
更具牛顿莱布尼茨定理有
$$
\int_a^b∇f\cdot \bold{T}dt=f(t=b)-f(t=a)=f(P_{t=b})-f(P_{t=a})
$$
a vector field, even if it is continuous, does not need to have a potential function.
即使场$\bold{F}$连续，也可能没有势函数
### example
Applying the Fundamental Theorem
$$
\bold{F}=<2xlny,\dfrac{x^2}{y}+z^2,2yz>\\
\bold{r}(t)=<t^2,t,t>,1\leq t\leq e
$$
$$
f_x=2xlny,f_z=2yz,f=\int f_xdx+\int f_zdz=x^2lny+yz^2
$$
thus $\bold{F}$ is conservative
$$
\int_C\bold{F}\cdot \bold{T}dt=\int_C∇f\cdot \bold{T}dt=f(t=e)-f(t=1)=e^4+e^3-1
$$
### 势函数
also we have
$$
F(x)=\int_a^xf(x)dx
$$
$f(x)$在$[a,b]$上连续
因此也有
$$
f(x,y)=\int_a^t\bold{F}\cdot d\bold{r}=\int_a^t\bold{F}\cdot \bold{T}dt=\int_C∇f\cdot \bold{T}dt=f(\bold{r}(t))
$$
### The Path Independence Test for Conservative Fields
If $F$ is a continuous vector field that is **independent of path** and the domain $D$ of $F$ is **open and connected**, then $F$ is conservative.
### example
Use path independence to show that vector field $F(x, y) = 〈 x^2 y, y + 5 〉$ is not conservative.
如果一个闭曲线$C$的线积分不为0，那么就不是保守的
$$
\bold{r}(t)=<cost,sint>\\
\oint_C\bold{F}\cdot d\bold{r}=\int_0^{2\pi}-cos^2tsin^2t+(sint+5)costdt=-\dfrac{\pi}{4}\neq 0
$$
### Find the potential function
**Given**s a conservative vector field $\bold{F}$, how do we find a function $f$, such that $∇f=\bold{F}$?
**example**
find the potential function
$$
\bold{F}=<2xy^3,3x^2y^2+cos(y)>
$$
$$
f_x=2xy^3\\
f(x,y)=\int f_xdx=x^2y^3+\overbrace{h(y)}^{偏导的C}
$$
类似有
$$
\int f_xdx=x^2y^3+h(y,z)
$$
if $f=f(x,y,z)$
现在有
$$
f_y=3y^2x^2+\dfrac{dh}{dy}=3x^2y^2+cos(y)
$$
thus
$$
\dfrac{dh}{dy}=cos(y)\\
h=sin(y)+C
$$
因此势函数为
$$
f(x,y)=x^2y^3+sin(y)+C
$$
**example2**
Find a potential function for $\bold{F}(x,y,z)=<2xy,x^2+2yz^3,3y^2z^2+2z>$
$$
f_x=2xy,
f(x,y,z)=x^2y+h(y,z)\\
f_y=x^2+h_y=x^2+2yz^3,
h_y=2yz^3\\
h(y,z)=y^2z^3+g(z)\\
f_z=h_z=3z^2y^2+2z,g'(z)=2z\\
g(z)=z^2+C\\
f(x,y,z)=x^2y+y^2z^3+z^2
$$
###  The Cross-Partial Test for Conservative Fields
If $\bold{F} = 〈 P, Q, R 〉$ is a vector field on an **open, simply connected** region $D$ and $P_y = Q_x$, $P_z = R_x$,and $Q_z = R_y$ throughout $D$, then $F$ is conservative.
Let $\bold{F} = 〈 P, Q, R 〉$ be a vector field on **an open, simply connected** region $D$. Then $P_y = Q_x$, $P_z = R_x$, and $Q_z = R_y$ throughout $D $ **if and only if** $F$ is conservative.
### example
场$\bold{F}=<\dfrac{y}{x^2+y^2},\dfrac{-x}{x^2+y^2}>$不是保守场，但是
$$
P_y=\dfrac{x^2-y^2}{(x^2-y^2)^2}=Q_x
$$
因为场在$(0,0)$点无定义，因此其定义域不是简单开区域
## 格林公式
Let $D$ be an open, simply connected region with a boundary curve $C$ that is a **piecewise**(分段) smooth, simple closed curve oriented counterclockwise. Let $\bold{F} = 〈 P, Q 〉$ be a vector field with component functions that have continuous partial derivatives on $D$. Then,
$$
\oint_C\bold{F}\cdot d\bold{r}=\oint_CPdx+Qdy=\iint_D\underbrace{(Q_x-P_y)}_{表示所积曲线的方向性}dA
$$
Notice that Green’s theorem can be used only for a **two-dimensional** vector field $\bold{F}$. 
**rectangle condition**
正方形位于$[a,b]\times [c,d]$，bounded by curve $C$，方向为逆时针
$$
C_1:\bold{r_1}(t)=<t,c>,t\in [a,b]\\
C_2:\bold{r_2}(t)=<b,t>,t\in [c,d]\\
C_3:\bold{r_3}(t)=<t,d>,t\in [b,a]\\
C_4:\bold{r_4}(t)=<a,t>,t\in [d,c]\\
$$
因此
$$
\oint_C\bold{F}\cdot d\bold{r}=\int_{C_1}\bold{F}\cdot d\bold{r_1}+\int_{C_2}\bold{F}\cdot d\bold{r_2}+\int_{C_3}\bold{F}\cdot d\bold{r_3}+\int_{C_4}\bold{F}\cdot d\bold{r_4}\\
=\int_a^b\bold{F}\cdot (1,0)dt+\int_c^d\bold{F}\cdot (0,1)dt-\int_a^b\bold{F}\cdot(1,0)dt-\int_c^d\bold{F}\cdot(0,1)dt\\
=\int_a^bP(\bold{r_1})-P(\bold{r_3})dt+\int_c^dQ(\bold{r_2})-Q(\bold{r_4})dt\\
=\int_a^bP(t,c)-P(t,d)dt+\int_c^dQ(b,t)-Q(a,t)dt\\
=-\int_a^b\overbrace{P(t,d)-P(t,c)}^{看成原函数相减}dt+\int_c^dQ(b,t)-Q(a,t)dt\\
=-\int_a^b\underbrace{\int_c^d\dfrac{\partial}{\partial y}P(x=t,y)dy}_{a到b上的边缘积分}dt+\int_c^d\int_a^b\dfrac{\partial}{\partial x}Q(x,y=t)dxdt\\
第一部分x=x(t)=t，y与t无关(\bold{r_1}与\bold{r_3})\\
第二部分x与t无关(\bold{r_2}与\bold{r_4})，y=y(t)=t\\
=-\int_a^b\int_c^d\dfrac{\partial}{\partial y}P(x,y)dydx+\underbrace{\int_c^d\int_a^b}_{上下限都为常数}\dfrac{\partial}{\partial x}Q(x,y)dxdy\\
交换积分次序\\
=-\int_a^b\int_c^d\dfrac{\partial}{\partial y}P(x,y)dydx+\int_a^b\int_c^d\dfrac{\partial}{\partial x}Q(x,y)dydx\\
=\int_a^b\int_c^d(Q_x-P_y)dydx
$$
### example
Calculate the line integral
$$
\oint_Cx^2ydx+(y-x)dy
$$
where $C$ is a rectangle with vertices $(1, 1)$, $(4, 1)$, $(4, 5)$, and $(1, 5)$ oriented counterclockwise.
$$
\bold{r_1}=<t,1>,t\in [1,4]\\
\bold{r_2}=<4,t>,t\in [1,5]\\
\bold{r_3}=<t,5>,t\in [4,1]\\
\bold{r_4}=<1,t>,t\in [5,1]\\
$$
$$
\oint_Cx^2ydx+(y-x)dy=\iint_D(-1-x^2)dA=\int_1^4\int_1^5(-1-x^2)dydx
$$
### example2
Calculate the work done on a particle by force field
$$
F(x, y) = 〈 y + sin x, e^y − x 〉
$$
as the particle traverses circle $x^2 + y^2 = 4$ exactly once in the counterclockwise direction, starting and ending at point $(2, 0)$.
$$
\bold{r}(t)=<2cost,2sint>\\
\bold{F}=<2sint+sin(2cost),e^{2sint}-2cost>
$$
$$
\oint_C\bold{F}\cdot d\bold{r}=\iint_D\bigg(\dfrac{\partial}{\partial x}e^y-x\bigg)-\bigg(\dfrac{\partial}{\partial y}y + sin x\bigg)dA\\
=\int_0^{2\pi}\int_0^2(-1-1)rdrd\theta\\
=-2\pi4=-8\pi
$$
### example3(格林公式的逆用)
Calculate the area enclosed by ellipse
$$
\dfrac{x^2}{a^2}+\dfrac{y^2}{b^2}=1
$$
$$
\bold{r}=<acost,bsint>逆时针\\
\bold{F}=<P,Q>
$$
$$
\iint_DdA=\iint_D(Q_x-P_y)dA\\
Q_x-P_y=1
$$
可以令$\bold{F}=<0,x>$
$$
\iint_DdA=\oint_C\bold{F}\cdot d\bold{r}=\int_0^{2\pi}(0,acost)\cdot (-asint,bcost)dt\\
=\int_0^{2\pi}abcos^2tdt=ab\bigg(\dfrac{1}{2}t+\dfrac{1}{4}cos2t\bigg)_0^{2\pi}=ab\pi 
$$
### 格林面积公式
在二维图像上的面积可以由格林公式反向计算
令
$$
\bold{F}=<-\dfrac{y}{2},\dfrac{x}{2}>(<0,x>未必更简单)
$$
图像边界$C$**逆时针**
则有
$$
\iint_DdA=\oint_C(-\dfrac{y}{2},\dfrac{x}{2})\cdot (dx,dy)dt=\dfrac{1}{2}\oint_C-ydx+xdy
$$
### example
Find the area of the region enclosed by the curve with parameterization $\bold{r}(t) = 〈 sin t cos t, sin t 〉$ , $0 ≤ t ≤ π$.
$$
\iint_DdA=\dfrac{1}{2}\oint_C-ydx+xdy\\
=\dfrac{1}{2}\int_0^\pi-sint(cos^2t-sin^2t)+sintcos^2tdt\\
=\dfrac{1}{2}\int_0^\pi sin^3tdt=\dfrac{1}{2}\int_0^\pi(cos^2t-1)dcost\\
=\dfrac{1}{2}\dfrac{cos^3t}{3}\vert_0^\pi-\dfrac{1}{2}cost\vert_0^\pi\\
=\dfrac{2}{3}
$$
### Flux Form of Green’s Theorem
Let $D$ be an open, simply connected region with a boundary curve $C$ that is a piecewise smooth, simple closed curve that is oriented **counterclockwise**. Let $\bold{F} = 〈 P, Q 〉$ be a vector field with component functions that have continuous partial derivatives on an open region containing $D$. Then,
$$
\oint_C\bold{F}\cdot \bold{N}dt=\oint_C\bold{F}\cdot \bold{N^u}ds=\iint_D(P_x+Q_y)dA
$$
将复杂的线积分转换为简单的二重积分
$$
\iint_D\underbrace{(P_x+Q_y)}_{通过引入偏导极大化简被积函数}dA
$$
**proof**
$$
\oint_C\bold{F}\cdot \bold{N}dt=\oint_CPdy-Qdx=\oint_C-Qdx+Pdy\\
=\oint_C(-Q)dx+Pdy=\iint_D(P_x-[-Q]_y)dA\\
=\iint_D(P_x+Q_y)dA
$$
### example
Let $C$ be a circle of radius r centered at the origin and let $\bold{F}(x, y) = 〈 x, y 〉$ . Calculate the flux across $C$.
$$
\oint_Cxdy-ydx=\iint_D(1+1)dA=2\pi r^2
$$
### example2
Applying Green’s Theorem for Flux across a Triangle
Let $S$ be the triangle with vertices $(0, 0)$, $(1, 0)$, and $(0, 3)$ oriented **clockwise**. Calculate the flux of $\bold{F}(x, y) = 〈 P(x, y), Q(x, y) 〉 = 〈 x^2 + e^y, x + y 〉$ across $S$.
**If counterwise**
$$
\oint_C(x^2 + e^y)dy-(x + y)dx=\iint_D(2x+1)dA\\
=\int_0^1\int_0^{-3x+3}2x+1dydx=\dfrac{5}{2}
$$
所以逆时针为$-\dfrac{5}{2}$
### Source-free field(无源场)
场$\bold{F}=<P,Q>$是无源场，则
1. 任意闭合曲线通量$\oint_C\bold{F}\cdot \bold{N}dt$为0
2.  flux is independent of path.
3.  Has **steam function** $g(x,y)$ such that
$$
\bold{F}=<P,Q>\\
g_y=P,g_x=-Q
$$
考虑有
$$
∇g=(g_x,g_y)\\
∇g\cdot (g_y,-g_x)=0
$$
因此$(g_y,-g_x)$是函数$g(x,y)$的等值线切线
因此若场$\bold{F}=<P,Q>$存在函数$g(x,y)$使得$\bold{F}$为其**等值线切线**，则$\bold{F}$为无源场
4. $P_x+Q_y=0$
$$
P_x=g_{yx}=g_{xy}=-Q_y
$$
### Finding a Stream Function
Verify that rotation vector field $\bold{F}(x, y) = 〈 y, −x 〉$ is source free, and find a stream function for $\bold{F}$.
first verify the source free field
$\bold{F}\in \R^2$
$$
\oint_C\bold{F}\cdot \bold{N}dt=\oint_C ydy-(-x)dx\\
=\int_0^{2\pi}sintcost-costsintdt=0
$$
$$
g_x=-Q=x,g_y=P=y\\
g(x,y)=\dfrac{x^2}{2}+h(y)\\
g_y=h_y=y,h(y)=\dfrac{y^2}{2}+C\\
g(x,y)=\dfrac{x^2}{2}+\dfrac{y^2}{2}+C
$$
### laplace equation
如果场$\bold{F}=<P,Q>$在**简单开区域**既是**保守场**又是**无源场**，那么$\bold{F}$是和谐场
因为是保守场，所以
$$
f_x=P,f_y=Q
$$
则
$$
f_{xx}=P_x,f_{yy}=Q_y
$$
因为是无源场，则有
$$
P_x+Q_y=0
$$
因此
$$
f_{xx}+f_{yy}=0
$$
### Green’s Theorem on General Regions
page 734
现在有两条简单闭合曲线$C_1$和$C_2$，$C_1$包含$C_2$，现在要探讨这两条曲线在场$\bold{F}=<P,Q>$内的线积分的关系
即：
$$
\oint_{C_1}\bold{F}\cdot d\bold{r}-\oint_{C_2}\bold{F}\cdot d\bold{r}
$$
当
1. 两曲线所围的区域$D_{C_1}$和$D_{C_2}$均为简单连通开区域，
2. 并且$C_1$和$C_2$均为**逆时针**时(positive oriented)，

运用格林公式
$$
\oint_{C_1}\bold{F}\cdot d\bold{r}-\oint_{C_2}\bold{F}\cdot d\bold{r}\\
=\iint_{D_{C_1}}(Q_x-P_y)dA-\iint_{D_{C_2}}(Q_x-P_y)dA\\
=\iint_{D_{C_1}-D_{C_2}}(Q_x-P_y)dA
$$
当
1. 两曲线所围的区域$D_{C_1}$和$D_{C_2}$均为简单连通开区域，
2. 并且$C_1$**逆时针**，$C_2$为**顺时针**时
$$
\oint_{C_1}\bold{F}\cdot d\bold{r}-\oint_{C_2}\bold{F}\cdot d\bold{r}\\
=\iint_{D_{C_1}}(Q_x-P_y)dA-\iint_{D_{C_2}}(P_y-Q_x)dA\\
=\iint_{D_{C_1}}(Q_x-P_y)dA+\iint_{D_{C_2}}(Q_x-P_y)dA\\
=\iint_{D_{C_1}+D_{C_2}}(Q_x-P_y)dA
$$
**问题**
**若曲线$C_2$内有无定义点时，如何计算两线积分的关系？**
**案例**
$\bold{F}=<-\dfrac{x}{x^2+y^2},\dfrac{y}{x^2+y^2}>$在洞$(0，0)$点无定义
现有闭合曲线
$$
\bold{r_1}=<2cost,2sint>\\
\bold{r_2}=<cost,sint>
$$
包含$(0,0)$
如何计算$\oint_{C_1}\bold{F}\cdot \bold{r}-\oint_{C_2}\bold{F}\cdot \bold{r}$

**Method**
page 734图
将区域从中间一道划分两块形成两块简单连通区域$D_1$和$D_2$，这时可以运用格林公式，并且：
**$C_1$逆时针，$C_2$顺时针**
$$
\oint_{\partial D_1}\bold{F}\cdot d\bold{r}=\iint_{D_1}(Q_x-P_y)dA\\
\oint_{\partial D_2}\bold{F}\cdot d\bold{r}=\iint_{D_2}(Q_x-P_y)dA
$$
同时
$$
\oint_{\partial D_1}\bold{F}\cdot d\bold{r}+\oint_{\partial D_2}\bold{F}\cdot d\bold{r}\\=\oint_{C_1}\bold{F}\cdot d\bold{r}+\oint_{C_2}\bold{F}\cdot d\bold{r}\\=\underbrace{\oint_{C_1}\bold{F}\cdot d\bold{r}}_{逆时针}-\underbrace{\oint_{-C_2}\bold{F}\cdot d\bold{r}}_{逆时针}
$$
因此当有曲线$S_1$和$S_2$并且**都逆时针**时
$$
\oint_{S_1}\bold{F}\cdot d\bold{r}-\oint_{S_2}\bold{F}\cdot d\bold{r}\\=\oint_{\partial D_1}\bold{F}\cdot d\bold{r}+\oint_{\partial D_2}\bold{F}\cdot d\bold{r}\\
=\iint_{D_1}(Q_x-P_y)dA+\iint_{D_2}(Q_x-P_y)dA\\
=\iint_{D_1+D_2}(Q_x-P_y)dA\\
=\iint_{两曲线所夹区域}(Q_x-P_y)dA
$$
与此同时有
$$
\oint_{S_1}\bold{F}\cdot d\bold{r}-\oint_{S_2}\bold{F}\cdot d\bold{r}\\
=\underbrace{\oint_{S_1}\bold{F}\cdot d\bold{r}}_{逆时针}+\underbrace{\oint_{-S_2}\bold{F}\cdot d\bold{r}}_{顺时针}\\
=\iint_{两曲线所夹区域}(Q_x-P_y)dA
$$
总结因此
1. 当$S_1$逆时针，$S_2$逆时针，则两者线积分之差为特定值，且
$$
\oint_{S_1}\bold{F}\cdot d\bold{r}-\oint_{S_2}\bold{F}\cdot d\bold{r}=\iint_{两曲线所夹区域}(Q_x-P_y)dA
$$
2. 当$S_1$逆时针，$S_2$顺时针，则两者线积分之和为特定值，且
$$
\oint_{S_1}\bold{F}\cdot d\bold{r}+\oint_{S_2}\bold{F}\cdot d\bold{r}=\iint_{两曲线所夹区域}(Q_x-P_y)dA
$$
### example
Using Green’s Theorem on a Region with Holes
Calculate integral
$$
\oint_{\partial D}\left(sinx-\dfrac{y^3}{3} \right)dx+\bigg(\dfrac{y^3}{3}+siny\bigg)dy
$$
where $D$ is the annulus given by the polar inequalities $1 ≤ r ≤ 2$, $0 ≤ θ ≤ 2π$.
$$
\oint_{\partial D}\bold{F}\cdot d\bold{r}=\iint_D(0+y^2)dA\\
=\int_0^{2\pi}\int_1^2(rsin\theta)^2rdrd\theta\\
=\dfrac{15\pi}{4}
$$
### example2
Let $\bold{F}=<\dfrac{y}{x^2+y^2},\dfrac{-x}{x^2+y^2}>$
and let C be any simple closed curve in a plane oriented counterclockwise.  What are the possible values of $\oint_C\bold{F}\cdot d\bold{r}$
1. 对于$C$不过原点，有
$$
\oint_C\bold{F}\cdot d\bold{r}=\iint_D\overbrace{(Q_x-P_y)}^{0}dA=0
$$
2. 对于$C$过原点，另一任意曲线$S$逆时针包含$C$，
$$
\oint_S\bold{F}\cdot d\bold{r}-\oint_C\bold{F}\cdot d\bold{r}=\iint_{D_{between}}(Q_x-P_y)dA=0
$$
故对于所有包含原点的曲线$C$的值相同，不妨令$\bold{r}=<cost,sint>$
$$
\oint_C\bold{F}\cdot d\bold{r}=\int_0^{2\pi}(sint,-cost)\cdot (-sint,cost)dt\\
=\int_0^{2\pi}-dt=-2\pi
$$
## Divergence and Curl
If $\bold{F} = 〈 P, Q, R 〉$ is a vector field in $ℝ^3$ and $P_x$, $Q_y$, and $R_z$ **all exist**, then the divergence of $\bold{F}$ is defined by
$$
div\bold{F}=P_x+Q_y+R_z
$$
注意散度是关于点$(x,y,z)$的数值函数
In terms of the gradient **operator** $∇ = \bigg(\dfrac{\partial}{\partial x},\dfrac{\partial}{\partial y},\dfrac{\partial}{\partial z} \bigg)$,  divergence can be written symbolically as the dot product
$$
div\bold{F}=∇\cdot \bold{F}
$$
如果场$\bold{F}$是速度场，那么在场中某一点$P$的散度$div\bold{F}(P)$就是单位时间内离开点$P$的净离开量
### 磁场的散度为0
### Divergence of a Source-Free Vector Field
If $\bold{F} = 〈 P, Q 〉$ is a source-free continuous vector field with differentiable component functions, then div $\bold{F} = 0$.
无源场的闭合曲线线积分为0，闭合曲线可以任意缩小至一点，则这点的通量为0，则散度为0
### Divergence Test for Source-Free Vector Fields
Let $\bold{F} = 〈 P, Q 〉$ be a continuous vector field with differentiable component functions with a domain that is simply connected. Then, div $\bold{F} = 0$ if and only if $\bold{F}$ is source free.
### 通量的散度定义
通量
$$
\oint_C\bold{F}\cdot \bold{N}dt=\iint_D(P_x+Q_y)dA=\underbrace{\iint_Ddiv\bold{F}dA}_{每个点的散度在D上的积分}
$$
### Curl
If $\bold{F} = 〈 P, Q, R 〉$ is a vector field in $ℝ^3$ , and $P_x$, $Q_y$, and $R_z$ all exist, then the curl of $\bold{F}$ is defined by
$$
curl\bold{F}=(R_y-Q_z)\bold{i}+(P_z-R_x)\bold{j}+(Q_x-P_y)\bold{k}
$$
旋度是向量
旋度就是扭矩，$\tau = \vec{r}\times \vec{F}$，某点的旋度越大表示越能**更快地**扭动附近的点绕着以旋度向量为轴做旋转
旋度就是通过改变物体运动状态对物体做功的能力，旋度越大就越能更快地改变物体的运动状态
旋度的记忆
$$
curl\bold{F}=\left|
    \begin{matrix}
    \bold{i}&\bold{j}&\bold{k}\\
    \dfrac{\partial}{\partial x}&\dfrac{\partial}{\partial y}&\dfrac{\partial}{\partial z}\\
    P&Q&R
    \end{matrix}
\right|=∇\times \bold{F}
$$
如果是$\R^2$
$$
curl\bold{F}=\left|
\begin{matrix}
\bold{i}&\bold{j}&\bold{k}\\
\dfrac{\partial}{\partial x}&\dfrac{\partial}{\partial y}&0\\
P&Q&0
\end{matrix}
\right|=(Q_x-P_y)\bold{k}
$$
### Divergence of the Curl
Let $\bold{F} = 〈 P, Q, R 〉$ be a vector field in ℝ^3 such that the component functions all have continuous second-order partial derivatives. Then, $div ( curl (\bold{F}) )= ∇ · (∇ × \bold{F}) = 0$.
该定理说明，如果$\bold{F}$是某一个场的旋度场，那么$div(\bold{F})=0$
**proof**
$$
curl\bold{F}=(R_y-Q_z)\bold{i}+(P_z-R_x)\bold{j}+(Q_x-P_y)\bold{k}\\
div\quad (curl\bold{F})=∇\cdot crul(\bold{F})\\
=R_{yx}-Q_{zx}+P_{zy}-R_{xy}+Q_{xz}-P_{yz}=0
$$
**如果一个场的散度不为0，那么该场不是另外一个场的旋度**
### Curl of a Conservative Vector Field
If $\bold{F} = 〈 P, Q, R 〉$ is conservative, then $curl (\bold{F}) = \bold{0}$.
在$\R^2$上，场$\bold{F}$的旋度为
$$
curl(\bold{F})=(Q_x-P_y)\bold{k}
$$
如果场$\bold{F}$为保守场，那么
$$
Q_x-P_y=0
$$
故
$$
curl(\bold{F})=\bold{0}
$$
因为场为保守场，所以存在势函数$f$，则
$$
∇ \times ∇f=\bold{0} 
$$
简写为
$$
∇ \times \underbrace{∇}_{梯度} =\bold{0}
$$
当物体在保守场内做闭环运动时，保守场不对物体做功，这个功也包括不会让物体旋转位移的功，因此其旋度应为0
格林公式
$$
W=\oint_C\bold{F_{conservative}}\cdot d\bold{r}=\iint_DQ_x-P_ydA=\iint_Dcurl(\bold{F})\cdot (0,0,1) dA=0
$$
### Curl Test for a Conservative Field
Let $\bold{F} = 〈 P, Q, R 〉$ be a vector field in space on a simply connected domain. If $curl (\bold{F}) = 0$, then $\bold{F}$ is conservative.
## Surface Integrals
### 平面参数化定义
Given a parameterization of surface $\bold{r}(u, v) = 〈 x(u, v), y(u, v), z(u, v) 〉$ , the parameter domain of the parameterization is the set of points in the uv-plane that can be substituted into $\bold{r}$.
### 一些参数化的平面
$$
\bold{r}=<cosu,sinu,v>,(u,v)\in \R^2\\
x^2+y^2=1,z=v\\
\bold{r}=<ucosv,usinv,u^2>,u\in (0,\infin)\\
x^2+y^2=u^2,z=u^2\\
\bold{r}=<vcosu,vsinu,v>,v\in(-1,\infin)\\
x^2+y^2=z^2,z>-1\\
\bold{r}(\theta,\phi)=<\rho  sin\phi cos\theta,\rho sin\phi sin\theta,\rho cos\phi>,\theta\in [0,\dfrac{\pi}{2}],\phi\in[0,\pi]\\
x^2+y^2+z^2=\rho^2\\
\bold{r}(x,y)=<x,y,z(x,y)>,(x,y)\in D\\
z=z(x,y)\\
\bold{r}(x,z)=<x,y(x,z),z>,(x,z)\in D\\
y=y(x,z)\\
\bold{r}(x,z)=<x(y,z),y,z>,(y,z)\in D\\
x=x(y,z)
$$
### parametric regulation
为了保证参数化后的是平面
Parameterization $\bold{r}(u, v) = 〈 x(u, v), y(u, v), z(u, v) 〉$ is a regular parameterization if $\bold{r}_u × \bold{r}_v$ is not $\bold{0}$ for point $(u, v)$ in the parameter domain.
相似的，为了保证曲线的参数化是曲线，则$\bold{r}'(t)\neq \bold{0}$(向量值函数的导数还是向量值函数，而不是0向量)
### 光滑性
如果一个参数化曲面是光滑的，那么曲面连续且没有角和尖，可导可微
A surface parameterization $\bold{r}(u, v) = 〈 x(u, v), y(u, v), z(u, v) 〉$ is smooth if vector $(\bold{r}_u × \bold{r}_v)\vert_{(u,v)}$ is not $\bold{0}$ for any choice of $u$ and $v$ in the parameter domain.
### example
determine whether the surface is smooth
$$
\bold{r}=< (2+cosv)cosu,(2+cosv)sinu,sinv>,u\in [0,2\pi),v\in [0,2\pi)
$$
$$
\bold{r}_u=<-(2+cosv)sinu,(2+cosv)cosu,0>\\
\bold{r}_v=<-cosusinv,-sinusinv,cosv>\\
\bold{r}_u\times \bold{r}_v=[(2 + cos v)cos u cos v]i +[(2 + cos v)sin u cos v]j +[(2 + cos v)sin v]k.
$$
曲面上对任何$(u,v)$，$\bold{r}_u\times \bold{r}_v\neq \bold{0}$因此曲面光滑
### Surface Area of a Parametric Surface
思想1. 因为可微，$du$和$dv$会在$\bold{r}$上带来微小的增量$d\bold{r}_u$和$d\bold{r}_v$
思想2. 当$u$和$v$的变化足够小时，能够用微小的平面的面积表示该曲面的面积，而该微小的曲面的面积的增量就是$d\bold{r}_u$和$d\bold{r}_v$所围成平行四边形面积$\Vert d\bold{r}_u\times d\bold{r}_v\Vert$
Let $\bold{r}(u, v) = 〈 x(u, v), y(u, v), z(u, v) 〉$ with parameter domain D be a smooth parameterization of surface $S$. Furthermore, assume that $S$ is traced out only once as $(u, v)$ varies over $D$. The surface area of $S$ is
$$
\iint_{D_{(u,v)}}\Vert d\bold{r}_u\times d\bold{r}_v\Vert=\iint_{D_{(u,v)}}\Vert du\bold{r}_u\times dv\bold{r}_v\Vert=\iint_{D_{(u,v)}}\Vert \bold{r}_u\times \bold{r}_v\Vert dA
$$
其中
$$
\bold{r}_u=<\dfrac{\partial x}{\partial u},\dfrac{\partial y}{\partial u},\dfrac{\partial z}{\partial u}>,\bold{r}_v=<\dfrac{\partial x}{\partial v},\dfrac{\partial y}{\partial v},\dfrac{\partial z}{\partial v}>
$$
### 计算球面面积
球面的参数化为
$$
\bold{r}(\theta,\phi)=<\rho  sin\phi cos\theta,\rho sin\phi sin\theta,\rho cos\phi>\\
\bold{r}_{\theta}=<-\rho sin\phi sin\theta,\rho sin\phi cos\theta,0>\\
\bold{r}_{\phi}=<\rho cos\theta cos\phi,\rho sin\theta cos\phi,-\rho sin\phi>\\
\bold{r}_u\times \bold{r}_v=\left|
    \begin{matrix}
    \bold{i}&\bold{j}&\bold{k}\\
    -\rho sin\phi sin\theta&\rho sin\phi cos\theta&0\\
    \rho cos\theta cos\phi&\rho sin\theta cos\phi&-\rho sin\phi
    \end{matrix}
    \right|\\=<-\rho^2sin^2\phi cos\theta,-\rho^2 sin^2\phi sin\theta,-\rho^2 sin\phi cos\phi>\\
\
\\
\iint_D\Vert \bold{r}_u\times \bold{r}_v\Vert dA=\iint_D(\rho^2sin\phi)dA\\
=\int_0^{2\pi}\int_0^{\pi}\rho^2sin\phi d\phi d\theta=\rho^24\pi
$$
$$
(-cos\theta)_0^{\pi}=2
$$
### example2
Find the area of the surface of revolution obtained by rotating $y = x^2, 0 ≤ x ≤ b $ about the x-axis
参数化平面:
绕着x轴旋转，那么在yz平面上是圆圈，则
$$
\bold{r}=<?,rcosu,rsinu>
$$
又因为$y=x^2\rightarrow r=x^2$
所以
$$
\bold{r}=<\sqrt{r},rcosu,rsinu>
$$
不要根号
$$
\bold{r}=<r,r^2cosu,r^2sinu>
$$
### Surface Integral of a Scalar-Valued Function(曲面积分)
The surface integral of a scalar-valued function of $f$ over a piecewise smooth surface $S$ is
$$
\iint_Sf(x,y,z)dS=\lim_{m,n\rightarrow \infin}\sum_{i=1}^m\sum_{j=1}^nf(P^*_{ij})\Delta S_{ij}\\
\Delta S_{ij}=\lim_{\Delta u,\Delta v\rightarrow 0}\Vert \bold{r}_u(P_{ij})\times \bold{r}_v(P_{ij})\Vert\Delta u\Delta v
$$
thus
$$
\iint_Sf(x,y,z)dS=\iint_Df(\bold{r}(u,v))\Vert \bold{r}_u\times \bold{r}_v\Vert dA
$$
### Orientation of a Surface
用法向量表示曲面的朝向
曲面$z=f(x,y)$的一个参数化为
$$
\bold{r}(x,y)=<x,y,f(x,y)>
$$
则曲面的法向量由切线的叉乘得到
$$
\bold{N}=\bold{r}_x\times \bold{r}_y\\
=<1,0,f_x>\times <0,1,f_y>\\
=<-f_x,-f_y,1>
$$
则单位法向量表示曲面方向
$$
\bold{N^u}=\dfrac{\bold{r}_x\times \bold{r}_y}{\Vert \bold{r}_x\times \bold{r}_y\Vert}
$$
并不是所有曲面都有方向，只有能分出内外面的曲面才有方向
(莫比乌斯曲面)
也可以用法向量
$$
\bold{N}=\bold{r}_y\times \bold{r}_x
$$
表示曲面的朝向，使之朝向另外一面
### 球面法向量
设球面由
$$
\bold{r}(\theta,\phi)=<Rsin\phi cos\theta,Rsin\phi sin\theta,Rcos\phi>
$$
给出
那么他的法向量$\bold{N}$是
$$
\bold{r}_\phi\times \bold{r}_\theta=\\
<R^2sin^2\phi cos\theta,R^2sin^2\phi sin\theta,R^2cos\phi sin\phi>
$$
### Surface Integral of a Vector Field(曲面场积分)
要求**曲面的通量**，取曲面的微小单元$dS$，假设在此单元上的场$\bold{F}$是相同的，那么其通量就是
$$
dS\overbrace{\bold{F}\cdot \underbrace{\bold{N^u}}_{决定了曲面的朝向}}^{沿着曲面方向通过的量}
$$
所以
Let $\bold{F}$ be a continuous vector field with a domain that contains oriented surface $S$ with unit normal vector $\bold{N^u}$. The surface integral of $\bold{F}$ over $S$ is
$$
\iint_S\bold{F}\cdot d\bold{S}=\iint_S\bold{F}\cdot \bold{N^u}dS=\iint_S\bold{F}\cdot \bold{N}dA
$$
故
$$
\iint_S\bold{F}\cdot \bold{N^u}dS=\iint_D\bigg(\bold{F}(\bold{r}(u,v))\cdot \dfrac{\bold{r}_u\times \bold{r}_v}{\Vert \bold{r}_u\times \bold{r}_v\Vert}\bigg)\Vert \bold{r}_u\times \bold{r}_v\Vert dA
$$
### example
Let $\bold{v}(x, y, z) = 〈 2x, 2y, z 〉$ represent a velocity field (with units of meters per second) of a fluid with constant density $80 kg/m^3$. Let $S$ be hemisphere $x^2 + y^2 + z^2 = 9$ with $z ≥ 0$ such that $S$ is oriented outward.Find the mass flow rate of the fluid across $S$.
$$
\rho\iint_{S}\bold{v}\cdot \bold{N}dA\\
\bold{r}(\phi,\theta)=<3sin\phi cos\theta,3sin\phi sin\theta,3cos\phi>,\phi\in [0,\dfrac{\pi}{2}],\theta\in [0,2\pi]\\
\bold{r}_\phi\times\bold{r}_\theta=<9sin^2\phi cos\theta,9sin^2\phi sin\theta,9cos\phi sin\phi>\\
80\iint_S\bold{v}\cdot \bold{N}dA\\
=80\int_0^{2\pi}\int_0^{\frac{\pi}{2}}<6sin\phi cos\theta,6sin\phi sin\theta,3cos\phi>\cdot <9sin^2\phi cos\theta,9sin^2\phi sin\theta,9cos\phi sin\phi>d\phi d\theta\\
=80\int_0^{2\pi}\int_0^{\frac{\pi}{2}}54sin^3\phi+27cos^2\phi sin\phi d\phi d\theta=7200\pi\\
$$
### 柱面法向量
柱面$x^2+y^2=R^2$的参数化平面是
$$
\bold{r}(\theta,z)=<Rcos\theta,Rsin\theta,z>
$$
$$
\bold{r}_\theta=<-Rsin\theta,Rcos\theta,0>,\bold{r}_z=<0,0,1>\\
\bold{r}_\theta\times \bold{r}_z=<Rcos\theta,Rsin\theta,0>
$$
## Stokes'Theorem
### 曲面边界方向
设曲面$S$的朝向为$\bold{N^u}$，则其边界曲线$C$的**正向**的定义为：
在曲面$S$的朝向一侧放一个圆头，圆头踩着法向量组成的栈道前进，使得曲面在圆头的**左边**。
### 斯托克斯定理
Let $S$ be a piecewise smooth oriented surface with a boundary that is a **simple closed** curve $C$ with **positive orientation**. If $\bold{F}$ is a vector field with component functions that have continuous partial derivatives on an open region containing $S$, then
$$
\underbrace{\oint_C\bold{F}\cdot d\bold{r}}_{\bold{曲线C在场\bold{F}的环量}}=\underbrace{\iint_S  curl(\bold{F})\cdot \bold{N^u}dS}_{\bold{曲面S在场curl(\bold{F})的通量}}\neq \iint_Sdiv(\bold{curl(F)})dS
$$
当曲面$S$是二维平面时，格林公式
$$
\oint_C\bold{F}\cdot d\bold{r}=\iint_DQ_x-P_ydA=\iint_Dcurl{\bold{F}}\cdot \bold{N^u}dA
$$
因此格林公式是斯托克斯公式的特殊情况
**proof**
证明$S:z=f(x,y)$的情况
曲面S有边界C，曲面S的投影为D，D的边界为C'
$$
\bold{r_{S}}(x,y)=<x,y,f(x,y)>\\
\bold{r}_x=<1,0,f_x>,\bold{r}_y=<0,1,f_y>\\
\bold{r}_x\times \bold{r}_y=<-f_x,-f_y,1>
$$
令$\bold{F}=<P,Q,R>$
$$
\iint_Scurl{\bold{F}}\cdot d\bold{S}=\iint_D<(R_y-Q_z),(P_z-R_x),(Q_x-P_y)>\cdot <-f_x,-f_y,1>dA\\
=\iint_D-(R_y-Q_z)f_x-(P_z-R_x)f_y+(Q_x-P_y)dA
$$
此时积分的值仅仅取决于曲面$S$
这个积分表达式很像格林公式
假设$\bold{r_{C'}}(t)=<x(t),y(t)>$是曲面$S$的边界投影$C'$的参数方程，那么$C$的参数方程就为$\bold{r_C}(t)=<x(t),y(t),f(x(t),y(t))>$(参数方程$<x轴坐标，y轴坐标，z轴坐标>$)，$a\leq t\leq b$
$$
\oint_C\bold{F}\cdot d\bold{r_C}=\int_a^b<P,Q,R>\cdot <x'(t),y'(t),z'(t)>dt\\
=\int_a^bPx'(t)+Qy'(t)+R\bigg(f_x\dfrac{dx}{dt}+f_y\dfrac{dx}{dt}\bigg)dt\\
=\int_a^b(P+Rf_x)x'(t)+(Q+Rf_y)y'(t)dt\\
=\int_{C'}<P+Rf_x,Q+Rf_y>\cdot d\bold{r_{C'}}\\
$$
运用格林公式
$$
=\int_{C'}<P+Rf_x,Q+Rf_y>\cdot d\bold{r_{C'}}\\
=\iint_D\bigg((Q+Rf_y)_x-(P+Rf_x)_y\bigg)dA\\
$$
注意到
$$
\bold{r_{S}}(x,y)=<x,y,f(x,y)>\\
P=P(x,y,f(x,y)),Q=Q(x,y,f(x,y)),R=R(x,y,f(x,y))
$$
因此
$$
=\iint_D\bigg(Q_x+Q_ff_x+(R_x+R_ff_x)f_y+Rf_{yx}\bigg)-\\
\bigg(P_y+P_ff_y+(R_y+R_ff_y)f_x+Rf_{yx}\bigg)dA\\
=\iint_D-(R_y-Q_z)f_x-(P_z-R_x)f_y+(Q_x-P_y)dA\\
=\iint_Scurl{\bold{F}}\cdot d\bold{S}
$$
### example
Verify that Stokes’ theorem is true for vector field $\bold{F}(x, y, z) = 〈 y, 2z, x^2 〉$ and surface $S$, where $S$ is the paravbolid $z = 4 - x^2 - y^2$ .
$$
\oint_C\bold{F}\cdot d\bold{r_C}=\iint_Scurl(\bold{F})\cdot d\bold{S}
$$
$curl(\bold{F})$是
$$
curl{\bold{F}}=\nabla \times \bold{F}=[(x^2)_y-(2z)_z]\bold{i}+[y_z-(x^2)_x]\bold{j}+[(2z)_x-y_y]\bold{k}\\
=[0-2]\bold{i}+[0-2x]\bold{j}+[0-1]\bold{k}
$$
$\bold{N}$为
$$
\bold{r_S}=<x,y,4-x^2-y^2>\\
\bold{r_S}_x\times \bold{r_S}_y=<-z_x,-z_y,1>=<2x,2y,1>
$$
$$
\iint_Scurl(\bold{F})\cdot d\bold{S}=\iint_D<-2,-2x,-1>\cdot <2x,2y,1>dA\\
=\int_0^{2\pi}\int_0^2(-4(rcos\theta)-4r^2cos\theta sin\theta-1)rdrd\theta\\
=-4\pi
$$
$\bold{r_C}=<2cos\theta,2sin\theta,0>$
$$
\oint_C\bold{F}\cdot d\bold{r_C}=\int_0^{2\pi}<2sin\theta,0,4cos^2\theta>\cdot <-2sin\theta,2cos\theta,0>d\theta\\
=\int_0^{2\pi}-4sin^2\theta d\theta\\
=-4(\dfrac{1}{2}\theta-\dfrac{1}{4}sin(2\theta))_0^{2\pi}=-4\pi
$$
### surface independent
假设场$\bold{G}$是另外一个场$\bold{F}$的旋度场
$$
\bold{G}=curl(\bold{F})
$$
则有
$$
div(curl(\bold{F}))=div(\bold{G})=0
$$
那么场$\bold{G}$的通量
$$
\iint_S\bold{G}\cdot d\bold{S}=\iint_S\bold{G}\cdot \bold{N^u}dS
$$
与曲面无关，只与曲面的边界曲线$C$及其方向有关
若曲面$S$和曲面$S'$的边界曲线相同并且**曲面朝向**相同，则
$$
\iint_S\bold{G}\cdot d\bold{S}=\iint_{S'}\bold{G}\cdot d\bold{S}=\oint_C\bold{F}\cdot d\bold{r_C}
$$
### example
Calculate the line integral $∫_C\bold{F} · d\bold{r}$, where $\bold{F} = 〈 xy, x^2 + y^2 + z^2, yz 〉$ and $C$ is the boundary of the parallelogram with vertices $(0, 0, 1)$, $(0, 1, 0)$, $(2, 0, −1)$, and $(2, 1, −2)$.
用斯托克斯定理
$curl(\bold{F})$是
$$
curl(\bold{F})=<-z,0,x>
$$
现在要设定曲面，使得其边界曲线$C$为四边形的边，不妨就取四边形所在的平面为曲面
已知平面过点$(0,0,1)$和$(0,1,0)$那么其法向量
$$
\bold{n}=<(0,0,1)-(0,1,0)>\times <(0,0,1)-(2,0,-1)>=<-2,-2,-2>
$$
则平面方程为
$$
-2x-2y-2z+2=0,x+y+z-1=0
$$
故曲面参数化为
$$
\bold{r_S}=<x,y,1-x-y>,0\leq x\leq 2,0\leq y \leq 1
$$
$\bold{N}$为
$$
\bold{N}=<-f_x,-f_y,1>=<1,1,1>
$$
所以
$$
\oint_C\bold{F}\cdot d\bold{r}=\iint_D<-(1-x-y),0,x>\cdot <1,1,1>dA\\
=\int_0^1\int_0^2-1+2x+ydxdy=3\\
$$
## 散度定理
Let $S$ be a piecewise, smooth **closed** surface that **encloses** solid $E$ in space. Assume that $S$ is oriented outward, and let $\bold{F}$ be a vector field with continuous partial derivatives on an open region containing $E$. Then
$$
\iiint_Ediv(\bold{F})dV=\iint_S\bold{F}\cdot d\bold{S}
$$