### 斜率
$$
slop = \dfrac{y_2-y_1}{x_2-x_1}
$$
#### 点斜式
$$
f(x)-y_1 = m(x-x_1)，m为斜率，(x_1,y_1)为已知点
$$
点斜式——————non vertical
#### 标准式
$$
ax + by = c
$$
#### 幂方程
$$
y = ax^b\quad a,b \in R
$$
#### rational functions
$$
f(x) = \dfrac{p(x)}{q(x)}
$$
where p(x) and q(x) are polynominals
#### root function
$$
f(x) = x^{\dfrac{1}{n}},n>1
$$
#### exponential functions
$$
f(x) = b^x\quad b>0,b\neq 1
$$
#### logarithmic function
$$
f(x) = log_b (x)\quad b>0,b\neq 1
$$
### transformations, scaling and reflections of functions
$$
y+a = y_{original}\\
y = y_{original}-a\quad a<0上移；a>0下移\\
\
\\
x + b = x_{original}\\
x = x_{original}-b\quad b<0左移；a>0右移\\
\
\\
c*x = x_{original}\\
x = \dfrac{x_{original}}{c}\quad 0<c<1,expand; c>1,shrink\\
\
\\
c*y = y_{original}\\
y = \dfrac{y_{original}}{c}\quad 0<c<1,pulled; c>1,pushed\\
\
\\
(-1)*x = x_{original}\\
x = -x_{original}\quad 左右对称\\
\
\\
(-1)*y = y_{original}\\
y= -y_{original}\quad 上下对称\\
\
\\
x<-->y互换\\
关于y=x对称
$$
###   trigonometric equations
$$
1 + tan^2\theta=sec^2\theta\\
1 + cot^2\theta = csc^2\theta\\
\
\\
sin(\alpha\pm\beta)=sin\alpha cos\beta\pm cos\alpha sin\beta \\
cos(\alpha\pm\beta)=cos\alpha cos\beta\mp sin\alpha sin\beta \\
\
\\
sin(2\theta) = 2cos\theta sin\theta\\
cos(2\theta) = 2cos^2\theta -1=1-2sin^2\theta=cos^2\theta - sin^2\theta\\
\
\\
cos^2\theta=\dfrac{1+cos2\theta}{2},sin^2\theta=1-cos^2\theta=\dfrac{1-cos2\theta}{2}
$$
###  period
$$
f(x) = Asin(B(x-a))+C\\
\vert A\vert 是振幅amplitude，周期=\dfrac{2\pi}{\vert B\vert}，中心轴线y=C，a是水平移动的距离
$$
###  inverse function
$$
重要 ：xy互换x<--->y,同时xy的取值范围互换\\
\
\\
如果f^{-1}(x)被限定了值域，那么f^{-1}(f(x))=x当且仅当x在f^{-1}(x)的值域内\\
\\
同理f(f^{-1}y)=y当且仅当y在f(x)的值域内\\
\
\\
sin(sin^{-1}y)=y,\quad if -1\leq y\leq 1\\
sin^{-1}(sin(x)) = x,\quad if -\dfrac{\pi}{2} \leq x \leq \dfrac{\pi}{2}\\
\
\\
cos(cos^{-1}y)=y,\quad if -1\leq y\leq 1\\
cos^{-1}(cos(x)) = x,\quad if \quad 0 \leq x \leq \pi\\
$$
### 对数方程
$$
log_b(ac)=log_b(a)+log_b(c)\\
log_b(\dfrac{a}{c})=log_b{a}-log_b{c}\\
log_b(a^r)=rlog_b(a)\\
\
\\
a^x=e^{xlna}=b^{xlog_ba}\\
$$
### hyperbolic functions
$$
coshx=\dfrac{e^x+e^{-x}}{2}\quad sinhx=\dfrac{e^x-e^{-x}}{2}\\
tanhx=\dfrac{e^x-e^{-x}}{e^x+e^{-x}}=\dfrac{sinhx}{coshx}\quad cothx=\dfrac{e^x+e^{-x}}{e^x-e^{-x}}=\dfrac{coshx}{sinhx}\\
sechx=\dfrac{2}{e^x+e^{-x}}=\dfrac{1}{coshx}\quad cschx=\dfrac{2}{e^x-e^{-x}}=\dfrac{1}{sinhx}\\
\
\\
cosh^2-sinh^2=1\\
cosh(x)=cosh(-x)\\
sinh(x)=-sinh(-x)\\
cosh(x)+sinh(x)=e^x\\
cosh(x)-sinh(x)=e^{-x}\\
\
\\
1-tanh^2x=sech^2x\\
coth^2x-1=csch^2x\\
\
\\
sinh(x\pm y)=sinhxcoshy\pm coshxsinhy\\
cosh(x\pm y)=coshxcoshy \pm sinhxsinhy \\
sinh(2x)=2sinhxcoshx\\
cosh(2x)=cosh^2x+sinh^2x=1+2sinh^2x=2cosh^2x-1=e^{2x}-sinh(2x)\\
sinh^2x=\dfrac{cosh(2x)-1}{2},cosh^2x=\dfrac{cosh(2x)+1}{2}
$$
### inverse hyperbolic functions
$$
复合函数反函数:f(g(x))=h(x)\\
h^{-1}(x)=[f(g(x))]^{-1}=g^{-1}(f^{-1}(x)),f^{-1}(x)的值域就是g(x)的值域\\
\
\\
sinh^{-1}x=[f(g(x))]^{-1}=g^{-1}(f^{-1}(x))\quad 这里f(x)=\dfrac{x^2-1}{2x}\quad x>0;g(x)=e^x\\
g^{-1}(f^{-1}(x))=ln((\dfrac{x^2-1}{2x})^{-1}(x>0))\\
求f(x)=\dfrac{x-x^{-1}}{2}上x>0时的反函数:x,y互换有\\
x=\dfrac{y-y^{-1}}{2};y^2-2xy-1=0\\此时\Delta>0,必定有两个不同的解y,其中一个大于0一个小于0\\
求解得y={x\pm \sqrt{x^2+1}},y>0时为x+ \sqrt{x^2+1}\\
故sinh^{-1}x=g^{-1}(f^{-1}(x))=ln(x+ \sqrt{x^2+1})\\
\
\\
步骤：写出f(x)和g(x)=f(g(x))，标定f(x)的定义域x\in g(x)\\
求g^{-1}(x)与f^{-1}(x)，复合g^{-1}(f^{-1}(x))，f^{-1}(x)\in g(x)\\
\
\\
sinh^{-1}x = arcsinhx=ln(x+\sqrt{x^2+1})\quad cosh^{-1}x=arccoshx=ln(x+\sqrt{x^2-1})\\
tanh^{-1}x=arctanhx=\dfrac{1}{2}ln{\dfrac{x+1}{1-x}}\quad coth^{-1}x=arccothx=\dfrac{1}{2}ln{\dfrac{x+1}{x-1}}\\
sech^{-1}x=arcsechx=arccosh(\dfrac{1}{x})(\dfrac{1}{x}>1)=ln{\dfrac{1+\sqrt{1-x^2}}{x}}\quad \\
csch^{-1}x=arccschx=arcsinh(\dfrac{1}{x})(\dfrac{1}{x}\neq 0)=ln{(\dfrac{1}{x}+\dfrac{\sqrt{1+x^2}}{\vert x\vert})}(这是个奇函数，分段函数)\\
f(x)=ln{(\dfrac{1}{x}+\dfrac{\sqrt{1+x^2}}{\vert x\vert})}=\begin{cases}
ln{(\dfrac{1}{x}+\dfrac{\sqrt{1+x^2}}{x})},x>0\\
\\
ln{(\dfrac{1}{x}-\dfrac{\sqrt{1+x^2}}{x})},x<0\\
\end{cases}\\
若x>0,f(x)=ln{(\dfrac{1}{x}+\dfrac{\sqrt{1+x^2}}{x})},f(-x)=ln{(-\dfrac{1}{x}+\dfrac{\sqrt{1+x^2}}{x})}=-ln{(\dfrac{1}{x}+\dfrac{\sqrt{1+x^2}}{x})}=-f(x)\\
$$
### several conclusion
$$
\lim_{x\rightarrow a}\dfrac{1}{(x-a)^n}=+\infin,n为偶数\\
\
\\
\lim_{x\rightarrow a^+}\dfrac{1}{(x-a)^n}=+\infin,n为奇数\\
\lim_{x\rightarrow a^-}\dfrac{1}{(x-a)^n}=-\infin,n为奇数\\
\lim_{x\rightarrow a}\dfrac{1}{(x-a)^n}DNE,n为奇数\\
$$
### vertical asymptote
$$
\lim_{x\rightarrow a^-}f(x)=+\infin or-\infin\quad and\quad\lim_{x\rightarrow a^+}f(x)=+\infin or-\infin\\
or\\
\lim_{x\rightarrow a}f(x)=+\infin or-\infin\\
$$
then x=a is a vertical asymptote
### limit laws
f(x) and g(x) have definition on some open interval containing a,and be defined for all **$\bold{x \neq a}$**:
**极限研究的是自变量不等于该点的函数行为**
$$
\lim_{x\rightarrow a}f(x)=L\\
\lim_{x\rightarrow a}g(x)=M\\
$$
then:
$$
\lim_{x\rightarrow a}(f(x)+g(x))=L+M\\
\lim_{x\rightarrow a}(f(x)-g(x))=L-M\\
\lim_{x\rightarrow a}cf(x)=cL\\
\lim_{x\rightarrow a}f(x)*g(x)=L*M\\
\lim_{x\rightarrow a}\dfrac{f(x)}{g(x)}=\dfrac{L}{M}\quad\quad M\neq 0\\
\lim_{x\rightarrow a}f(x)^n=(\lim_{x\rightarrow a}f(x))^n=L^n\quad对于所有正整数n\\
\lim_{x\rightarrow a}\sqrt[n]{f(x)}=\sqrt[n]{(\lim_{x\rightarrow a}f(x))}=\sqrt[n]L \quad对于所有L\in R和正奇数n或L>0和正偶数n\\
$$
### limits of polynomial and rational functions(its dependent value is R)
for all polynomial and rational functions f(x) and g(x) and a is a point defined
(分段函数不属于基本函数)
$$
\lim_{x\rightarrow a}f(x)=f(a)\\
\lim_{x\rightarrow a}\dfrac{f(x)}{g(x)}=\dfrac{f(a)}{g(a)}\quad g(a)\neq 0
$$
### if f(x) = g(x) and x=a is defined at g but not at f, then
$$
\lim_{x\rightarrow a}f(x) = \lim_{x\rightarrow a}g(x)
$$
### the squeeze theorem
### several trigonometric inequities
$$
sin(\theta)\leq \theta \quad0\leq\theta \leq \dfrac{\pi}{2}\\
对于-\dfrac{\pi}{2}\leq\theta\leq0有0\leq-\theta \leq \dfrac{\pi}{2}，因此sin(-\theta)\leq-\theta，故\theta\leq sin(\theta)\\
综上所述有\vert sin(\theta)\vert \leq\vert \theta\vert\\
sin(\theta)\leq\theta\leq tan(\theta)\quad 0\leq\theta \leq \dfrac{\pi}{2}
$$
### continuity
f(x) is continuity at x = a should satisfy:
$$
 f(a)\quad is\quad defined\\
