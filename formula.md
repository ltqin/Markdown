## 1. 基本语法  
### 1.1  行内公式
+ 正文(inline)中的LaTeX公式用$...$定义  
+ 语句为\$\sum_{i=0}^N\int_{a}^{b}g(t,i)\text{d}t$
+ 这是行内公式: $\sum_{i=0}^N\int_{a}^{b}g(t,i)\text{d}t$
### 1.2 行间公式  
+ 单独显示(display)的LaTeX公式用\$$...\$$定义，此时公式居中并放大显示
+ 语句为\$$\sum_{i=0}^N\int_{a}^{b}g(t,i)\text{d}t$$
+ 这是行间公式:
$$\sum_{i=0}^N\int_{a}^{b}g(t,i)\text{d}t$$
## 2. 希腊字母
|显示|	命令|	显示|	命令|
| :----| :----| :---- | :---- |
|α|	\alpha|β|\beta|
|γ|	\gamma|δ|\delta|
|ε|	\epsilon|ζ|\zeta|
|η|	\eta|θ|\theta|
|ι|	\iota|κ|\kappa|
|λ|	\lambda|μ|\mu|
|ν|	\nu|ξ|\xi|
|π|	\pi|ρ|\rho|
|σ|	\sigma|τ|\tau|
|υ|	\upsilon|φ|	\phi|
|χ|	\chi|ψ|\psi|
|ω|	\omega|


+ 若需要大写希腊字母，将命令首字母大写即可。  
\Gamma $\Gamma$
+ 若需要斜体希腊字母，将命令前加上var前缀即可。  
\varGamma $\varGamma$
## 3. 字母修饰
### 3.1 上下标
+ 上标：^
+ 下标：_
+ 举例: C_n^2 或C^2_n 显示为 $C_n^2$ $C^2_n$
### 3.2 矢量
+ \vec a 显示为: $\vec a$
+ \overrightarrow{xy} 显示为: $\overrightarrow{xy}$
### 3.3 字体
+ Typewriter:  \mathtt{A} 显示为 $\mathtt{A}$  
$\mathtt{A}\mathtt{B}\mathtt{C}\mathtt{D}\mathtt{E}\mathtt{F}\mathtt{G}\mathtt{H}\mathtt{I}\mathtt{J}\mathtt{K}\mathtt{L}\mathtt{M}\mathtt{N}\mathtt{O}\mathtt{P}\mathtt{Q}\mathtt{R}\mathtt{S}\mathtt{T}\mathtt{U}\mathtt{V}\mathtt{W}\mathtt{X}\mathtt{Y}\mathtt{Z}$
+ Blackboard Bold: \mathbb{A} 显示为 $\mathbb{A}$  
$\mathbb{A}\mathbb{B}\mathbb{C}\mathbb{D}\mathbb{E}\mathbb{F}\mathbb{G}\mathbb{H}\mathbb{I}\mathbb{J}\mathbb{K}\mathbb{L}\mathbb{M}\mathbb{N}\mathbb{O}\mathbb{P}\mathbb{Q}\mathbb{R}\mathbb{S}\mathbb{T}\mathbb{U}\mathbb{V}\mathbb{W}\mathbb{X}\mathbb{Y}\mathbb{Z}$
+ Sans Serif: \mathsf{A} 显示为 $\mathsf{A}$  
$\mathsf{A}\mathsf{B}\mathsf{C}\mathsf{D}\mathsf{E}\mathsf{F}\mathsf{G}\mathsf{H}\mathsf{I}\mathsf{J}\mathsf{K}\mathsf{L}\mathsf{M}\mathsf{N}\mathsf{O}\mathsf{P}\mathsf{Q}\mathsf{R}\mathsf{S}\mathsf{T}\mathsf{U}\mathsf{V}\mathsf{W}\mathsf{X}\mathsf{Y}\mathsf{Z}$

### 3.4 分组
+ 使用{}将具有相同等级的内容扩入其中，成组处理
+ 举例: 10^{10} 呈现为 $10^{10}$，而 10^10 显示为 $10^10$

### 3.5 括号和分隔符
+ ()、[]和|表示符号本身。
+ 当要显示大号的括号或分隔符时，要用 \left 和 \right 命令。 使括号大小和邻近的公式相适应，适应于所有括号。
+ (\frac{x}{y}) 显示为 $$(\frac{x}{y})$$
+ \left(\frac{x}{y}\right) 显示为 $$\left(\frac{x}{y}\right)$$

+ 一些特殊的括号：  
> | 命令 | 说明 | 输入 | 显示 |
> | :----| :----:| :---- | :----: |
> | \langle \rangle |  尖括号  | \langle a+b \rangle | $\langle a+b \rangle$| 
> | \lceil \rceil   |上方括号  | \lceil a+b \rceil   | $\lceil a+b \rceil$  |  
> |\lfloor \rfloor	|下方括号  |\lfloor a+b \rfloor	 | $\lfloor a+b \rfloor$|
> |\lbrace \rbrace	|大括号	  |\lbrace a+b \rbrace   |$\lbrace a+b \rbrace$|
> |\overline	    |连线符号  |\overline{a+b+c+d}	 |$\overline{a+b+c+d}$|
> |\underline       |下划线    |\underline{a+b+c+d}  |$\underline{a+b+c+d}$|	
> |\overbrace       |上大括号  |\overbrace{a+\underbrace{b+c}_{1.0}+d}^{2.0}|$\overbrace{a+\underbrace{b+c}_{1.0}+d}^{2.0}$|	
> |\underbrace      |下大括号  |\underbrace{a+d}_3   |$\underbrace{a+d}_3$|	

