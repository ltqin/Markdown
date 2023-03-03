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
<table>
<thead><tr>
<th style="text-align:center">显示</th>
<th style="text-align:center">命令</th>
<th style="text-align:center">显示</th>
<th style="text-align:center">命令</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center">α</td>
<td style="text-align:center"><code>\alpha</code></td>
<td style="text-align:center">β</td>
<td style="text-align:center"><code>\beta</code></td>
</tr>
<tr>
<td style="text-align:center">γ</td>
<td style="text-align:center"><code>\gamma</code></td>
<td style="text-align:center">δ</td>
<td style="text-align:center"><code>\delta</code></td>
</tr>
<tr>
<td style="text-align:center">ε</td>
<td style="text-align:center"><code>\epsilon</code></td>
<td style="text-align:center">ζ</td>
<td style="text-align:center"><code>\zeta</code></td>
</tr>
<tr>
<td style="text-align:center">η</td>
<td style="text-align:center"><code>\eta</code></td>
<td style="text-align:center">θ</td>
<td style="text-align:center"><code>\theta</code></td>
</tr>
<tr>
<td style="text-align:center">ι</td>
<td style="text-align:center"><code>\iota</code></td>
<td style="text-align:center">κ</td>
<td style="text-align:center"><code>\kappa</code></td>
</tr>
<tr>
<td style="text-align:center">λ</td>
<td style="text-align:center"><code>\lambda</code></td>
<td style="text-align:center">μ</td>
<td style="text-align:center"><code>\mu</code></td>
</tr>
<tr>
<td style="text-align:center">ν</td>
<td style="text-align:center"><code>\nu</code></td>
<td style="text-align:center">ξ</td>
<td style="text-align:center"><code>\xi</code></td>
</tr>
<tr>
<td style="text-align:center">π</td>
<td style="text-align:center"><code>\pi</code></td>
<td style="text-align:center">ρ</td>
<td style="text-align:center"><code>\rho</code></td>
</tr>
<tr>
<td style="text-align:center">σ</td>
<td style="text-align:center"><code>\sigma</code></td>
<td style="text-align:center">τ</td>
<td style="text-align:center"><code>\tau</code></td>
</tr>
<tr>
<td style="text-align:center">υ</td>
<td style="text-align:center"><code>\upsilon</code></td>
<td style="text-align:center">φ</td>
<td style="text-align:center"><code>\phi</code></td>
</tr>
<tr>
<td style="text-align:center">χ</td>
<td style="text-align:center"><code>\chi</code></td>
<td style="text-align:center">ψ</td>
<td style="text-align:center"><code>\psi</code></td>
</tr>
<tr>
<td style="text-align:center">ω</td>
<td style="text-align:center"><code>\omega</code></td>
</tr>
</tbody>
</table>

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







### 参考：
1. http://events.jianshu.io/p/8b6fc36035c0