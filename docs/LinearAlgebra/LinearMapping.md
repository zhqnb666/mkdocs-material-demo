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

## 核空间与像空间

### 1. 定义

> $\textbf{像空间}Im(\varphi)=${$\varphi(v)\mid v\in V$}    
$\textbf{核空间}Ker(\varphi)=${$v\mid \varphi(v)=0_{U}$}