### 3.6 空格
+ Latex语法本身会忽略空格的存在。
+ 小空格: a\ b 显示为 $a\ b$
+ 大空格: a \quad b 显示为 $a \quad b$

## 4. 数学公式
### 4.1 初等运算
|命令|	说明|	输入|	显示|
| :----| :----:| :---- | :----: | 
|  =   |  等于  |   x=y | $x=y$  |	
|  +   |  加   |   x+y  | $x+y$  |	
|  -   |  减   |   x−y	| $x-y$ |
| \ast |  乘   |x \ast y|$x \ast y$|	
| \div |  除   |x \div y|$x \div y$|	
|\pm   | 加减  | x \pm y |$x \pm y$|	
|\mp   | 减加  |x \mp y	|$x \mp y$|
|\times| 叉积  |x \times y|$x \times y$|	
|\cdot |点积(内积)|x \cdot y|$x \cdot y$|	
|^     |幂     |x^a|$x^a$|	
|^     |  指数 |a^x|$a^x$|	
|\log  |  对数 |\log_ax|$\log_ax$|	
|\ln   |自然对数(e为底)|\ln x|$\ln x$|	
|\lg|10为底对数|\lg x|$\lg x$|	
|\frac|分式|\frac{x}{y}|$\frac{x}{y}$|	
|\sqrt|二次开方根式|\sqrt{x}|$\sqrt{x}$|	
|\sqrt|根式|\sqrt[n]{x}|$\sqrt[n]{x}$|	
|\sqrt|常数二次开方根式|\sqrt{a}|$\sqrt{a}$|
|\sqrt|常数根式|\sqrt[n]{a}|$\sqrt[n]{a}$|	
||多项式|a_nx^n + \cdots + a_1x + a_0 \quad n \geq 0|$a_nx^n + \cdots + a_1x + a_0$|	

### 4.2 比较运算
|命令|	说明|	输入|	显示|
| :----| :----| :---- | :----: | 
|\leq|	小于等于|	x \leq y|$x \leq y$|	
|\geq|	大于等于|	x \geq y|$x \geq y$|	
|\nleq|	不小于等于|	x \nleq y|$x \nleq y$|	
|\not \leq|	不小于等于|	x \not \leq y|$x \not \leq y$|	
|\ngeq|	不大于等于|	x \ngeq y|$x \ngeq y$|	
|\not \geq|	不大于等于|	x \not \geq y|$x \not \geq y$|	
|\neq|	不等于|	x \neq y|$x \neq y$|	
|\approx|	约等于|	x \approx y|$x \approx y$|	
|\equiv|	恒等于|	x \equiv y|$x \equiv y$|	

### 4.3 集合运算
|命令|	说明|	输入|	显示|
| :----| :----| :---- | :----: |
|\in|	属于|	x \in y|$x \in y$|
|\notin|	不属于|	x \notin y	|$x \notin y$|
|\subset|	真子集|	x \subset y	|$x \subset y$|
|\not \subset|	非子集|	x \not \subset y|$x \not \subset y$|
|\subseteq|	子集|	x \subseteq y|$x \subseteq y$|
|\supset|	真超集|	x \supset y	|$x \supset y$|
|\supseteq|	超集|	x \supseteq y|$x \supseteq y$|
|\cup|	并集|	x \cup y|	$x \cup y$|
|\cap|	交集|	x \cap y	|$x \cap y$|
|\setminus|	差集|	x \setminus y|$x \setminus y$|
|\emptyset|	空集合|	\emptyset|$\emptyset$|
### 4.4 三角函数
|命令|	说明|	输入|	显示|
| :----| :----| :---- | :----: |
|\sin|	正弦|	\sin x|$\sin x$|
|\cos|	余弦|	\cos x|$\cos x$|
|\tan|	正切|	\tan x|$\tan x$|
|\cot|	余切|	\cot x|$\cot x$|
|\sec|	正割|	\sec x|$\sec x$|
|\csc|	余割|	\csc x|$\csc x$|

