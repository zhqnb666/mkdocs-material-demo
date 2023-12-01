# 线性映射

## 线性映射及运算

### 概念

> $\textbf{定义4.1.1 }$设$\varphi$是数域$\mathbb{F}$上向量空间$V$到$U$的映射，若$\varphi$适合以下条件：  
(1) $\varphi(\alpha+\beta)=\varphi(\alpha)+\varphi(\beta), \alpha,\beta\in V$;  
(2) $\varphi(k\alpha)=k\varphi(\alpha),\alpha\in V, k\in\mathbb{F},$  
则称$\varphi$是向量空间$V$到$U$的线性映射.

* $V$到自身的线性映射成为$V$上的线性变换;

* $\varphi:V\rightarrow V$为线性变换;

* 若$\varphi$是单射（满射），则成为单（满）线性映射;

* 若$\varphi$是双射，则称$\varphi:V\rightarrow U$为线性同构，记为$V\cong U$.

### 运算

$\textbf{定义4.1.2}$

1. **加法**  
设$\varphi,\psi$是$\mathbb{K}$上线性空间$V\rightarrow U$的线性映射，$\varphi+\psi$为$V\rightarrow U$上的映射
$$(\varphi+\psi)(\mathbf{\alpha})=\varphi(\mathbf{\alpha})+\psi(\mathbf{\alpha})$$

2. **数乘**  
若$k\in \mathbb{K}$,则$k\varphi$为$V\rightarrow U$上的映射
$$(k\varphi)(\mathbf{\alpha})=k\varphi(\mathbf{\alpha}),\mathbf{\alpha}\in V$$

> **命题1** 设$\varphi:V\rightarrow U$为线性映射，则  
(1) $\varphi (0_{V})=0_{U}$;  
(2) $\forall \alpha, \beta\in V,k,l\in\mathbb{K}, \varphi(k\alpha+l\beta)=k\varphi(\alpha)+l\varphi(\beta)$;  
(3) 若$\varphi:V\rightarrow U$为线性同构，则$\varphi^{-1}:U\rightarrow V$也为线性同构;   
(4) 设$\varphi:V\rightarrow U,\psi:U\rightarrow W$为线性映射（同构）,   
则$\varphi\circ \psi:V\rightarrow W$为线性映射（同构）.

**证明:**  
(3) 
$\varphi$是双射$\Longrightarrow \varphi^{-1}$是双射，因此只要证$\varphi^{-1}$保持线性组合.  
任取$x,y\in U,k,l\in\mathbb{K}$, 只需$\varphi^{-1}(kx+ly)=k\varphi^{-1}(x)+l\varphi^{-1}(y)$.  
$\because \varphi(\varphi^{-1}(kx+ly)-k\varphi^{-1}(x)-l\varphi^{-1}(y))=0_{U}$  
$\therefore \varphi^{-1}(kx+ly)-k\varphi^{-1}(x)-l\varphi^{-1}(y)=0_{V}$  
于是$\varphi^{-1}(kx+ly)=k\varphi^{-1}(x)+l\varphi^{-1}(y)$.

> **推论**  
（1）线性同构是等价关系；  
（2）两个线性空间之间存在同构$\Longleftrightarrow$它们维数相同.  

**证明**  
1. 必要性  
设$\varphi:V\rightarrow U$为线性同构，任取$V$的一组基{$e_{1},...,e_{n}$},  
则{$\varphi(e_{1}),...,\varphi(e_{n})$}线性无关.  
任取$x\in U,\exists \alpha\in V, x=\varphi(\alpha)$. 设$\alpha=a_{1}e_{1}+...+a_{n}e_{n}$, 则  
$x=\varphi(\alpha)=a_{1}\varphi(e_{1})+...+a_{n}\varphi(e_{n})$  
$\therefore$ {$\varphi(e_{1}),...,\varphi(e_{n})$}是$U$的一组基，$\dim V=\dim U=n$.  
2. 充分性  
设$\dim V=\dim U=n$,$V$的基为$\{e_1,...,e_n\}$,$U$的基为$\{f_1,...,f_n\}$  
$\varphi_V:V\rightarrow \mathbb{K}^n，\alpha=\sum a_i e_i\longmapsto \begin{pmatrix}
             a_1 \\
             \vdots\\
             a_n
         \end{pmatrix}$是线性同构，  
$\varphi_U:U\rightarrow \mathbb{K}^n,\beta=\sum b_i e_i\longmapsto \begin{pmatrix}
             b_1 \\
             \vdots\\
             b_n
\end{pmatrix}$是线性同构.  
$\varphi^{-1}_U\circ\varphi_V:V\rightarrow U$为线性同构.

设$V,U$为$\mathbb{K}$上的线性空间，记$\mathscr{L}(V,U)$为$V$到$U$的线性映射全体.  
对于$\varphi,\psi\in\mathscr{L}(V,U)$  
定义加法$(\varphi+\psi)(\alpha)\xlongequal{def}\varphi(\alpha)+\psi(\alpha)$;  
定义数乘$k\in\mathbb{K},(k\varphi)(\alpha)\xlongequal{def}k\cdot\varphi(\alpha)$.  
定义复合$\psi\circ\varphi:V\rightarrow V$为乘法.

> **定理** $\mathscr{L}$在上述定义下为$\mathbb{K}$上的线性空间.

> **定义** 设$A$为数域$\mathbb{K}$上的线性空间，  
定义乘法运算 $\cdot:A\times A\rightarrow A, (a,b)\longmapsto a\cdot b$ ,若$\forall a,b,c\in A,k\in\mathbb{K}$
满足  
（1）乘法结合律：$(a\cdot b)\cdot c=a\cdot (b\cdot c)$  
（2）乘法单位元：$\exists e\in A, e\cdot a=a\cdot e=a$  
（3）乘法分配律：$a\cdot(b+c)=a\cdot b+a\cdot c,(a+b)\cdot c=a\cdot c+b\cdot c$  
（4）乘法数乘相容性：$k(a\cdot b)=(ka)\cdot(b)=a\cdot(kb)$  
则称$A$为$\mathbb{K}$上的代数.  


## 核空间与像空间

### 定义

> $\textbf{像空间}Im(\varphi)=${$\varphi(v)\mid v\in V$}    
$\textbf{核空间}Ker(\varphi)=${$v\mid \varphi(v)=0_{U}$}