\lim_{x\rightarrow a}f(x)exists\\
\lim_{x\rightarrow a}f(x) = f(a)\\
$$
### polynomials and rational functions are continues at every point in their domains
### types of discontinuity
removable discontinuity 左右极限存在且相等
$$
\lim_{x\rightarrow a}f(x)\neq f(a)
$$
jump discontinuity 左右极限存在且不相等
$$
\lim_{x\rightarrow a^-}f(x)\quad and\quad \lim_{a\rightarrow a^+}f(x)\neq\pm\infin\\
\lim_{x\rightarrow a^-}f(x)\neq\lim_{a\rightarrow a^+}f(x)
$$
infinite discontinuity-----located at a vertical asymptote 左右极限中至少一个不存在
$$
\lim_{x\rightarrow a^-}f(x)\quad or\quad \lim_{a\rightarrow a^+}f(x)=\pm\infin
$$
### continuous from the right and left
$$
\lim_{x\rightarrow a^-}f(x)=f(a)\\
\lim_{x\rightarrow a^+}f(x)=f(a)\\
$$
### composite function theorem
if f(x) is continuous at L and (注意这里g(x)并没有要求在a上连续):
$$
\lim_{x\rightarrow a}g(x) = L
$$
then:
$$
\lim_{x\rightarrow L}f(x)=\lim_{x\rightarrow a}f(g(x))=f(\lim_{x\rightarrow a}g(x))=f(L)
$$
### trigonometric functions are continuous over their entire domains
Proof?
### intermediate value theorem
f(x) 在闭区间[a,b]上连续，对任意z在f(a)和f(b)之间，存在c属于[a,b]，使得f(c)=z
### 一些绝对值不等式
$$
\vert x-a\vert<\epsilon\longleftrightarrow-\epsilon<x-a<\epsilon\longleftrightarrow-\epsilon+a<x<\epsilon +a\\
0<\vert x-a\vert<\epsilon\longleftrightarrow-\epsilon+a<x<\epsilon +a，x\neq a\\
\
\\
\vert a+b\vert\leq \vert a\vert+\vert b\vert\\
\vert a\vert=\vert a-b+b\vert\leq \vert a-b\vert + \vert b\vert,\vert a\vert-\vert b\vert \leq \vert a-b\vert\\
同理，\vert b\vert=\vert b-a+a\vert\leq\vert b-a\vert +\vert a\vert，\vert b\vert-\vert a\vert \leq\vert b-a\vert\\
\vert a\vert -\vert b\vert \leq \vert a-b\vert，\vert a\vert -\vert b\vert \geq -\vert a-b\vert，-\vert a-b\vert\leq \vert a\vert -\vert b\vert \leq \vert a-b\vert\\
$$
**$\vert a+b\vert\leq \vert a\vert+\vert b\vert$**
**$-\vert a-b\vert\leq \vert a\vert -\vert b\vert \leq \vert a-b\vert$**