### 4.5 累加与累乘
+ 累加求和: \sum_{i=0}^{n}{a_i}
$$\sum_{i=0}^{n}{a_i}$$
+ 累乘求积: \prod_{i=0}^{n}{a_i} 
$$\prod_{i=0}^{n}{a_i}$$
+ 累计并集: \bigcup_{i=0}^{n}{A_i} 
$$\bigcup_{i=0}^{n}{A_i}$$
+ 累计交集: \bigcap_{i=0}^{n}{A_i} 
$$\bigcap_{i=0}^{n}{A_i}$$
### 4.6 数学分析
|命令|	说明|	输入|	显示|
| :----| :----| :---- | :----: |
|\lim|极限|\lim_{0 \to \infty}|$\lim_{0 \to \infty}$|
|\Delta|微变量|\Delta x|$\Delta x$|	
|\mathrm{d}|微分算子|\mathrm{d}{x}|$\mathrm{d}{x}$|
|\partial|	偏微分算子|	\partial{x}|$\partial{x}$|
|\int|	一重积分|\int_{a}{b}|$\int_{a}{b}$|
|\iint|	二重积分|\iint_{D}{f(x, y)}\mathrm{d}{\delta}|$\iint_{D}{f(x, y)}\mathrm{d}{\delta}$|
|\iiint|三重积分||$\iiint$|
|\oint|	一重曲线积分|\oint_{L}{P\mathrm{d}x+Q\mathrm{d}y}|$\oint_{L}{P\mathrm{d}x+Q\mathrm{d}y}$|
|\oiint|二重曲线积分||$\oiint$|
|\oiiint|三重曲线积分||$\oiiint$|	


## 5. 矩阵
### 5.1 基本语法
+ 起始标记\begin{matrix}，结束标记\end{matrix}
+ 每一行末尾标记\\，行间元素之间以&分隔
+ 举例:

\$$  
\begin{matrix}  
1&0&0\\\  
0&1&0\\\  
0&0&1\\\  
\end{matrix}  
\$$  
#### 呈现为：
$$
\begin{matrix}
1&0&0\\
0&1&0\\
0&0&1\\
\end{matrix}
$$

### 5.2 矩阵边框
+ 在起始、结束标记处用下列词替换 matrix
+ pmatrix ：小括号边框
$$
\begin{pmatrix}
1&0&0\\
0&1&0\\
0&0&1\\
\end{pmatrix}
$$
+ bmatrix ：中括号边框
$$
\begin{bmatrix}
1&0&0\\
0&1&0\\
0&0&1\\
\end{bmatrix}
$$
+ Bmatrix ：大括号边框
$$
\begin{Bmatrix}
1&0&0\\
0&1&0\\
0&0&1\\
\end{Bmatrix}
$$
+ vmatrix ：单竖线边框
$$
\begin{vmatrix}
1&0&0\\
0&1&0\\
0&0&1\\
\end{vmatrix}
$$
+ Vmatrix ：双竖线边框
$$
\begin{Vmatrix}
1&0&0\\
0&1&0\\
0&0&1\\
\end{Vmatrix}
$$

### 5.3 省略元素
+ 横省略号：\cdots
+ 竖省略号：\vdots
+ 斜省略号：\ddots
+ 底省略号: \ldots 效果显示为 $1,2,\ldots,n$
#### 举例:
\$$  
\begin{bmatrix}  
{a_{11}}&{a_{12}}&{\cdots}&{a_{1n}}\\\  
{a_{21}}&{a_{22}}&{\cdots}&{a_{2n}}\\\  
{\vdots}&{\vdots}&{\ddots}&{\vdots}\\\  
{a_{m1}}&{a_{m2}}&{\cdots}&{a_{mn}}\\\  
\end{bmatrix}  
\$$
#### 呈现为：
$$
\begin{bmatrix}
{a_{11}}&{a_{12}}&{\cdots}&{a_{1n}}\\
{a_{21}}&{a_{22}}&{\cdots}&{a_{2n}}\\
{\vdots}&{\vdots}&{\ddots}&{\vdots}\\
{a_{m1}}&{a_{m2}}&{\cdots}&{a_{mn}}\\
\end{bmatrix}
$$

### 5.4 阵列
+ 需要array环境: 起始、结束处以{array}声明
+ 对齐方式: 在{array}后以{}逐行统一声明
+ 左对齐: l 居中: c 右对齐: r
+ 竖直线: 在声明对齐方式时，插入|建立竖直线
+ 插入水平线: \hline
#### 举例:
\$$  
\begin{array}{c|lll}  
{↓}&{a}&{b}&{c}\\\  
\hline  
{R_1}&{c}&{b}&{a}\\\  
{R_2}&{b}&{c}&{c}\\\  
\end{array}  
\$$
#### 呈现为:
$$
\begin{array}{c|lll}
{↓}&{a}&{b}&{c}\\
\hline
{R_1}&{c}&{b}&{a}\\
{R_2}&{b}&{c}&{c}\\
\end{array}
$$

### 5.5 方程组
+ 需要cases环境：起始、结束处以{cases}声明
+ 举例:
\$$  
\begin{cases}  
a_1x+b_1y+c_1z=d_1\\\  
a_2x+b_2y+c_2z=d_2\\\  
a_3x+b_3y+c_3z=d_3\\\  
\end{cases}  
\$$  
#### 呈现为:
$$
\begin{cases}
a_1x+b_1y+c_1z=d_1\\
a_2x+b_2y+c_2z=d_2\\
a_3x+b_3y+c_3z=d_3\\
\end{cases}
$$


### 参考：
1. [Markdown-常用数学公式编辑命令](http://events.jianshu.io/p/8b6fc36035c0)