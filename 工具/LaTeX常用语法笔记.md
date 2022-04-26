[TOC]



#### Markdown 中使用数学公式

输入 `$$ ` 后回车，开始输入LaTeX公式。
两个 `$` 包裹，则为行内公式。
Typora需要手动打开：文件 => 偏好设置 => Markdown , 勾选 '内联公式'，重启 Typora.



#### 数学符号

```latex
% 逻辑 
\Rightarrow 、 \Leftrightarrow 、\hat{a} 、\overline{ijk} 、\land 、\lor 、\neg 、\to 、\exists 、\forall

% 向量
\vec{c} 、\overrightarrow{ab}、 \widehat{abcd} 

% 小于等于 、大于等于 、等价 、不等于 、约等于 、恒等于
\leq 、\geq 、 \sim 、\neq 、\approx 、\equiv

% 极限 、积分
\lim_{n \to \infty}X^n 、 \int_{-N}^{N} e^x\,dx 、\iint_{D}^{W} \,dx \,dy

% 分数、根号
\frac {2}{4+5} 、 \tfrac {2}{4+5} 、\left(x+\frac{a}{b}\right) 、\sqrt[3]{9} 

% 矩阵
C^n_{r-a} 、C_{r-a}^{n-a} 

% 希腊字母
\pi 、 \Alpha  \alpha 、 \Beta  \beta 、\Delta \delta 、\Eta  \eta 、 \Phi \phi \psi \varphi 、 \Xi  \xi
```

$$
\begin{align*}

& 逻辑 & \Rightarrow 、 \Leftrightarrow 、\hat{a} 、\overline{ijk} 、\land 、\lor 、\neg 、\to 、 \exists 、\forall \\ 

& 向量 & \vec{c} 、\overrightarrow{ab}、 \widehat{abcd} \\

& 小于等于 & \leq 、\geq 、\sim 、 \neq 、\approx 、\equiv \\

& 极限、积分：&\lim_{n \to \infty}x^n 、 \int_{-N}^{N} e^x\,dx 、 \iint_{D}^{W} \,dx \,dy \\

& 分数：& \frac {2}{4+5} 、 \tfrac {2}{4+5} 、\left(x+\frac{a}{b}\right) 、\sqrt[3]{9}\\

& 矩阵：& C^n_{r-a} 、C_{r-a}^{n-a} \\

& 希腊字母：& \pi 、 \Alpha  \alpha 、 \Beta  \beta 、\Delta \delta 、\Eta  \eta 、 \Phi \phi \psi \varphi 、 \Xi  \xi \\

\end{align*}
$$







#### 矩阵

| 原码                                                         | 效果                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| \begin{matrix} x & y \\ z & v \end{matrix}                   | $\begin{matrix} x & y \\ z & v \end{matrix}$                 |
| \begin{vmatrix} x & y \\ z & v \end{vmatrix}                 | $\begin{vmatrix} x & y \\ z & v \end{vmatrix}$               |
| \begin{Vmatrix} x & y \\ z & v \end{Vmatrix}                 | $\begin{Vmatrix} x & y \\ z & v \end{Vmatrix}$               |
| \begin{bmatrix} 0 & \cdots & 0 \\ \vdots & \ddots & \vdots \\ 0 & \cdots & 0 \end{bmatrix} | $\begin{bmatrix} 0 & \cdots & 0 \\ \vdots & \ddots & \vdots \\ 0 & \cdots & 0 \end{bmatrix}$ |
| \begin{Bmatrix} x & y \\ z & v \end{Bmatrix}                 | $\begin{Bmatrix} x & y \\ z & v \end{Bmatrix}$               |
| \begin{pmatrix} x & y \\ z & v \end{pmatrix}                 | $\begin{pmatrix} x & y \\ z & v \end{pmatrix}$               |
| \dbinom {n} {r-a}                                            | $\dbinom{n}{r-a}$                                            |





#### 对齐

`&` 表示对齐的位置

```latex
% 不对齐
x = a+b+c+e \\
y = sin(x)


% 对齐
\begin{align*}
    x & = a+b+c+e \\
    y & = sin(x)
\end{align*}
```

$$
x = a+b+c+e \\
y = sin(x)
$$

$$
\begin{align*}
x & = a+b+c+e \\
y & = sin(x)
\end{align*}
$$



#### 大括号

```latex
f(x)=\left\{
	\begin{aligned}
	x & = & \cos(a) \\
	y & = & \sin(a) \\
	z & = & \frac xy
	\end{aligned}
\right.
```

$$
f(x)=\left\{
	\begin{align*}		
	x & = & \cos(a) \\
	y & = & \sin(a) \\
	z & = & \frac xy
	\end{align*}
\right.
$$

```latex
f(n) = \begin{cases} 
	n/2,  & \mbox{if }n\mbox{ is even} \\ 
	3n+1, & \mbox{if }n\mbox{ is odd} \\
	a, 	  & x>0
\end{cases}
```


$$
f(n) = \begin{cases} 
	n/2,  & \mbox{if }n\mbox{ is even} \\ 
	3n+1, & \mbox{if }n\mbox{ is odd} \\
	a, 	  & x>0
\end{cases}
$$