### derivative m at x
$$
m = \lim_{h\rightarrow 0}\dfrac{f(x+h)-f(x)}{h} = \lim_{h\rightarrow 0}\dfrac{f(x-h)-f(x)}{-h} = lim_{h\rightarrow 0}\dfrac{f(x)-f(x-h)}{h}\\
\
\\
m = \lim_{x\rightarrow a}\dfrac{f(x)-f(a)}{x-a}\\
\
\\
f'(x)=\lim_{h\rightarrow o}\dfrac{f(x+h)-f(x)}{h}
$$
可以看出，如果f(x)在x=a可导必须在a上有定义
### Differentiability implies continuity
f(x) has its domain A and if f(x) is differentiable at A, then f(x) is continuous at A.
but not the other way
### several rules
suppose f(x) and g(x) is differentiable
$$
[f(x)\pm g(x)]'=f'(x)\pm g'(x)\\
[kf(x)]'=kf'(x)\\
[f(x)g(x)]'=f'(x)g(x)+f(x)g'(x)\\
\
\\
[\dfrac{f(x)}{g(x)}]'=\dfrac{f'(x)g(x)-f(x)g'(x)}{g^2(x)}
$$
### average rate of change at a
$$
R=\dfrac{f(a+h)-f(a)}{h}\\
\
\\
so \quad f(a + h)=f(a)+R(a+h-a)=f(a)+Rh
$$
for h small enough
$$
f(a + h)\approx f(a)+f'(a)h\\
f(a-h)\approx f(a)+f'(a)(-h)
$$
### derivative of trigonometric functions
$$
sin'x =cosx\\
cos'x =-sinx\\
tan'x = sec^2x\\
cot'x = -csc^2x\\
sec'x=secxtanx\\
csc'x=-cscxcotx\\
$$
### higher-order derivatives
$$
for\quad n=0,1,...\\
sin^{(4n)}x=sinx\\
sin^{(4n+1)}x=cosx\\
sin^{(4n+2)}x=-sinx\\
sin^{(4n+3)}x=-cosx\\
\
\\
cos^{(4n)}x=cosx\\
cos^{(4n+1)}x=-sinx\\
cos^{(4n+2)}x=-cosx\\
cos^{(4n+3)}x=sinx\\
$$
### exercise
$$
sin^{74}x=sin^{4*18+2}x=sin''x=-sinx
$$
### derivatives of compositions of functions
设f和g两个函数，并且g在定义域内可导，f在g的值域内可导，那么
$$
[f(g(x))]'=f'(g(x))g'(x)=\dfrac{dy}{dg}*\dfrac{dg}{dx}
$$
for more functions
$$
[f_1(f_2(f_3(...f_n(x))))]'=\dfrac{dy_1}{dy_2}\dfrac{dy_2}{dy_3}...\dfrac{dy_n}{dx}
$$
### the derivative of an inverse function
let the inverse function be
$$
y = f^{-1}(x)
$$
the derivative is
$$
(f^{-1})'(x)=\dfrac{1}{f'(y)}=\dfrac{1}{f'(f^{-1}(x))}=\dfrac{1}{{\dfrac{df}{dx}}\vert _{x=y}}
$$
这里的y，就是原函数的x

要注意的是对于函数$y=f(x)$和其反函数$y=f^{-1}(x)$，函数$y=f(x)$在$x=x_0$的导数是和其反函数$y=f^{-1}(x)$的在$x=f(x_0)$上的导数相乘等于1，而不是和其反函数$y=f^{-1}(x)$的在$x=x_0$上的导数的乘积为1，所以：
$$
\dfrac{df^{-1}}{dx}\dfrac{df}{dx}\neq 1(y\neq x)
$$

核心思想就是：
对于函数$y=f(x)$和其反函数$y=f^{-1}(x)$，$f(x)$在点$(x_0,f(x_0))$的导数和$f^{-1}(x)$在点$(f(x_0),x_0)$的导数的乘积为1.
###  the derivative of arcsinx
for $y=sin(x),x\in [-\dfrac{\pi}{2},\dfrac{\pi}{2}]$ and $y=arcsin(x)$:
$$
arcsin'x=\dfrac{1}{sin'(arcsin(x))}=\dfrac{1}{cos(arcsin(x))}=\dfrac{1}{\sqrt{1-x^2}}
$$
### derivatives of inverse trigonometric functions
$$
arcsin'(x)=\dfrac{1}{\sqrt{1-x^2}}\\
arccos'(x)=\dfrac{-1}{\sqrt{1-x^2}}\\
arctan'(x)=\dfrac{1}{1+x^2}\\
arccot'(x)=\dfrac{-1}{1+x^2}\\
arcsec'(x)=\dfrac{1}{\vert x\vert\sqrt{x^2-1}}\\
arccsc'(x)=\dfrac{-1}{\vert x\vert\sqrt{x^2-1}}\\
\
\\
arcsec'x=\dfrac{1}{sec(arcsec(x))tan(arcsec(x))}\\
\
\\
\theta=arcsec(x)\in(0,\dfrac{\pi}{2})\cup(\dfrac{\pi}{2},\pi)**此处取不到端点值\\
\theta \in(0,\dfrac{\pi}{2}),tan(arcsec(x))=\sqrt{x^2-1}\\
\theta \in(\dfrac{\pi}{2},\pi),tan(arcsec(x))=-\sqrt{x^2-1}\\
\theta=arcsec(x)\in(0,\dfrac{\pi}{2}),x=sec(\theta)>1,sec(arcsex(x))tan(arcsec(x))=x\sqrt{x^2-1}>0\\
\theta=arcsec(x)\in(\dfrac{\pi}{2},\pi),x=sec(\theta)<{-1},sec(arcsex(x))tan(arcsec(x))=-x\sqrt{x^2-1}>0\\
arcsec'x=\dfrac{1}{\vert x\vert\sqrt{x^2-1}}
$$
### implicit functions
对于方程$x^2+y^2=1$所定义的隐函数$y=f(x)$，其导数有：
$$
\dfrac{d(x^2+y^2)}{dx}=\dfrac{d(x^2)}{dx}+\dfrac{d(y^2(x))}{dx}=\dfrac{d1}{dx}\\
\
\\
2x+2y\dfrac{dy}{dx}=0\\
\dfrac{dy}{dx}=-\dfrac{x}{y}
$$
### 指数函数导数
$$
*****\dfrac{de^{x}}{dx}\vert_{x=0}=\lim_{h\rightarrow 0}\dfrac{e^h-1}{h}=1\\
\
\\
\dfrac{db^{x}}{dx}=\lim_{h\rightarrow 0}\dfrac{b^{x+h}-b^x}{h}=\lim_{h\rightarrow 0}\dfrac{b^x(b^h-1)}{h}=b^x\dfrac{db^x}{dx}\vert_{x=0}\\
\dfrac{db^x}{dx}\vert_{x=0}=\lim_{h\rightarrow 0}\dfrac{b^h-1}{h}=\lim_{h\rightarrow 0}\dfrac{e^{hlnb}-1}{h}=\lim_{hlnb\rightarrow 0}\dfrac{e^{hlnb}-1}{\dfrac{hlnb}{lnb}}=lnb\\
\
\\
(b^x)'=b^xlnb
$$
### 对数函数导数
$$
(lnx)'=\dfrac{1}{e^y}=\dfrac{1}{e^{lnx}}=\dfrac{1}{x}\\
(log_bx)'=\dfrac{1}{b^ylnb}=\dfrac{1}{xlnb}
$$
### 线性逼近法估计值
比如$\sqrt{8.01}$
线性逼近公式：当x靠近a时的线性逼近估计为
$$
L(x)=f(a)+f'(a)(x-a)
$$
### 微分中值定理与函数极值
#### extreme value theorem
连续函数闭区间有界性
if f(x) is continuous at [a,b],then there is a point $x=c_{min}$ that $f(c_{min})\leq f(x)$for all x in [a,b] and $x=c_{max}$ that $f(c_{max})\geq f(x)$ for all x in [a,b]

