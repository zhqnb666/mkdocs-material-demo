# 积分不等式

## 均值不等式推广的积分形式

均值不等式:
$$\sqrt[n]{a_1 a_2 ... a_n}\leq \frac{a_1+a_2+...+a_n}{n}$$
推广：

设$a_1,...,a_n$全为正数，$q_1+...+q_n=1$
$$a_1^{q_1}a_2^{q_2}...a_n^{q_n}\leq q_1 a_1+q_2 a_2+...+q_n a_n$$
积分形式：
$$e^{\frac{1}{b-a}\int_{a}^{b}\ln \varphi(x) dx}\leq \frac{1}{b-a}\int_{a}^{b}\varphi(x) dx$$
$\textbf{证明：}$

将区间$[a,b]$划分为$[x_0,x_1],[x_1,x_2],...,[x_{n-1},x_n]$($x_0=a,x_n=b$).

令$\Delta x_i=x_i-x_{i-1}$,取$\xi_i\in[x_{i-1},x_{i}]$则
$$\frac{\Sigma_{i=1}^n \ln\varphi(\xi_i)\Delta x_i}{\Sigma_{i=1}^{n}\Delta x_i}\leq \ln (\frac{\Sigma_{i=1}^{n}\varphi(\xi_i)\Delta x_i}{\Sigma_{i=1}^{n} \Delta x_i})$$
令$\Delta x_i\rightarrow 0$, 即有
$$\frac{\int_{a}^{b} \ln\varphi(x) dx}{\int_{a}^{b}dx}\leq \ln (\frac{\int_{a}^{b}\varphi(x)dx}{\int_{a}^{b}dx})$$

即$$e^{\frac{1}{b-a}\int_{a}^{b}\ln \varphi(x) dx}\leq \frac{1}{b-a}\int_{a}^{b}\varphi(x) dx$$

## `Jensen不等式`的积分形式

设$f(x)$在区间$[a,b]$内是凸函数，定义在$[a,b]$上的$p(x),\varphi(x)$满足$p(x)>0$,则
$$f\big (\frac{\int_{a}^{b}p(x)\varphi(x)dx}{\int_{a}^{b}p(x)dx}\big )\leq \frac{\int_{a}^{b}p(x)f(\varphi(x))dx}{\int_{a}^{b}p(x)dx}$$

**证明：**

将区间$[a,b]$划分为$[x_0,x_1],[x_1,x_2],...,[x_{n-1},x_n]$($x_0=a,x_n=b$).

令$\Delta x_i=x_i-x_{i-1}$,取$\xi_i\in[x_{i-1},x_{i}]$，则由`Jensen不等式`：
$$f\big(\frac{\Sigma_{i=1}^n p(x_i)\Delta x_i\varphi(x_i)}{\Sigma_{i=1}^n p(x_i)\Delta x_i}\big)\leq \frac{\Sigma_{i=1}^n p(x_i)\Delta x_if(\varphi(x_i))}{\Sigma_{i=1}^n p(x_i)\Delta x_i}$$

令$\Delta x_i\rightarrow 0$, 可得
$$f\big(\frac{\int_{a}^{b} p(x)\varphi(x)dx}{\int_{a}^b p(x)dx}\big)\leq \frac{\int_{a}^b p(x)f(\varphi(x))dx}{\int_{a}^b p(x)dx}$$