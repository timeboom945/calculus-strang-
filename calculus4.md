## 重积分
### 二重积分
对于一个区域R，$R=[a,b]\times [c,d]$，有划分$(a=x_0,x_1,...x_n=b)$和$(c=y_0,y_1,...,y_m=d)$， 则在区域R中由函数$z=f(x,y)$确定的体积的黎曼和为
$$
\sum_{i=1}^n\sum_{j=1}^mf(x^*_{[x_{i-1},x_i]},y^*_{[y_{j-1},y_j]})\Delta x\Delta y=\sum_{i=1}^n\sum_{j=1}^mf(x^*_{[x_{i-1},x_i]},y^*_{[y_{j-1},y_j]})\dfrac{b-a}{n}\dfrac{d-c}{m}\\
\iint_Rf(x,y)dA=\lim_{n,m\rightarrow \infin}\sum_{i=1}^n\sum_{j=1}^mf(x^*_{[x_{i-1},x_i]},y^*_{[y_{j-1},y_j]})\Delta x\Delta y
$$
$dA$为$d xdy$
### Properties of Double Integrals
Assume that the functions $f (x, y)$ and $g(x, y)$ are integrable over the rectangular region $R$; $S$ and $T$ are subregions of $R$; and assume that $m$ and $M$ are real numbers.
1. The sum $f (x, y) + g(x, y)$ is integrable and
$$
\iint_R [f+g]dA=\iint_RfdA+\iint_RgdA
$$
2. If $c $ is a constant, then $c f (x, y)$ is integrable and
$$
\iint_RcfdA=c\iint_RfdA
$$
3.  If $R = S ∪ T$ and $S ∩ T = ∅$ except an overlap on the boundaries, then
$$
\iint_RfdA=\iint_SfdA+\iint_TfdA
$$
4. If $f (x, y) ≥ g(x, y)$ for $(x, y)$ in $R$, then
$$
\iint_RfdA\geq \iint_RgdA
$$
5.  If $m ≤ f (x, y) ≤ M$, then
$$
m\times Area(R)\leq \iint_RfdA\leq M\times Area(R)
$$
6. In the case where $f (x, y)$ can be factored as a product of a function $g(x)$ of $x$ only and a function $h(y)$ of $y$ only, then over the region $R =\{(x, y)|a ≤ x ≤ b, c ≤ y ≤ d\}$, the double integral can be written as
$$
\iint_R fdA=\bigg(\int_a^bgdx\bigg)\bigg(\int_c^dhdy\bigg)
$$
注意A是一个方形
### Iterated Integrals and Fubini’s Theorem
Suppose that $f (x, y)$ is a function of two variables that is continuous over a **rectangular region** $R =\{(x, y) ∈ ℝ^2 |a ≤ x ≤ b, c ≤ y ≤ d\}$ 
$$
\iint_Rf(x,y)dxdy=\int_a^b\left[\int_c^df(x,y)dy\right]dx\\
\iint_Rf(x,y)dxdy=\int_c^d\left[\int_a^bf(x,y)dx\right]dy\\
$$
More generally, Fubini’s theorem is true if $f$ is **bounded**(有界) on $R$ and $f$ is discontinuous only on a finite number of continuous curves. In other words, $f$ has to be integrable over $R$.
$$
\int_c^df(x,y)dy
$$
就是$y$轴切片的面积
### 交换积分次序
evaluate
$$
\iint_R xsin(xy)dA
$$
over the region $R =\{(x, y)|0 ≤ x ≤ \pi, 0 ≤ y ≤ 2\}$
$$
\begin{aligned}
\int_0^2\left[\int_0^{\pi}xsin(xy)dx\right]dy&=\int_0^2\left[\int_0^{\pi y}\dfrac{xysin(xy)}{y^2}dxy\right]dy\\&=\int_0^2\dfrac{1}{y^2}\left[sin(u)-ucos(u)\right]\vert_0^{\pi y}dy\\
&=\int_0^2\dfrac{1}{y^2}(sin(\pi y)-\pi ycos(\pi y))dy
\end{aligned}\\
\begin{aligned}
\int_0^\pi\left[\int_0^2xsin(xy)dy\right]dx&=\int_0^{\pi}\left[\int_0^{2x}sin(xy)dxy\right]dx\\
&=\int_0^{\pi}-cos(u)\vert_0^{2x}dx\\
&=-\int_0^{\pi}(cos(2x)-1)dx\\
&=-\dfrac{sin2x}{2}\vert_0^{\pi}+\pi\\
&=\pi 
\end{aligned}
$$
### Applications of Double Integrals
The area of R is given by
$$
S=\iint_R 1dA
$$
The average value of a function of two variables over a region R is
$$
f_{ave}=\dfrac{1}{AreaR}\iint_Rf(x,y)dA
$$
## General Regions of Integration
A Type I region lies between two vertical lines and the graphs of two functions of x.
A Type II region lies between two horizontal lines and the graphs of two functions of y.
A region $D$ in the $xy$ -plane is of Type I if it lies between two vertical lines and the graphs of two continuous functions $g1 (x)$ and $g2 (x)$. That is
$$
D =\{(x, y)|a ≤ x ≤ b, g_1 (x) ≤ y ≤ g_2 (x)\}
$$
A region $D$ in the $xy$ plane is of Type II if it lies between two horizontal lines and the graphs of two continuous functions $h1 (y)$ and $h2 (y)$. That is
$$
D =\{(x, y)|c ≤ y ≤ d, h1 (y) ≤ x ≤ h2 (y)\}
$$
### Double Integrals over Nonrectangular Regions
Suppose $g(x, y)=\begin{cases}f(x,y),(x,y)\in R\\0,others\end{cases}$ is the extension to the rectangle $R$ of the function $f (x, y)$ defined on the regions $D$ . Then $g(x, y)$ is integrable and we define the double integral of $f (x, y)$ over $D$ by
$$
\iint_Df(x,y)dA=\iint_Rg(x,y)dA
$$
### Fubini’s Theorem (Strong Form)
For a function $f (x, y)$ that is continuous on a region $D$ of Type I, we have
$$
\iint_D f(x,y)dA=\int_a^b\left[\int_{g_1(x)}^{g_2(x)}f(x,y)dy\right]dx
$$
Similarly, for a function $f (x, y)$ that is continuous on a region $D$ of Type II, we have
$$
\iint_Df(x,y)dA=\int_c^d\left[\int_{h_1(y)}^{h_2(y)}f(x,y)dx\right]dy   
$$
### Decomposing Regions into Smaller Regions
Suppose the region $D$ can be expressed as $D = D1 ∪ D2$ where $D1$ and $D2$ do not overlap except at their boundaries. Then
$$
\iint_DfdA=\iint_{D_1}fdA+\iint_{D_2}fdA
$$
### Improper Double Integrals
If R is an unbounded rectangle such as $\{R =(x, y): a ≤ x ≤ ∞, c ≤ y ≤ ∞\}$, then when the limit exists, we have
$$
\iint_Rf(x,y)dA=\lim_{(b,d)\rightarrow \infin}\int_a^b\bigg(\int_c^df(x,y)dy\bigg)dx
$$
### example
Evaluate the integral $\iint_R xye^{-x^2-y^2}dA$, where R is the first quadrant of the plane.
$$
\begin{aligned}
\iint_R xye^{-x^2-y^2}dA&=\int_0^b\dfrac{x}{2}\int_0^{d^2}e^{-x^2-y^2}dy^2dx\\&=\int_0^b-\dfrac{x}{2}[e^{-x^2-y^2}]\vert^{d^2}_0dx\\&=\int_0^b-\dfrac{x}{2}(e^{-x^2-d^2}-e^{-x^2})dx\\&=\dfrac{1}{4}[e^{-x^2-d^2}]\vert_0^{b^2}-\dfrac{1}{4}[e^{-x^2}]\vert_0^{b^2}\\&=\dfrac{1}{4}[e^{-b^2-d^2}-e^{-d^2}-e^{-b^2}+1]
\end{aligned}\\
\lim_{(b,d)\rightarrow (\infin,\infin)}\int_0^b\dfrac{x}{2}\int_0^{d^2}e^{-x^2-y^2}dy^2dx=\lim_{(b,d)\rightarrow (\infin,\infin)}\dfrac{1}{4}[e^{-b^2-d^2}-e^{-d^2}-e^{-b^2}+1]=\dfrac{1}{4}
$$
solve 2
$$
\begin{aligned}
\iint_R xye^{-x^2-y^2}dA&=\iint_Rxe^{-x^2}ye^{-y^2}dA\\&=\int_0^bxe^{-x^2}dx\int_0^dye^{-y^2}dy\\
&=-\dfrac{1}{2}e^{-x^2}\vert_0^{b^2}\times -\dfrac{1}{2}e^{-y^2}\vert_0^{d^2}\\&=\dfrac{1}{4}(e^{-b^2}-1)(e^{-d^2}-1)
\end{aligned}
$$
### 联合概率密度分布
Consider a pair of continuous random variables $X$ and $Y$, such as the birthdays of two people or the number of sunny and rainy days in a month. The joint density function $f$ of $X$ and $Y$ satisfies the probability that $(X, Y)$ lies in a certain region $D$:
$$
P((X,Y)\in D)=\iint_Df(x,y)dA
$$
Since the probabilities can never be negative and must lie between $0$ and $1$, the joint density function satisfies the following inequality and equation:
$$
f(x,y)\geq0,\iint_{R^2}f(x,y)dA=1
$$
The variables $X$ and $Y$ are said to be independent random variables if their joint density function is the product of their individual density functions:
$$
f (x, y) = f_1 (x) f_2 (y)
$$
### expects
In probability theory, we denote the expected values $E(X)$ and $E(Y)$, respectively, as the most likely outcomes of the events. The expected values $E(X)$ and $E(Y)$ are given by
$$
E(X)=\iint_Sxf(x,y)dA=\int x\int f(x,y)dydx\\
E(Y)=\iint_Syf(x,y)dA=\int y\int f(x,y)dxdy
$$
where $S$ is the sample space of the random variables $X$ and $Y$.
##  Double Integrals in Polar Coordinates
$$
dA=\dfrac{d\theta}{2}(r+dr)^2-\dfrac{d\theta}{2}r^2=\dfrac{d\theta}{2}(d^2r+2rdr)=rdrd\theta+o(drd\theta)\\
$$
注意，$dS=\dfrac{\partial S}{\partial \theta}d\theta+\dfrac{\partial S}{\partial r}dr$并不是一小块区域的面积，而是大扇形减去小扇形的面积
The double integral of the function $f (r, θ)$ over the polar rectangular region $R$ in the $rθ$ -plane is defined as
$$
\begin{aligned}
\iint_Rf(r,\theta)dA&=\lim_{(m,n)\rightarrow \infin}\sum_1^m\sum_1^n \overbrace{f(r^*,\theta^*)}^{柱形的高}dA\\&=\lim_{(m,n)\rightarrow \infin}\sum_1^m\sum_1^n f(r^*,\theta^*)r^*\Delta r\Delta\theta   
\end{aligned} 
$$
### example
Evaluate the integral 
$$
\iint_R(1-x^2-y^2)dA
$$
where R is the unit circle on the xy -plane
$$
\begin{aligned}
\int_0^{2\pi}\int_0^1(1-r^2cos^2\theta-r^2sin^2\theta)rdrd\theta&=\int_0^{2\pi}(\dfrac{1}{2}-cos^2\theta\dfrac{r^4}{4}\vert_0^1-sin^2\theta\dfrac{r^4}{4}\vert_0^1)d\theta\\
=&\int_0^{2\pi}\dfrac{1}{2}-\dfrac{1}{4}cos^2\theta-\dfrac{1}{4}sin^2\theta d\theta\\
&=\pi-\dfrac{1}{4}\theta\vert_0^{2\pi}\\
&=\dfrac{\pi}{2}    
\end{aligned}
$$
### example2
Evaluate the integral
$$
\iint_R(x+y)dA
$$
where $R =\{(x, y)|1 ≤ x^2 + y^2 ≤ 4, x ≤ 0\}$
$$
\begin{aligned}
\iint_RfdA&=\int_1^2\int_{\frac{\pi}{2}}^{\frac{3\pi}{2}}(rcos\theta+rsin\theta)rd\theta dr\\
&=\int_1^2r^2(sin\theta\vert_{\frac{\pi}{2}}^{\frac{3\pi}{2}}-cos\theta\vert_{\frac{\pi}{2}}^{\frac{3\pi}{2}})dr\\
&=\dfrac{-2}{3}r^3\vert_1^2\\
&=-\dfrac{14}{3}
\end{aligned}
$$
### Double Integrals over General Polar Regions
If $f (r, θ)$ is continuous on a general polar region $ D$ as described above, then
$$
\iint_Df(r,\theta)rdrd\theta=\int_\alpha^\beta\int_{r=h_1(\theta)}^{r=h_2(\theta)}f(r,\theta)rdrd\theta
$$
积的角度是常数
$r=\alpha$和$r=\beta$两个函数
### example
Find the volume of the solid that lies under the paraboloid $z = 4 − x^2 − y^2$ and above the disk $(x − 1)^2 + y2 = 1$ on the xy-plane
$$
\begin{aligned}
&\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\int_0^{2cos\theta}(4-r^2cos^2\theta-r^2sin^2\theta)rdrd\theta\\
&=\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}(2r^2-\dfrac{1}{4}r^4)\vert_0^{2cos\theta}d\theta\\
&=\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}8cos^2\theta-4cos^4\theta d\theta\\
&=8\int_0^{\frac{\pi}{2}}cos^2\theta(2-cos^2\theta)d\theta\\
&=8\int_0^{\frac{\pi}{2}}cos^2\theta(1+sin^2\theta)d\theta\\
&=8(\dfrac{1}{2}\theta+\dfrac{1}{4}sin(2\theta))\vert_0^{\frac{\pi}{2}}+\int_0^{\frac{\pi}{2}}sin^2(2\theta)d2\theta\\
&=2\pi+(\theta-\dfrac{1}{4}sin(4\theta))\vert_0^{\frac{\pi}{2}}\\
&=2\pi+\dfrac{\pi}{2}\\
\end{aligned}
$$
### try
Find the area enclosed by the circle $r = 3 cos θ $ and the cardioid $r = 1 + cos θ$ 
## 三重积分
We can define a rectangular box $B$ in $ℝ^3$ as $B =\{(x, y, z)|a ≤ x ≤ b, c ≤ y ≤ d, e ≤ z ≤ f\}$, and there is a partition $(a=x_0,x_1,..,x_p=b), (c=y_0,y_1,...,y_q=d),(e=z_0,z_1,...,z_t=f)$, then the Riemann sum is
$$
\sum_1^p\sum_1^q\sum_1^t f(x^*_{[x_{i-1},x_i]},y^*_{[y_{i-1},y_i]},z^*_{[z_{i-1},z_i]})\Delta V
$$
then
$$
\lim_{p,q,t\rightarrow \infin}\sum_1^p\sum_1^q\sum_1^t f(x^*_{[x_{i-1},x_i]},y^*_{[y_{i-1},y_i]},z^*_{[z_{i-1},z_i]})\Delta x\Delta y\Delta z=\iiint_Bf(x,y,z)dV
$$
### Fubini’s Theorem for Triple Integrals
If $f (x, y, z)$ is continuous on a rectangular box $B = [a, b] × [c, d] × [e, f ]$, then
$$
\iiint_Bf(x,y,z)dV=\int_e^b\int_c^d\int_a^bf(x,y,z)dxdydz
$$
化成三个单次积分
### Triple Integral over a General Region——Type 1
The triple integral of a continuous function $f (x, y, z)$ over a general three-dimensional region
$$
E=\{(x,y,z)\vert (x,y)\in D,u_1(x,y)\leq z\leq u_2(x,y)\}
$$
in $ℝ^3$, where $D$ is the projection of $E$ onto the $xy -plane$, is
$$
\iiint_Ef(x,y,z)dV=\iint_D\int_{u_1(x,y)}^{u_2(x,y)}f(x,y,z)dzdA
$$
如果定义域区域能够用其他两个维度去表示第三个维度，就可以化作一个单词积分和一个二次积分
### example
Find the volume of a right pyramid that has the square base in the xy -plane $[−1, 1] × [−1, 1]$ and vertex at the point $(0, 0, 1)$ as shown in the following figure.
$$
\iiint_V1dV=8\iiint_{V'}1dV'
$$
$V'$是平面$x+z=1$(xz平面从第一象限截坐标轴)和平面$y=x$及$z=0$围成的区域
$$
\begin{aligned}
\iiint_{V'}dV'&=\iint_D\int_0^{1-x}dzdD\\
&=\int_0^1\int_0^x(1-x)dydx\\
&=\int_0^1x(1-x)dx\\
&=\dfrac{1}{2}-\dfrac{1}{3}\\
&=\dfrac{1}{6}
\end{aligned}
$$
那么其体积为$8\dfrac{1}{6}=\dfrac{4}{3}$
### Changing the Order of Integration
Consider the iterated integral
$$
\int_{x=0}^{x=1}\int_{y=0}^{y=x^2}\int_{z=0}^{z=y}f(x,y,z)dzdydx
$$
交换积分顺序
$$
\iint_{D_{xy}}\int_{z=0}^{\overbrace{z=y}^{将z弄到D_{xy}上去}}fdzdydx=\iint_{D_{xz}}\int_{\underbrace{y=z}_{下界平面}}^{\overbrace{y=x^2}^{上界平面}}fdydD_{xz}=\iint_{D_{yz}}\int_{x=\sqrt{y}}^{x=1}fdxdD_{yz}
$$
交换积分次序
$$
\begin{aligned}
\iint_{D_{xy}}\int_0^yxyzdzdD_{xy}&=\iint_{D_{xy}}xy\dfrac{1}{2}y^2dD_{xy}\\
&=\dfrac{1}{2}\int_0^1x\int_0^{x^2}y^3dydx\\
&=\dfrac{1}{8}\int_0^1x^{9}dx\\
&=\dfrac{1}{8}\dfrac{1}{10}
\end{aligned}
$$
$$
\begin{aligned}
\iint_{D_{xz}}\int_z^{x^2}xyzdydD_{xz}&=\iint_{D_{xz}}xz\dfrac{1}{2}(x^4-z^2)dD_{xz}\\
&=\dfrac{1}{2}\int_0^1x\int_{z=0}^{z=x^2}x^4z-z^3dzdx\\
&=\dfrac{1}{2}\int_0^1x(x^4\dfrac{1}{2}z^2\vert_0^{x^2}-\dfrac{1}{4}z^4\vert_0^{x^2})dx\\
&=\dfrac{1}{2}\int_0^1\dfrac{1}{2}x^9-\dfrac{1}{4}x^9dx\\
&=\dfrac{1}{8}\dfrac{1}{10}
\end{aligned}
$$
$$
\begin{aligned}
\iint_{D_{yz}}\int_{x=\sqrt{y}}^1xyzdxdD_{yz}&=\iint_{D_{yz}}yz\dfrac{1}{2}(1-y)dD_{yz}\\
&=\dfrac{1}{2}\int_0^1z\int_{y=z}^{y=1}y-y^2dydz\\
&=\dfrac{1}{2}\int_0^1z(\dfrac{1}{2}(1-z^2)-\dfrac{1}{3}(1-z^3))dz\\
&=\dfrac{1}{2}[\dfrac{1}{4}-\dfrac{1}{8}-\dfrac{1}{6}+\dfrac{1}{15}]\\
&=\dfrac{1}{80}
\end{aligned}
$$
投影、向下曲面表达式非常重要
### example
evaluate
$$
\iiint_E\sqrt{x^2+z^2}dV
$$
where $E$ is the region bounded by the paraboloid $y = x^2 + z^2$ and the plane y = 4.
$$
\begin{aligned}
\iint_{D_{xz}}r\int_{r^2}^4dydD_{xz}&=\iint_{D_{xz}}4r-r^3dD_{xz}\\
&=\int_0^{2\pi}\int_0^2(4r-r^3)rdrd\theta\\
&=\int_0^{2\pi}\dfrac{4}{3}8-\dfrac{1}{5}32d\theta\\
&=\dfrac{32}{3}2\pi-\dfrac{32}{5}2\pi\\
&=\dfrac{128}{15}\pi
\end{aligned}
$$
$$
\begin{aligned}
\iiint_E\sqrt{x^2+z^2}dV&=\int_0^4\iint_{D_{xz}(y)}rdD_{xz}(y)dy\\
&=\int_0^4\int_0^{2\pi}\int_0^{\sqrt{y}}r^2drd\theta dy\\
&=\int_0^4\int_0^{2\pi}\dfrac{1}{3}y^{\frac{3}{2}}d\theta dy\\
&=\dfrac{2\pi}{3}\int_0^4y^{\frac{3}{2}}dy\\
&=\dfrac{4\pi}{15}(4^{\frac{5}{2}})\\
&=\dfrac{128\pi}{15}
\end{aligned}
$$
### Average Value of a Function of Three Variables
If $f (x, y, z)$ is integrable over a solid bounded region $E$ with positive volume $V(E)$, then the average value of the function is
$$
f_{ave}=\dfrac{1}{V(E)}\iiint_Ef(x,y,z)dV
$$
## 柱坐标和球坐标三重积分
### 柱极坐标
Consider the cylindrical box (expressed in cylindrical coordinates)
$$
B =\{(r, θ, z)|a ≤ r ≤ b, α ≤ θ ≤ β, c ≤ z ≤ d\}.
$$
If the function $f (r, θ, z)$ is continuous on B and if $(r^*_{ijk}, θ^*_{ijk}, z^*_{ijk})$ is any sample point in the cylindrical subbox $B_{i jk} = [r_{i − 1}, r_i] ×[θ_{j − 1}, θ_ j]× [z_{k − 1}, z_k]$, then we can define the triple integral in cylindrical coordinates as the limit of a triple Riemann sum, provided the following limit exists:
$$
\lim_{l,m,n\rightarrow \infin}\sum_{i=1}^l\sum_{j=1}^m\sum_{k=1}^nf(r^*_{ijk}, θ^*_{ijk}, z^*_{ijk})r^*_{ijk}\Delta r\Delta \theta\Delta z
$$
### Fubini’s Theorem in Cylindrical Coordinates
Suppose that $g(x, y, z)$ is continuous on a rectangular box B, which when described in cylindrical coordinates looks like $B =\{(r, θ, z)|a ≤ r ≤ b, α ≤ θ ≤ β, c ≤ z ≤ d\}$.
Then $g(x, y, z) = g(r cos θ, r sin θ, z) = f (r, θ, z)$ and
$$
\iiint_Bg(x,y,z)dV=\int_c^d\int_{\alpha}^{\beta}\int_a^bf(r,\theta,z)rdrd\theta dz
$$
当三个单次积分上下限都是常数时，可以任意交换
### 柱面坐标系积法
几种积法
1. 先求得上下直线，求切面，旋转求旋转体
2. 先求得上下直线，旋转成柱面，(shell)左右积得旋转体
3. 先旋转成圆线，积得圆面，上下积得到立体
4. 先旋转成圆线，上下积得圆柱面，(shell)左右积得旋转体
5. 先左右积得横线，旋转成圆，上下积得立体
6. 先左右积得横线，上下积得切面，旋转成旋转体
Let $E$ be the region bounded below by the cone $z = \sqrt{x^2 + y^2}$ and above by the paraboloid $z = 2 − x^2 − y^2$.
Set up a triple integral in cylindrical coordinates to find the volume of the region, using the following orders of integration:
$$
dzdrd\theta\\
drdzd\theta
$$
$$
\begin{aligned}
\iiint_B1dV&=\iint_{D_{r\theta}}\int_r^{2-r^2}1dzdD_{r\theta}\\
&1. =\int_0^{2\pi}\int_0^1\int_r^{2-r^2}rdzdrd\theta\\
&2. =\underbrace{\int_0^1\int_0^{2\pi}}_{积分上下限是定值且紧挨，可以交换}\overbrace{\int_r^{2-r^2}}^{上减下曲面}rdzd\theta dr\\
&=\iint_{D_{zr}}\int_0^{2\pi}d\theta dD_{zr}\\
&3. =\int_0^1\int_0^{r=z}\int_0^{2\pi}rd\theta drdz+\int_1^2\int_0^{r=\sqrt{2-z}}\int_0^{2\pi}rd\theta drdz\\
&4. =\int_0^1\int_{z=r}^{z=2-r^2}\int_0^{2\pi}rd\theta dzdr\\
&5. =\int_0^1\int_0^{2\pi}\int_0^{r=z}rdrd\theta dz+\int_1^2\int_0^{2\pi}\int^{\sqrt{2-z}}_0rdrd\theta dz\\
&6. =\overbrace{\int_0^{2\pi}\int_{0}^{1}}^{D_{z\theta}^1}\underbrace{\int_0^{r=z}}_{第一段右减左，r=u_1(z,\theta)}rdrdzd\theta+\overbrace{\int_0^{2\pi}\int_1^2}^{D_{z\theta}^2}\overbrace{\int^{\sqrt{2-z}}_0}^{第二段右减左，r=u_2(z,\theta)}rdrdzd\theta
\end{aligned}
$$

**都是常数且紧挨的可以互换**
**对于旋转体，旋转可以和其紧挨的互换**
### example2
Let $E$ be the region bounded below by the $rθ -plane$, above by the sphere $x^2 + y^2 + z^2 = 4$, and on the sides by the cylinder $x^2 + y^2 = 1$. Set up a triple integral in cylindrical coordinates to find the volume of the region using the following orders of integration, and in each case find the volume and check that the answers are the same:
$$
dzdrd\theta\\
drdzd\theta
$$
$$
\begin{aligned}
\iiint_E1dV&=\iint_{D_{r\theta}}\int^{\sqrt{4-r^2}}_0rdzdD_{r\theta}\\
\end{aligned}\\
\iiint_E1dV=\iint_{D_{z\theta}^1}\int_0^1rdrdD_{z\theta}+\iint_{D_{z\theta}^2}\int_0^{\sqrt{4-z^2}}rdrdD_{z\theta}
$$
### 球坐标图像
1. 球
$$
\rho = R
$$
centered at $(0,0,0)$
$$
\rho =2Rsin\phi cos\theta
$$
centered at $(R,0,0)$
$$
\rho=2Rsin\phi sin\theta
$$
centered at $(0,R,0)$
$$
\rho=2Rcos\phi
$$
centered at $(0,0,R)$
2. 半平面
$$
\theta = \theta_0
$$
3. 上下圆锥
$$
\phi = \phi_0
$$
$\phi_0\in (0,\pi),\phi = \dfrac{\pi}{2}$时为平面
### 球坐标三重积分
$$
dA=d\rho\times \underbrace{(\rho d\phi)}_{侧面里宽}\times\overbrace{(\underbrace{\rho sin\phi}_{\rho的投影} d\theta)}^{底面里边长}
$$
没必要选择$(\rho+d\rho)$作为因子，因为积出来除了$\rho^2 sin\phi d\rho d\phi d\theta$其他都是$\rho^2 sin\phi d\rho d\phi d\theta$的高阶无穷小
底面里边长为$\rho sin\phi d\theta$，受到$\phi$的影响。而$\rho d\theta $是底面里边长的最大处，是西瓜切片的中间横截弧长
设有划分$(a=\rho_0,\rho_1,...,\rho_l=b),(\alpha=\theta_0,\theta_1,...,\theta_m=\beta),(ψ=\phi_0,\phi_1,...,\phi_n=\gamma)$，则
$$
\iiint_{\Omega}f(\rho,\theta,\phi)dV\\=\lim_{l,m,n\rightarrow \infin}\sum_{i=1}^l\sum_{j=1}^m\sum_{k=1}^nf(\rho^*_{[\rho_{i-1},\rho_i]},\theta^*_{[\theta_{j-1},\theta_j]},\phi^*_{[\phi_{k-1},\phi_k]})\rho^{*2}_{[\rho_{i-1},\rho_i]}sin\phi \Delta\rho \Delta\theta \Delta\phi
$$
### Fubini’s Theorem for Spherical Coordinates
If $f(ρ, θ, φ)$ is continuous on a spherical solid box $B =[a, b]×[α, β]× [γ, ψ]$, then
$$
\iiint_{\Omega}f(\rho,\theta,\phi)\rho^2 sin\phi d\rho d\phi d\theta=\int_a^b\int_{\alpha}^{\beta}\int_{γ}^ψf(\rho,\theta,\phi)\rho^2 sin\phi d\phi d\theta d\rho
$$
This iterated integral may be replaced by other iterated integrals by integrating with respect to the three variables in other orders.
### example
evaluate
$$
\int_0^{2\pi}\int_0^{\frac{\pi}{2}}\int_0^1\rho^2 sin\phi d\rho d\phi d\theta
$$
$$
\begin{aligned}
&\int_0^{2\pi}\int_0^{\frac{\pi}{2}}\int_0^1\rho^2 sin\phi d\rho d\phi d\theta\\
&=\bigg(\int_0^{2\pi}d\theta\bigg)\bigg(\int_0^{\frac{\pi}{2}}sin\phi d\phi\bigg)\bigg(\int_0^1\rho^2d\rho\bigg)\\
&=2\pi\times1\times \dfrac{1}{3}\\
\end{aligned}
$$
### 球体积
$$
\begin{aligned}
V&=\iiint_{\Omega}dV\\
&=\int_0^{2\pi}\int_0^{\pi}\int_0^R\rho^2 sin\phi d\rho d\phi d\theta\\
&=2\pi\times 2\times \dfrac{1}{3}R^3\\
&=\dfrac{4}{3}\pi R^3
\end{aligned}
$$
### 球面坐标系积法
Set up an integral for the volume of the region bounded by the cone $z=\sqrt{3(x^2+y^2)}$ and the hemisphere $z=\sqrt{4-x^2-y^2}$
$$
\begin{aligned}
\iiint_{\Omega}dV=\int_0^{\theta = 2\pi}\int_0^{\rho=2}\int_0^{arctan\frac{1}{\sqrt{3}}}\rho^2 sin\phi  d\phi d\rho d\theta
\end{aligned}
$$
Let $E$ be the region bounded below by the cone $z=\sqrt{x^2+y^2}$ and above by the sphere $z=x^2+y^2+z^2$ set up a triple integral in spherical coordinates and find the volume of the region using the following orders of integration:
$$
d\rho d\phi d\theta\\
d\phi d\rho d\theta
$$
**积法**
1. 先从表面积到原点成线，后在切面内积成面，后旋转积成体
2. 先从表面积到原点成线，后旋转积成锥面，后对shell积成体
3. 先旋转积成圆线，后从表面积成锥面$(\rho=u(\phi))$，最后shell积成体
4. 先旋转积成圆线，后积成一个球面$(\phi=u(\rho))$，再积成一个球体
5. 先积成上下的弧线，后积成一个切面，最后旋转成旋转体
6. 先积成上下的弧线，后旋转成球面，最后积成旋转体
$$
\begin{aligned}
\iiint_EdV&1.=\int_0^{\theta=2\pi}\int_0^{arctan1}\int_0^{\rho=2Rcos\phi=cos\phi}\rho^2 sin\phi d\rho d\phi d\theta\\
&2. =\int_0^{arctan1}\int_0^{\theta=2\pi}\int_0^{\rho=2Rcos\phi=cos\phi}\rho^2 sin\phi  d\rho d\theta  d\phi \\
&3. =\int_0^{arctan1}\int_0^{\rho=cos\phi}\int_0^{\theta = 2\pi}\rho^2 sin\phi d\theta d\rho d\phi \\
&4. =\int_0^{\rho=\frac{\sqrt{2}}{2}}\int_0^{\phi=arctan1}\int_0^{2\pi}\rho^2 sin\phi d\theta d\phi d\rho+\int_{\rho=\frac{\sqrt{2}}{2}}^1\int_{\phi=0}^{\phi=arccos\rho}\int_0^{2\pi}\rho^2 sin\phi d\theta d\phi d\rho  \\
&5. =\int_0^{\theta=2\pi}\int_0^{\rho=\frac{\sqrt{2}}{2}}\int_0^{arctan1}\rho^2 sin\phi d\phi d\rho d\theta+\int_0^{2\pi}\int_{\rho=\frac{\sqrt{2}}{2}}^1\int_0^{arccos\rho}\rho^2 sin\phi d\phi d\rho d\theta\\
&6. =\int_0^{\rho=\frac{\sqrt{2}}{2}}\int_0^{2\pi}\int_0^{arctan1}\rho^2 sin\phi d\phi d\theta d\rho +\int_{\rho=\frac{\sqrt{2}}{2}}^1\int_0^{2\pi}\int_0^{arccos\rho}\rho^2 sin\phi d\phi d\theta d\rho 
\end{aligned}
$$
### 坐标系转换
Convert the following integral into cylindrical coordinates:
$$
\int_{y=-1}^{y=1}\int_{x=0}^{x=\sqrt{1-y^2}}\int_{z=x^2+y^2}^{z=\sqrt{x^2+y^2}}xyzdzdxdy
$$
$$
\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\int_{arctan{1}}^{\frac{\pi}{2}}\int_0^{\rho=cot\phi csc\phi}\rho^5sin^3\phi cos\theta sin\theta cos\phi  d\rho d\phi d\theta=0\\
\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\int_0^1\int_{z=r^2}^{z=r}zr^3cos\theta sin\theta dzdrd\theta=0
$$
$$
\int_{-a}^acos\theta sin\theta d\theta=0
$$
### Converting from Rectangular Coordinates to Spherical Coordinates
Convert the following integral into spherical coordinates:
$$
\int_0^{3}\int_0^{x=\sqrt{9-y^2}}\int_{z=\sqrt{x^2+y^2}}^{z=\sqrt{18-x^2-y^2}}(x^2+y^2+z^2)dzdxdy
$$
$$
x^2+y^2=9,\sqrt{18-9}=3,\sqrt{9}=3,上下曲面相交\\
\
\\
\begin{aligned}
&\int_0^{3}\int_0^{x=\sqrt{9-y^2}}\int_{z=\sqrt{x^2+y^2}}^{z=\sqrt{18-x^2-y^2}}(x^2+y^2+z^2)dzdxdy\\
&=\int_0^{\frac{\pi}{2  }}\int_0^{arctan1}\int_0^{\rho=\sqrt{18}}\rho^2\rho^2sin\phi d\rho d\phi d\theta
\end{aligned}
$$
### 椭圆体积于微元变换
find the volumn
$$
\dfrac{x^2}{a^2}+\dfrac{y^2}{b^2}+\dfrac{z^2}{c^2}=1
$$
令$x=a\rho sin\phi cos\theta,y=b\rho sin\phi sin\theta,z=c\rho cos\phi$，有$\rho=1$，在把椭圆化成圆后的体积微元 $dxdydz=abc\underbrace{(d\rho sin\phi cos\theta)(d\rho sin\phi sin\theta)(d\rho cos\phi)}_{椭圆的体积微元}=abc(\rho^2 sin\phi d\rho d\phi d\theta)$
$$
V=8\int_0^{\theta=\frac{\pi}{2}}\int_0^{\phi=\frac{\pi}{2}}\int_0^1abc\rho^2 sin\phi d\rho d\phi d\theta=\dfrac{4}{3}abc\pi
$$
**变换**
对满足$\dfrac{x^2}{a^2}+\dfrac{y^2}{b^2}+\dfrac{z^2}{c^2}=1$做代换，令$x=ax',y=by',z=cz'$，那么则有$x'^2+y'^2+z'^2=1$
$$
\iiint_{椭圆}dV=\iiint_{椭圆}\underbrace{dxdydz}_{椭圆的微元}=\iiint_{圆}abc\underbrace{dx'dy'dz'}_{圆的微元}
$$
看微元定积分区域
$$
\iiint_{\Omega_1}dV_{\Omega_1}=\iiint_{\Omega_2}f()dV_{\Omega_2}
$$
if $dV_{\Omega_1}=f()dV_{\Omega_2}$
## center of mass and Moments of inertia
### Center of Mass in Two Dimensions
$$
\bar x=\dfrac{\sum_1^n m_ix_i}{m},\bar y=\dfrac{\sum_1^m m_iy_i}{m}
$$
物体的重心是每个质点坐标的加权平均值
### 点密度的定义
Suppose that the lamina occupies a region $R$ in the xy-plane, and let $ρ(x, y)$ be its density (in units of mass per unit area) at any point $(x, y)$.
Hence, $ρ(x, y) = \lim_{\Delta A\rightarrow \infin}\dfrac{\Delta m}{\Delta A}$ where $Δm$ and $ΔA$ are the mass and area of a small rectangle **containing** the point $(x, y)$  and the limit is taken as the dimensions of the rectangle go to 0
### 薄片质量
有划分$(a=x_0,x_1,...,x_m=b),(c=y_0,y_1,...,y_n=d)$
$$
m=\lim_{m,n\rightarrow \infin}\sum_1^m\sum_1^n\Delta m_{ij}=\lim_{m,n\rightarrow \infin}\sum_1^m\sum_1^n\rho(x^*_{[x_{i-1},x_i]},y^*_{[y_{j-1},y_j]})\Delta x\Delta y
$$
### 力矩
$M_x$表示让x轴转动的效应量大小
$M_{xy}$表示让平面转动的效应量大小
### 重心
review of mass center with constant $\rho$
$$
\bar{x}=\dfrac{M_y}{m}=\dfrac{\int_a^b\overbrace{\rho f(x)dx}^{长条质量}\times x}{\int_a^b \rho f(x)dx}\\
\bar{y}=\dfrac{M_x}{m}=\dfrac{\int_a^b\rho f(x)dx\times\overbrace{\dfrac{f(x)}{2}}^{对称性取中点}}{\int_a^b \rho f(x)dx}
$$
then the $\rho$ becomes $\rho=\rho(x,y)$
$$
\bar{x}=\dfrac{M_y}{m}=\dfrac{\iint_R\rho(x,y)xdxdy}{\iint_R\rho(x,y)dxy}\\
\bar{y}=\dfrac{M_x}{m}=\dfrac{\iint_R\rho(x,y)ydxdy}{\iint_R\rho(x,y)dxy}\\
$$
### the centroid of a region
$$
{x_c}=\dfrac{M_y}{m}=\dfrac{\iint_Rxdxdy}{\iint_Rdxy}\\
{y_c}=\dfrac{M_x}{m}=\dfrac{\iint_Rydxdy}{\iint_Rdxy}\\
$$
### Moments of Inertia
转动惯量
动量=质量(标量)$\times$速度(矢量)
角动量=转动惯量(标量)$\times $角速度(矢量)
动量和角动量守恒
**The moment of inertia of a particle of mass m about an axis is $mr^2$**, where r is the distance of the particle from the axis.
**绕x轴旋转**
The moment of inertia $I_x$ about the x-axis for the region $R$ 
$$
I_x=\iint_R\underbrace{y^2\overbrace{\rho(x,y)dA}^{dm}}_{dmr^2}\\
I_y=\iint_Rx^2\rho(x,y)dA
$$
**绕原点旋转**
$$
I_0=\iint_R\overbrace{(x^2+y^2)}^{r^2}\rho(x,y)dA=I_x+I_y
$$
**有$I_0=I_x+I_y$**
### Center of Mass and Moments of Inertia in Three Dimensions
质量
$$
m=\iiint_{\Omega}\rho(x,y,z)dV\\
$$
力矩
$$
M_{xy}=\iiint_{\Omega}z\rho(x,y,z)dV\\
M_{xz}=\iiint_{\Omega}y\rho(x,y,z)dV\\
M_{yz}=\iiint_{\Omega}x\rho(x,y,z)dV\\
$$
重心
$$
\bar{x}=\dfrac{M_{yz}}{m},\bar{y}=\dfrac{M_{xz}}{m},\bar{z}=\dfrac{M_{xy}}{m}\\
$$
转动惯量
$$
I_x=\iiint_{\Omega}(y^2+z^2)\rho(x,y,z)dV\\
I_y=\iiint_{\Omega}(x^2+z^2)\rho(x,y,z)dV\\
I_z=\iiint_{\Omega}(x^2+y^2)\rho(x,y,z)dV\\
I_0=\iiint_{\Omega}(x^2+y^2+z^2)\rho(x,y,z)dV\\
$$
## Change of Variables in Multiple Integrals
A transformation $T: G → R$, defined as $T(u, v) = (x, y)$ (从坐标系uv映射到坐标系xy), is said to be a one-to-one transformation if no two points map to the same image point.
如果不存在两个不同的点映射到相同的点，就是点对点映射
**$T^{-1}(x,y)=(u,v)$**也是点对点映射
### example
映射$T(r,\theta)=(x,y),x=rcos\theta,y=rsin\theta$是一个点对点映射
假设有$T(r_1,\theta_1),T(r_2,\theta_2)$，有$(x_1,y_1),(x_2,y_2)$，若$(x_1,y_1)=(x_2,y_2)$
$$
x_1=x_2,y_1=y_2\\
r_1cos\theta_1=r_2cos\theta_2\\
r_1sin\theta_1=r_2sin\theta_2\\
cot\theta_1=cot\theta_2\\
\theta_1=\theta_2,\theta\in (0,2\pi)
$$
### 映射的边界特性
Let the transformation T be defined by $T(u, v) = (x, y)$ where $x = u^2 − v^2$ and $y = uv$. Find the image of the triangle in the uv-plane with vertices $(0, 0), (0, 1)$, and $(1, 1)$.
$$
R_{(u,v)}:1\geq v\geq u,u\in [0,1]
$$
**一个连续有偏导的映射必定把一个连通区间映射到另一个连通区间**
映射$T(u,v)=(x,y),x=f(u,v),y=g(u,v)$在区域$R_{(u,v)}$连续有偏导，如果点$(u_0,v_0)$是区域$(u,v)$的边界点，则存在$\Delta u,\Delta v,\sqrt{\Delta^2 u+\Delta^2 v}\rightarrow 0,$$(u_0+\Delta u,v_0+\Delta v)\notin(u,v)$，则点
$$
(f(u_0+\Delta u,v_0+\Delta v),g(u_0+\Delta u,v_0+\Delta v))\notin (x,y)
$$
有因为映射在点$(u_0,v_0)$连续可偏导，故在$\sqrt{\Delta^2 u+\Delta^2 v}\rightarrow 0$时
$$
f(u_0+\Delta u,v_0+\Delta v)= x_0+\dfrac{\partial f}{\partial u}\Delta u+\dfrac{\partial f}{\partial v}\Delta v\\
g(u_0+\Delta u,v_0+\Delta v)= y_0+\dfrac{\partial g}{\partial u}\Delta u+\dfrac{\partial g}{\partial v}\Delta v\\
$$
$\sqrt{\bigg(\dfrac{\partial f}{\partial u}\Delta u+\dfrac{\partial f}{\partial v}\Delta v\bigg)^2+\bigg(\dfrac{\partial g}{\partial u}\Delta u+\dfrac{\partial g}{\partial v}\Delta v\bigg)^2}\rightarrow 0$
因此$(x_0,y_0)$是区域$(x,y)$的边界点。

**逐个判断边界条件**
边界1. $u=0$
$$
x=-v^2,y=0,v\in[0,1]\\
-1\leq x\leq 0,y=0
$$
是一条边界
边界2. $v=1,0\leq u\leq 1$
$$
x=u^2-1,y=u,0\leq u\leq 1\\
x=y^2-1,0\leq y\leq 1
$$
是一条边界
边界3. $u=v,u\in[0,1]$
$$
x=0,y=u^2,u\in[0,1]\\
x=0,0\leq y\leq 1
$$
是一条边界
### 雅可比
为了考察映射$T(u,v)=(x,y)$前后的微元面积$dA_{(u,v)}$和$dA_{(x,y)}$的关系，建立向量值函数
$$
\vec{r}(u,v)=f(u,v)\vec{i}+g(u,v)\vec{j}\\
\vec{r}(u_0,v_0)=f(u_0,v_0)\vec{i}+g(u_0,v_0)\vec{j}=x_0\vec{i}+y_0\vec{j}\\
$$
$$
\dfrac{\partial \vec{r}}{\partial u}=\dfrac{\partial f}{\partial u}\vec{i}+\dfrac{\partial g}{\partial u}\vec{j}=\lim_{\Delta u\rightarrow 0}\dfrac{\vec{r}(u_0+\Delta u,v_0)-\vec{r}(u_0,v_0)}{\Delta u}
$$
$\Delta u\times \dfrac{\partial \vec{r}}{\partial u}$表示$\Delta u$对$(x_0,y_0)$带来的微增长$(\dfrac{\partial f}{\partial u}\Delta u,\dfrac{\partial g}{\partial u}\Delta u)$
同理有
$$
\dfrac{\partial \vec{r}}{\partial v}=\dfrac{\partial f}{\partial v}\vec{i}+\dfrac{\partial g}{\partial v}\vec{j}=\lim_{\Delta u\rightarrow 0}\dfrac{\vec{r}(u_0,v_0+\Delta v)-\vec{r}(u_0,v_0)}{\Delta v}
$$
$\Delta v\times \dfrac{\partial \vec{r}}{\partial v}$表示$\Delta v$对$(x_0,y_0)$带来的微增长$(\dfrac{\partial f}{\partial v}\Delta v,\dfrac{\partial g}{\partial v}\Delta v)$
因此，$dA_{(x_0,y_0)}$面积就是由向量$\Delta u\dfrac{\partial \vec{r}}{\partial u},\Delta v\dfrac{\partial \vec{r}}{\partial v}$组成平行四边形的面积
$$
\lVert\Delta u\dfrac{\partial \vec{r}}{\partial u}\times \Delta v\dfrac{\partial \vec{r}}{\partial v}\rVert\\
\
\\
\dfrac{\partial \vec{r}}{\partial u}\times \dfrac{\partial \vec{r}}{\partial v}=\left|\begin{matrix}
\bold{i}&\bold{j}&\bold{k}\\
\dfrac{\partial f}{\partial u}&\dfrac{\partial g}{\partial u}&0\\
\dfrac{\partial f}{\partial v}&\dfrac{\partial g}{\partial v}&0
\end{matrix}\right|=\left|\begin{matrix}
\overbrace{\dfrac{\partial f}{\partial u}}^{u给x带来的增长趋势}&\overbrace{\dfrac{\partial g}{\partial u}}^{u给y带来的增长趋势}\\
\underbrace{\dfrac{\partial f}{\partial v}}_{v给x带来的增长趋势}&\underbrace{\dfrac{\partial g}{\partial v}}_{v给y带来的增长趋势}
\end{matrix}\right|\bold{k}
$$
则$\lVert\Delta u\dfrac{\partial \vec{r}}{\partial u}\times \Delta v\dfrac{\partial \vec{r}}{\partial v}\rVert=\Delta u\Delta v\lVert\dfrac{\partial \vec{r}}{\partial u}\times \dfrac{\partial \vec{r}}{\partial v}\rVert=\Delta u\Delta v\left\lVert\left|\begin{matrix}
\dfrac{\partial f}{\partial u}&\dfrac{\partial g}{\partial u}\\
\dfrac{\partial f}{\partial v}&\dfrac{\partial g}{\partial v}
\end{matrix}\right|\right\rVert$
**故**
$$
dA_{(x,y)}=\left\lVert\left|\begin{matrix}
\dfrac{\partial f}{\partial u}&\dfrac{\partial g}{\partial u}\\
\dfrac{\partial f}{\partial v}&\dfrac{\partial g}{\partial v}
\end{matrix}\right|\right\rVert dudv=\left\lVert\left|\begin{matrix}
\dfrac{\partial f}{\partial u}&\dfrac{\partial g}{\partial u}\\
\dfrac{\partial f}{\partial v}&\dfrac{\partial g}{\partial v}
\end{matrix}\right|\right\rVert dA_{(u,v)}
$$
### example
finding the Jacobian
$$
T(u,v)=(x,y),x=u^2-v^2,y=uv\\
$$
$$
J(u,v)=\left|\begin{matrix}
2u&v\\
-2v&u
\end{matrix}\right|=2u^2+2v^2\\
dxdy=\vert(2u^2+2v^2)\vert dudv
$$
### Change of Variables for Double Integrals
$\overbrace{T(u,v)}^{想要转换成的}=(x,y),x=x(u,v),y=y(u,v)$
$$
\iint_{V_{(x,y)}}f(x,y)dV_{(x,y)}=\iint_{S=V_{(u,v)}}f(x(u,v),y(u,v))\vert J(u,v)\vert dV_{(u,v)}
$$
### example
Consider the integral $\iint_R(x-y)dydx$, where R is the parallelogram joining the points (1, 2), (3, 4), (4, 3), and (6, 5). 
make appropriate changes of variables, and write the resulting integral.
those lines bounded the parallelogram are
$$
y-2=\dfrac{1}{3}(x-1)\\
y-2=(x-1)\\
y-5=\dfrac{1}{3}(x-6)\\
y-5=(x-6)
$$
thus
$$
3y-x=5\\
y-x=1\\
3y-x=9\\
y-x=-1
$$
令
$$
u=3y-x\\
v=y-x
$$
则
$$
x=\dfrac{u-3v}{2}\\
y=\dfrac{u-v}{2}\\
\vert J(u,v)\vert=\dfrac{1}{2}
$$
therefore
$$
dA_{(x,y)}=\dfrac{1}{2}dudv
$$
$$
\iint_{A_{(x,y)}}x-ydA=\iint_{A_{(u,v)}}(-v)\dfrac{1}{2}dudv=\dfrac{1}{2}\int_{-1}^1\int_{5}^9-vdudv=0
$$
### example2
Using the change of variables $u = x − y$ and $v = x + y$, evaluate the integral
$$
\iint_R(x-y)e^{(x^2-y^2)}dA
$$
where $R $ is the region bounded by the lines $x + y = 1$ and $x + y = 3$ and the curves $x^2 − y^2 = −1$ and $x^2 − y^2 = 1$
$$
x=\dfrac{u+v}{2}\\
y=\dfrac{v-u}{2}\\
J(u,v)=(\dfrac{1}{2}\dfrac{1}{2}-\dfrac{-1}{2}\dfrac{1}{2})=\dfrac{1}{2}\\
dA=\dfrac{1}{2}dudv\\
\iint_R(x-y)e^{(x^2-y^2)}dA=\int_1^3\int_{u=-\frac{1}{v}}^{u=\frac{1}{v}}ue^{uv}\dfrac{1}{2}dudv
$$
### Jacobian for three dimension
要求三维向量的体积微元
$$
\left|
\begin{matrix}
\bold{i}&\bold{j}&\bold{k}&\bold{l}\\
x_u&y_u&z_u&0\\
x_v&y_v&z_v&0\\
x_w&y_w&z_w&0\\
\end{matrix}
\right|=\left|
\begin{matrix}
x_u&y_u&z_u\\
x_v&y_v&z_v\\
x_w&y_w&z_w
\end{matrix}
\right|\bold{l}
$$
并且$\left\lVert\left|
\begin{matrix}
x_u&y_u&z_u\\
x_v&y_v&z_v\\
x_w&y_w&z_w
\end{matrix}
\right|\bold{l}\right\rVert\Delta u\Delta v\Delta w$为所组成平行四面体体积微元
The Jacobian determinant $J(u, v, w)$ in three variables is defined as follows:
$$
J(u,v,w)=\left|
\begin{matrix}
x_u&y_u&z_u\\
x_v&y_v&z_v\\
x_w&y_w&z_w
\end{matrix}
\right|
$$
### Change of Variables for Triple Integrals
Let $\overbrace{T(u, v, w)}^{想要转换成的} = (x, y, z)$ where $x = g(u, v, w)$, $y = h(u, v, w)$, and $z = k(u, v, w)$, be a one-to-one $C^1$(连续有偏导) transformation, with a nonzero Jacobian, that maps the region $G$ in the uvw-plane into the region $D$ in the $xyz-plane$. As in the two-dimensional case, if $F$ is continuous on $D$, then
$$
\iiint_{\Omega_{(x,y,z)}}f(x,y,z)dV_{(x,y,z)}=\iiint_{\Omega_{(u,v,w)}}f(g(),h(),k())\vert J(u,v,w)\vert dV_{(u,v,w)}
$$
### Obtaining Formulas in Triple Integrals for Cylindrical and Spherical Coordinates
$T(r,\theta,z)=(x,y,z),x=rcos\theta,y=rsin\theta,z=z$
$$
J(r,\theta,z)=
\left|
\begin{matrix}
cos\theta&sin\theta&0\\
rsin\theta&-rcos\theta&0\\
0&0&1
\end{matrix}
\right|=-rcos^2\theta-rsin^2\theta=-r\\
dxdydz=rd\theta drdz
$$
$T(\rho,\theta,\phi)=(x,y,z),x=\rho sin\phi cos\theta,y=\rho \sin\phi \sin\theta,z=\rho cos\phi$
$$
J(\rho,\theta,\phi)=\left|
\begin{matrix}
sin\phi cos\theta&sin\phi sin\theta&cos\phi\\
\rho sin\phi sin\theta&-\rho \sin\phi cos\theta&0\\
-\rho cos\phi cos\theta&-\rho cos\phi sin\theta&\rho sin\phi
\end{matrix}
\right|=-\rho^2sin\phi\\
dxdydz=\rho^2sin\phi d\rho d\theta d\phi
$$
### example
Evaluating a Triple Integral with a Change of Variables
$$
\int_0^3\int_0^4\int_{\frac{y}{2}}^{\frac{y}{2}+1}(x+\dfrac{z}{3})dxdydz
$$
边界
$$
x=\dfrac{y}{2}+1\\
x=\dfrac{y}{2}\\
y=4\\
y=0\\
z=3\\
z=0\\
$$
令
$$
u=x-\dfrac{y}{2}\\
v=y\\
w=z\\
$$
则有映射$T(u,v,w)=(x,y,z),x=u+\dfrac{v}{2},y=v,z=w$
$$
J(u,v,w)=\left|
\begin{matrix}
1&0&0\\
\dfrac{1}{2}&1&0\\
0&0&1
\end{matrix}
\right|=1\\
\int_0^3\int_0^4\int_{\frac{y}{2}}^{\frac{y}{2}+1}(x+\dfrac{z}{3})dxdydz=\int_0^3\int_0^4\int_0^1(u+\dfrac{v}{2}+\dfrac{w}{3})dudvdw=24
$$