####  critical points and local extremum
Let c be an interior point in the domain of f . We say that c is a critical point of f if $f '(c) = 0$ or $f '(c)$ is undefined.
a local extremum must be a critical point
but not all critical points are local extremum
####  fermat's theory
If f has a local extremum at c and f is differentiable at c, then $f ′(c) = 0$.
#### 连续函数闭区间极值存在定理
闭区间连续的函数必有极值，且极值在区间端点或者区间内critical points
#### 罗尔定理
Let f be a continuous function over the closed interval [a, b] and differentiable over the open interval (a, b) such that $f (a) = f (b)$. There then exists at least one $c ∈ (a, b)$ such that $f '(c) = 0$.
运用fermat定理和连续函数闭区间极值存在定理证明罗尔定理
#### The Mean Value Theorem 
The Mean Value Theorem states that if f is continuous over the closed interval [a, b] and differentiable over the open interval (a, b), then there exists a point c ∈ (a, b) such that the tangent line to the graph of f at c is parallel to the secant line connecting$(a,f (a))$and$(b, f (b))$.
Let f be continuous over the closed interval [a, b] and differentiable over the open interval (a, b). Then, there exists at least one point c ∈ (a, b) such that
$$
f'(c)=\dfrac{f(a)-f(b)}{a-b}
$$
#### Functions with a Derivative of Zero
Let f be differentiable over an interval I. If $f '(x) = 0$ for all x ∈ I, then $f (x) = constant $ for all x ∈ I.
#### Constant Difference Theorem
If f and g are differentiable over an interval I and $f '(x) = g' (x) $for all x ∈ I, then $f (x) = g(x) + C$ for some constant C.
#### Increasing and Decreasing Functions
Let f be continuous over the closed interval [a, b] and differentiable over the open interval (a, b).
i. If $f '(x) > 0 $ for all $x ∈ (a, b)$, then f is an increasing function over [a, b].
ii. If $f '(x) < 0$ for all $x ∈ (a, b)$, then f is a decreasing function over [a, b].
#### 极值判定——一阶导数
Suppose that f is a continuous function over an interval I containing a critical point c. If f is differentiable over I, except possibly at point c, then f (c) satisfies one of the following descriptions:
i. If $f '$ changes sign from positive when $x < c$ to negative when $x > c$, then $f (c)$ is a local maximum of f .
ii. If $f '$ changes sign from negative when $x < c$ to positive when $x > c$, then $f (c)$ is a local minimum of f .
iii. If $f '$ has the same sign for $x < c$ and $x > c$, then $f (c)$ is neither a local maximum nor a local minimum of f .
#### concave
Let f be a function that is differentiable over an open interval I. If $f '$ is increasing over I, we say f is concave up over I. If $f '$ is decreasing over I, we say f is concave down over I.
#### test for concave
Let f be a function that is twice differentiable over an interval I.
i. If $f''(x) > 0 $ for all $x ∈ I$, then f is concave up over I.
ii. If $f''(x) < 0 $ for all $x ∈ I$, then f is concave down over I.
However, a continuous function can switch concavity only at a point x if $f''(x) = 0$ or $f''(x)$ is undefined. 
#### reflection point
If f is continuous at a and f changes concavity at a, the point $(a, f (a))$ is an inflection point of f .
#### 极值判定——二阶导数(包含c在内的点可导)
如果c不可导那么只能使用一阶导数判定
Suppose $f ' (c) = 0$, $f''$ is continuous over an interval containing c.
i. If $f''(c)$ > 0, then f has a local minimum at c.
ii. If $f''(c)$ < 0, then f has a local maximum at c.
iii. If $f''(c)$ = 0, then the test is inconclusive.
#### horizontal asymptote
If $\lim_{x\rightarrow \infin} f (x) = L $ or $\lim_{x\rightarrow -\infin} f (x) = L$ , we say the line $y = L$ is a horizontal asymptote of f .
#### end behavior of polynomial functions 
end behavior
1.has horizontal asymptote
2.to infinity
3.oscillate 
 Consider a polynomial function
$$
f(x)=a_nx^n + a_{n-1}x^{n-1}+...+a_0\\
f(x)=a_nx^n(\dfrac{a_{n-1}}{a_n*x}+\dfrac{a_{n-2}}{a_n*x^2}+...+\dfrac{a_0}{a_n*x^n})
$$
故
$$
\lim_{x\rightarrow \pm\infin}f(x)=a_nx^n
$$
#### 长除法
$\dfrac{p(x)}{q(x)}$, 当$p(x)$的次数高于$q(x)$时，可以写成$g(x)+\dfrac{r(x)}{q(x)}$
#### oblique asymptote
if $\lim_{x\rightarrow \pm\infin}f(x)=ax+b(a\neq 0)$, then $ ax + b$ is a oblique asymptote
### LHopital(informal $\dfrac{0}{0}$)
Suppose f and g are differentiable functions over an open interval containing a, **except possibly at a.** If $\lim_{x\rightarrow a} f (x) = 0$ and $\lim_{x\rightarrow a}  g(x) = 0$, then
考虑在a上可导的情况
$$
\lim_{x\rightarrow a}\dfrac{f(x)}{g(x)}=\lim_{x\rightarrow a}\dfrac{f(a)+f'(a)(x-a)+o(x-a)}{g(a)+g'(a)(x-a)+o(x-a)}\\
\
\\
=\lim_{x\rightarrow a}\dfrac{0+f'(a)(x-a)}{0+g'(a)(x-a)}=\dfrac{f'(a)}{g'(a)}(g'(a)\neq 0)=\lim_{x\rightarrow a}\dfrac{f'(x)}{g'(x)}
$$
从中可以看到洛必达和泰勒的关系
### LHopital(informal $\dfrac{\infin}{\infin}$)
Suppose f and g are differentiable functions over an open interval containing a, **except possibly at a.** Suppose $\lim_{x\rightarrow a}f (x) = \infin$ (or $−\infin$) and $\lim_{x\rightarrow a}g(x) = \infin$ (or $−∞$). Then
$$
\lim_{x\rightarrow a}\dfrac{f(x)}{g(x)}=\lim_{x\rightarrow a}\dfrac{\dfrac{1}{g(x)}}{\dfrac{1}{f(x)}}=\lim_{x\rightarrow a}\dfrac{g'(x)f^2(x)}{f'(x)g^2(x)}=\lim_{x\rightarrow a}\dfrac{g'(x)}{f'(x)}\lim_{x\rightarrow a}\dfrac{f^2(x)}{g^2(x)}\\
\
\\
\lim_{x\rightarrow a}\dfrac{f(x)}{g(x)}=\dfrac{\lim_{x\rightarrow a}1}{\lim_{x\rightarrow a}\dfrac{g'(x)}{f'(x)}}=\lim_{x\rightarrow a}\dfrac{f'(x)}{g'(x)},\bigg(\lim_{x\rightarrow a}\dfrac{f'(x)}{g'(x)}\neq 0\bigg)
$$
**前提条件：洛必达法则假设极限存在**
## integrals
### basic integrals
$$
\int cosxdx=sinx+C\\
\int \dfrac{1}{x}dx=ln\vert nx\vert+C\\
\int e^xdx=e^x+C\\
\int x^ndx=\dfrac{x^{n+1}}{n+1}+C\\
\int sinxdx=-cosx+C\\
\int tanxdx=ln\vert secx\vert +C\\
\int cotxdx=-ln\vert cscx\vert+C\\
\int secxdx=ln\vert secx+tanx\vert +C\\
\int cscxdx=ln\vert cscx-cotx\vert +C\\
\int sec^2xdx=tanx+C\\
\int csc^2xdx=-cotx+C\\
\int secxtanxdx=secx+C\\
\int cscxcotxdx=-cscx+C\\
\int \dfrac{1}{1+x^2}dx = arctanx+C\\
\int \dfrac{1}{\sqrt{1-x^2}}dx=arcsinx+C\\
\int \dfrac{1}{x\sqrt{x^2-1}}dx=arcsec\vert x\vert+C
$$
### several integrals
$$
\int xe^xdx=xe^x-e^x+C\\
\int xcosxdx=xsinx+cosx+C\\
\int xsinxdx=sinx - xcosx+C
$$
### partition of interval
A set of points P = {xi} for i = 0, 1, 2,…, n with $a = x0 < x1 < x2 < ⋯ < xn = b$, which divides the interval [a, b] into subintervals of the form $[x_0, x_1], [x_1, x_2],…, [x_{n − 1}, x_n]$ is called a partition of [a, b]. If the subintervals all have the same width, the set of points forms a regular partition of the interval [a, b].
### left-endpoint approx
$$
A=L_n\approx \sum_0^{n-1}f(x_i=a+\Delta x*i)\Delta x,\Delta x=\dfrac{b-a}{n}
$$
### right-endpoint approx
$$
A=R_n\approx \sum_1^{n}f(x_i=a+\Delta x*i)\Delta x,\Delta x=\dfrac{b-a}{n}
$$
### special condition
$$
a=0,b=1,\Delta x=\dfrac{1}{n}\\
L_n\approx \sum_0^{n-1}f(\dfrac{i}{n})\dfrac{1}{n}\\
R_n\approx \sum_1^{n}f(\dfrac{i}{n})\dfrac{1}{n}\\
$$
### 连续闭区间可积
if f(x) is continuous on closed interval [a,b],then A exits and is unique
it does not depend on the choice of x in $[x_{i-1},x_i]$
### 定积分
If f (x) is a function defined on an interval $[a, b]$, the definite integral of f from a to b is given by
$$
\int_a^b f(x)dx=\lim_{n\rightarrow \infin}\sum_{i=1}^nf(x_i^*)\Delta x\\
x_i^*\in [x_{i-1},x_{i}](分成n份，第0，1，2...份)
$$
**provided the limit exists**.
### 积分存在性定理
If f (x) is continuous on [a, b], then f is integrable on[a, b].
非连续函数可能仍然可积
### the requests of partition
Any partition can be used to form a Riemann sum. However, if a nonregular partition is used to define the definite integral, it is not sufficient to take the limit as the number of subintervals goes to infinity. Instead, we must take the limit **as the width of the largest subinterval goes to zero**.
要保证积分与划分无关，必须保证划分的最大子区间趋于0
否则积分与划分方法相关
### 横坐标轴下积分(signed area)
坐标轴下的积分区域面积为负号
坐标轴上的积分区域面积为正号
net-signed area = integrals above the axis - integrals below the axis
### area
曲线和坐标轴围成的面积为
$$
\int_a^b \vert f(x)\vert dx
$$
### 定积分性质
$$
\int_a^a f(x)dx=0
$$
$$
\int_a^b f(x)dx=-\int_b^a f(x)dx
$$
$$
\int_a^b[f(x)\pm g(x)]dx=\int_a^b f(x)dx\pm \int_a^b g(x)dx\\
$$
$$
\int_a^b cf(x)dx=c\int_a^b f(x)dx
$$
$$
\int_a^b f(x)dx+\int_b^c f(x)dx=\int_a^c f(x)dx
$$
### 定积分比较
if $f(x)\geq0$ for $a\leq x\leq b$
$$
\int_a^bf(x)dx\geq 0
$$
if $f(x)\geq g(x)$ for $ a\leq x\leq b$
$$
\int_a^b f(x)dx \geq\int_a^b g(x)dx
$$
if $m$ and $M$ are constant such that $m\leq f(x)\leq M$ for $a\leq x\leq b$
(连续函数闭区间有界性)
$$
m(b-a)\leq\int_a^bf(x)dx\leq M(b-a)
$$
### average value of a function
求函数在闭区间$[a,b]$上的平均值
$$
\bar A=\lim_{n\rightarrow \infin}\dfrac{\sum_i^n{f(x_i^*)}}{n}=\dfrac{1}{b-a}\int_a^bf(x)dx
$$
当a=0时
$$
\bar A=\dfrac{1}{b}\int_0^bf(x)dx
$$
当a=0,b=1时候
$$
\bar A=\int_0^1f(x)dx
$$
当b=a+h时
$$
\bar A=\dfrac{1}{h}\int_a^{a+h}f(x)dx
$$
### several conclusion
$$
\int_0^\pi sintdt=2\\
\int_0^{2\pi}sin^2tdt=\pi=\int_0^{2\pi}cos^2tdt\\
\int_0^{\dfrac{\pi}{4}}tan^2tdt=\dfrac{\pi}{4}\\
\int_0^{\dfrac{\pi}{4}}sec^2tdt=\dfrac{\pi}{2}
$$
## Fundamental theorem of calculus Part1
### the mean value theorem for integrals
积分中值定理
if f(x) is continuous over an interval [a,b], then there is at least one point $c\in [a,b]$ such that
$$
f(c)=\bar A=\dfrac{1}{b-a}\int_a^bf(x)dx
$$

### Part1
if f(x) is continuous over an interval $[a,b]$, and the function F(x) is defined by
$$
F(x)=\int_a^xf(t)dt
$$
then $F'(x)=f(x)$ over $[a,b]$.
这个定理说明F(x)是f(x)的antiderivative
$$
G(x)=\int_x^a f(t)dt=-F(x)\\
G'(x)=-f(x)
$$
常数a一定是下限
### exercise
find F'(x)
$$
F(x)=\int_0^{\sqrt{x}}f(t)dt
$$
### Part2
if f(x) is continuous over interval [a,b] and F(x) is **any antiderivative of f(x)**,then
$$
\int_a^bf(x)dx=F(b)-F(a)
$$
### Net change theorem
The new value of a changing quantity equals the initial value plus the integral of the rate of change:
$$
F(b)=F(a)+\int_a^bF'(t)dt
$$
a点的初始值为$F(a)$，到b的变化量为$\int_a^bf(t)dt$
### 分段函数的积分
如果有分段函数
$$
f(x)=
\begin{cases}
f_1(x)\quad x\leq a\\
f_2(x) \quad x>a
\end{cases}
$$
则有
$$
F(x)=
\begin{cases}
F_1(x)=\int_a^xf_1(x)dx\quad x\leq a\\
\
\\
F_2(x)=\int_a^xf_2(x)dx\quad x\geq a
\end{cases}
$$
同时需要讨论函数$F(x)$在点$x=a$上的连续性
### 被积函数的奇偶性
if $f(x)=-f(-x)$
$$
\int_a^{-a}f(x)dx=0
$$
if $f(x)=f(-x)$
$$
\int_{-a}^{a}f(x)dx=2\int_0^af(x)dx
$$
## 积分代换
Let u = g(x), where g'(x) is continuous over an interval, let f(x) be continuous over the corresponding range of g, and let F(x) be an antiderivative of f(x). Then
$$
\begin{aligned}
\int f(g(x))g'(x)dx &=\int f(u)du\\
&=F(u)+C\\
&=F(g(x))+C
\end{aligned}
$$
### several substitution
$$
**udx=\dfrac{1}{b}d(bU)**\\
\
\\
xdx =d(\dfrac{x^2}{2})\\
\
\\
x^ndx=d(\dfrac{x^{n+1}}{n+1})\\
\
\\
**\dfrac{1}{x^n}=d(\dfrac{x^{1-n}}{1-n})=\dfrac{1}{1-n}d(\dfrac{1}{x^{n-1}})**\\
\
\\
\sqrt{x}dx=d(\dfrac{2}{3}\sqrt{x^3})\\
\
\\
**\dfrac{1}{\sqrt{x}}dx=d(2\sqrt{x})**\\
$$
### exercise
$$
\int \dfrac{x}{\sqrt{x-1}}dx\\
\int(cos\theta-1)(cos^2\theta-2cos\theta)^3sin\theta d\theta\\
\
\\
\int(1-cos\theta)(cos^2\theta-2cos\theta)^3 dcos\theta=-\dfrac{1}{2}\int(cos^2\theta-2cos\theta)^3d(cos^2\theta-2cos\theta)\\
-\int(cos^2\theta-2cos\theta)^3dcos\theta
$$
### 定积分上下限代换
Let $u = g(x)$ and let g' be continuous over an interval a, b, and let f be continuous over the range of $u = g(x)$. Then
$$
\int_a^b f(g(x))g'(x)=\int_{g(a)}^{g(b)}f(u)du\\
$$
### 指数积分
$$
\int e^xdx=e^x+C\\
\int a^xdx=\dfrac{a^x}{lna}+C
$$
### 对数积分
$$
\int x^{-1}dx=ln\vert x\vert +C\\
\int lnxdx = xlnx-x+C=x(lnx-1)+C,此处x已经大于0了\\
\int log_axdx=\dfrac{x}{lna}(lnx-1)+C
$$
### exercise
$$
\int log_2xdx\\
\int ln(x)\dfrac{\sqrt{1-(ln(x)^2)}}{x}dx
$$
### 反三角函数积分
#### 带有反三角函数的积分
$$
\int \dfrac{1}{\sqrt{1-x^2}}dx=arcsin(x)+C\\
\int \dfrac{1}{1+x^2}dx=arctan(x)+C\\
\int \dfrac{1}{\vert x\vert\sqrt{x^2-1}}dx=arcsec(x)+C\\
\int \dfrac{1}{x\sqrt{x^2-1}}dx=arctan(\sqrt{x^2-1})+C\\
$$
$$
\int \dfrac{1}{\sqrt{a^2-x^2}}dx=arcsin(\dfrac{x}{a})+C\\
\int \dfrac{1}{a^2+x^2}dx=\dfrac{1}{a}arctan(\dfrac{x}{a})+C\\
\int \dfrac{1}{\vert x\vert\sqrt{x^2-a^2}}dx=\dfrac{1}{a}arcsec(\dfrac{x}{a})+C\\
\int \dfrac{1}{ x\sqrt{x^2-a^2}}dx=\dfrac{1}{a}arctan\bigg(\dfrac{\sqrt{x^2-a^2}}{a}\bigg)+C\\
$$
## 定积分应用
### 面积
if $f(x)\geq g(x)$, and integrable, then
$$
A = \int_a^b[f(x)-g(x)]dx
$$
if f(X) and g(x) go across, then
$$
A=\int_a^b\vert f(x)-g(x)\vert dx
$$
if u(y) and v(y) are integrable and $u(y)\geq v(y)$ for $y\in [c,d]$, then
$$
A=\int_c^d [u(y)-v(y)]dy
$$
### 体积
#### slice method
page 645
find an axis perpendicular to slice, the partition ${(x_0=a, x_1,...,x_n=b)}$ cut the axis region [a,b] into n section, then the volume
$$
V\approx\sum_1^nV_{[x_{i-1},x_i]}=\sum_1^nA(x^*_{[x_{i-1},x_i]})\Delta x\\
\
\\
**V=\int_a^b A(x)dx**
$$
重点：区间的划分
将面积A看成一个函数，通过定义计算得到积分公式
#### 旋转体积
绕x轴
$$
V=\int_a^b \pi f^2(x)dx
$$
绕y轴
$$
V=\int_c^d \pi u^2(y)dx
$$
空腔旋转绕x轴
$$
V=\int_a^b \pi[f^2(x)-g^2(x)]dx
$$
空腔旋转绕y轴
$$
V=\int_a^b \pi[u^2(y)-v^2(y)]dy
$$
#### cylinder shell
绕y轴，对垂直于旋转轴的区域进行划分$(x_0,x_1,...,x_n)$,有
$$
V=\sum_1^n V_{shell}=\sum_1^n \underbrace{\overbrace{2\pi x^*_{[x_{i-1},x_i]}}^{圆柱周长}f(x^*_{[x_{i-1},x_i]})}_{绕轴圆柱表面积}\Delta x\\
\
\\
V=\int_a^b 2\pi xf(x)dx
$$
绕x轴，对垂直于旋转轴的区域进行划分$(y_0,y_1,...,y_n)$,有
$$
V=\int_c^d 2\pi yg(y)dy
$$
绕$x=k$, 有
$$
V=\int_a^b 2\pi \overbrace{(x-k)}^{距离}f(x)dx
$$
### 线段长度和表面积
#### 求曲线长度不能取水平线的原因
真实曲线长度$l$与$\sqrt{\Delta x^2+\Delta y^2}$更接近，$l\geq \sqrt{\Delta x^2+\Delta y^2}$，那么考察
$$
\Delta =\lim_{\Delta x\rightarrow 0}\sqrt{\Delta x^2+\Delta y^2}-\Delta x,\Delta x>0
$$
当$\Delta y = \Delta x$时，有
$$
\Delta = \lim_{\Delta x\rightarrow 0}\sqrt{2}\Delta x-\Delta x\neq o(\Delta x)
$$
故
$$
\lim_{\Delta x\rightarrow 0}l-\Delta x\neq o(\Delta x)
$$
#### 曲线长度
**设$f(x)$连续可导，并且导数连续**
在区间$[a,b]$上的一个划分$(x_0,x_1,...,x_n)$，对每一个子区间$[x_{i-1},x_i]$，$i=1,2,...,n$，有
$$
\Delta x=x_{i}-x_{i-1}\\
\Delta y=f(x_i)-f(x_{i-1})
$$
那么曲线f(x)在[a,b]的长度为
$$
l\approx \sum_1^n \sqrt{\Delta^2 x+\Delta^2 y}\\
\sum_1^n \sqrt{\Delta^2 x+\Delta^2 y}=\sum_1^n\sqrt{1+\bigg(\dfrac{\Delta y}{\Delta x}\bigg)^2}\Delta x\\
i. f(x)可导，运用微分中值定理存在x^*_{[x_{i-1},x_i]}，有\\
f'(x^*_{[x_{i-1},x_i]})=\dfrac{\Delta y}{\Delta x}\\
\
\\
故\sum_1^n\sqrt{1+\bigg(\dfrac{\Delta y}{\Delta x}\bigg)^2}\Delta x=\sum_1^n\sqrt{1+f'^2(x^*_{[x_{i-1},x_i]})}\Delta x\\
\
\\
ii.依据积分定义，f'(x)连续就有\\
\lim_{\Delta x\rightarrow 0}\sum_1^n\sqrt{1+f'^2(x^*_{[x_{i-1},x_i]})}\Delta x=\int_a^b\sqrt{1+f'^2(x)}dx
$$
同理对于光滑的函数$x=g(y)$，有
$$
l=\int_c^d\sqrt{1+g'^2(y)}dy
$$
#### 锥体表面积
点$(0,r)$和点$(h,0)$连成的直线绕x轴旋转形成一个锥体，其底边半径为$r$，高为$h$，其表面积
$$
\begin{aligned}
A&\approx \sum_1^n2\pi(-\dfrac{r}{h}x+r)\sqrt{\Delta^2 x+\Delta^2 y}\\
A&=\int_0^h2\pi (-\dfrac{r}{h}x+r)d\sqrt{d^2x+d^2y}\\
&=\int_0^h2\pi (-\dfrac{r}{h}x+r)\bigg(\sqrt{1+(\dfrac{dx}{dy})^2}\bigg)dx\\
&=\int_0^h2\pi (-\dfrac{r}{h}x+r)\bigg(\sqrt{1+(\dfrac{r}{h})^2}\bigg)dx\\
&=\pi r \sqrt{h^2+r^r}
\end{aligned}
$$
1.为什么不是$\sum_1^n2\pi(-\dfrac{r}{h}x+r)\Delta x$
因为$2\pi(-\dfrac{r}{h}x+r)\sqrt{\Delta^2 x+\Delta^2 y}-2\pi(-\dfrac{r}{h}x+r)\Delta x\neq o(\Delta x)$
2.在区间$[x_{i-1},x_i]$内的选值有影响么
$$
\begin{aligned}
&2\pi f(x_{i})\sqrt{\Delta^2 x+\Delta^2 y}-2\pi f(x_{i-1})\sqrt{\Delta^2 x+\Delta^2 y}\\
&=2\pi\sqrt{\Delta^2 x+\Delta^2 y}\big(f(x_{i})-f(x_{i-1})\big)\\
&=2\pi\sqrt{\Delta^2 x+\Delta^2 y}\Delta y\\
&=2\pi\sqrt{1+\bigg(\dfrac{\Delta x}{\Delta y}\bigg)^2}(\Delta^2 y)\\
&=o(\Delta y)=o(\Delta x)
\end{aligned}
$$
所以和区间内取值无关
### 旋转体表面积
绕x轴，一个划分$(x_0,x_1,...,x_n)$，对每一个子区间$[x_{i-1},x_i]$，$i=1,2,...,n$，有旋转体表面积
$$
A\approx\sum_1^n2\pi f(x)\sqrt{\Delta^2 x+\Delta^2 y}\\
A=\int_a^b 2\pi f(x)\sqrt{1+f'^2(x)}dx
$$
绕y轴，$x=g(y)$，有旋转体表面积
$$
A\approx\sum_1^n2\pi g(y)\sqrt{\Delta^2 x+\Delta^2 y}=\int_c^d 2\pi g(y)\sqrt{1+g'^2(y)}dy
$$
### 质量
#### 线性质量
在$[a,b]$上进行一个划分，$(x_0,x_1,...,x_n)$，那么线性质量
$$
M\approx \sum_1^n \rho l_{[x_{i-1},x_i]}=\sum_1^n \rho(x^*)\Delta x\\
\lim_{\Delta x\rightarrow 0}\sum_1^n \rho(x)\Delta x=\int_a^b \rho(x)dx
$$
#### mass from radial density
令圆盘密度$\rho$只与半径有关，半径为r的圆盘的一个划分为$(x_0,x_1,...,x_n)$，质量为
$$
\begin{aligned}
M&\approx \sum_1^n \pi(x^2_i-x^2_{i-1}) \rho(x^*_{[x_{i-1},x_i]})\\
&=\sum_1^n \pi(x_i+x_{i-1}) \rho(x^*_{[x_{i-1},x_i]})\Delta x\\
&=\sum_1^n2\pi x_{i-1}\rho(x^*_{[x_{i-1},x_i]})\Delta x-\sum_1^n\pi\rho(x^*_{[x_{i-1},x_i]})\Delta^2 x\\
&=\sum_1^n2\pi x_{i-1}\rho(x^*_{[x_{i-1},x_i]})\Delta x+o(\Delta x)\\
\end{aligned}\\
M=\int_0^r 2\pi x\rho(x) dx
$$
### 功
力F推动物体沿着x轴从a到b，$F=F(x)$，功
$$
W=\lim_{\Delta x\rightarrow 0}\sum_1^nF(x^*)\Delta x=\int_a^b F(x)dx
$$
### 重心
$$
\bar x=\dfrac{\sum_1^n m_ix_i}{\sum_i^n m_i}=\dfrac{\sum_1^n m_ix_i}{m}
$$
物体的重心是每个质点的加权平均值
page 712
#### 平面质心
$$
\bar x=\dfrac{\sum_1^n m_ix_i}{m},\bar y=\dfrac{\sum_1^m m_iy_i}{m}
$$
page 714
对称图形的质心在对称轴上
设$y=f(x)$和$x=a,x=b$以及坐标轴x围成一个平面，密度为$\rho$，则质心为
$$
\bar x =\dfrac{\lim_{\Delta x\rightarrow 0}\sum_1^n\rho f(x^*_{[x_{i-1},x_i]})\Delta xx^*_{[x_{i-1},x_i]}}{m}=\dfrac{\int_a^b \rho f(x)xdx}{\int_a^b \rho f(x)dx}\\
\bar y =\dfrac{\lim_{\Delta x\rightarrow 0}\sum_1^n\overbrace{\rho f(x^*_{[x_{i-1},x_i]})\Delta x}^{长条质量}\overbrace{\dfrac{f(x^*_{[x_{i-1},x_i]})}{2}}^{长条的y质心}}{m}=\dfrac{\int_a^b \rho \dfrac{f^2(x)dx}{2}}{\int_a^b \rho f(x)dx}
$$
###  Theorem of Pappus for Volume
Let R be a region in the plane and let l be a line in the plane that does not intersect R. Then the volume of the solid of revolution formed by revolving R around l is equal to the area of R multiplied by the distance d traveled by the centroid of R.
旋转体体积=旋转表面积$\times$质心绕旋转轴移动一圈的距离
立方体体积=地面面积$\times$高
## 和对数有关的微分
$$
\dfrac{x}{\sqrt{x^2+a}}dx=d(\sqrt{x^2+a})\\
\dfrac{x}{\sqrt{a-x^2}}dx=d(-\sqrt{a-x^2})\\
\
**
\\
\dfrac{1}{\sqrt{1+x^2}}dx=d(ln(x+\sqrt{1+x^2}))=d(sinh^{-1}x)\\
\int \dfrac{1}{1+x^2}dx=arctan(x)+C\\
\int \dfrac{1}{\sqrt{x^2+1}}dx=ln(x+\sqrt{x^2+1})+C\\
\int \sqrt{x^2+1}dx=\dfrac{x}{2}\sqrt{x^2+1}+\dfrac{1}{2}ln(x+\sqrt{1+x^2})+C\\
\
**
\\
\dfrac{1}{1-x^2}dx=d(\dfrac{1}{2}ln\bigg(\dfrac{x+1}{x-1}\bigg))--(x\in(-\infin,-1)\cup(1,\infin))\\
\dfrac{1}{1-x^2}dx=d(\dfrac{1}{2}ln\bigg(\dfrac{x+1}{1-x}\bigg))--(x\in (-1,1))\\
\
**
\\
\int\dfrac{1}{\sqrt{x^2-1}}dx=ln\vert x+\sqrt{x^2-1}\vert+C=
\begin{cases}
cosh^{-1}x+C(x>1)\\
-cosh^{-1}(-x)+C(x<-1)
\end{cases}\\
\int \dfrac{1}{\sqrt{1-x^2}}dx=arcsin(x)+C\\
\int \sqrt{x^2-1}dx=\dfrac{x}{2}\sqrt{x^2-1}-\dfrac{1}{2}ln\vert x+\sqrt{x^2-1}\vert+C\\
\int \sqrt{1-x^2}dx=\dfrac{x}{2}\sqrt{1-x^2}+\dfrac{1}{2}arcsin(x)+C\\
\
**
\\
-\dfrac{1}{x\sqrt{1-x^2}}dx=d\bigg(ln\bigg(\dfrac{1+\sqrt{1-x^2}}{x}\bigg)\bigg)\\
\int \dfrac{1}{x\sqrt{x^2-1}}dx=arcsec\vert x\vert+C\\
\int \dfrac{1}{x\sqrt{x^2-1}}dx=arctan(\sqrt{x^2-1})+C\\
$$
## 双曲函数积分
$$
\int sinhxdx=coshx+C\\
\int coshxdx=sinhx+C\\
\int sech^2xdx=tanhx+C\\
\int csch^2xdx=-cothx+C\\
\int sechxtanhxdx=-sechx+C\\
\int cschxcothxdx=-cschx+C
$$
### 反双曲函数导数
$$
(sinh^{-1}x)'=(ln(x+\sqrt{1+x^2}))'=\dfrac{1}{\sqrt{1+x^2}}\\
(cosh^{-1}x)'=(ln(x+\sqrt{x^2-1}))'(x>1)=\dfrac{1}{\sqrt{x^2-1}}\\
(tanh^{-1}x)'=\bigg(\dfrac{1}{2}ln{\dfrac{x+1}{1-x}}\bigg)'=\dfrac{1}{1-x^2}(x\in(-1,1))\\
(coth^{-1}x)'=\bigg(\dfrac{1}{2}ln{\dfrac{x+1}{x-1}}\bigg)'=\dfrac{1}{1-x^2}(x\in(-\infin,-1)\cup(1,\infin))\\
(sech^{-1}x)'=\bigg(ln{\dfrac{1+\sqrt{1-x^2}}{x}}\bigg)'=-\dfrac{1}{x\sqrt{1-x^2}}(x>0,x<1)\\
(csch^{-1}x)'=\bigg(ln{(\dfrac{1}{x}+\dfrac{\sqrt{1+x^2}}{\vert x\vert})}\bigg)'=-\dfrac{1}{\vert x\vert\sqrt{1+x^2}}(x\neq 0)
$$