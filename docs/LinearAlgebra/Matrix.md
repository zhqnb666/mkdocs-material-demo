# 矩阵

## 例题

>$\textbf{题目1 }$设$A$是$n\times m$矩阵，$B$是$m\times n$矩阵，$m<n$,$E$是$n$阶单位阵. 若$AB=E$，证明：$B$的列向量线性无关.

证明：记$B=(\beta_1,...,\beta_n)$, 设$x_1\beta_1+...+x_n\beta_n=0$，则
$$(\beta_1,...,\beta_n)
\begin{pmatrix}
    x_1 \\
    x_2 \\
    \vdots\\
    x_n\\
\end{pmatrix}
=B
\begin{pmatrix}
    x_1 \\
    x_2 \\
    \vdots\\
    x_n\\
\end{pmatrix}=0$$
左乘$A$得到：
$$AB
\begin{pmatrix}
    x_1 \\
    x_2 \\
    \vdots\\
    x_n\\
\end{pmatrix}=0\Longrightarrow \begin{pmatrix}
    x_1 \\
    x_2 \\
    \vdots\\
    x_n\\
\end{pmatrix}=
E\begin{pmatrix}
    x_1 \\
    x_2 \\
    \vdots\\
    x_n\\
\end{pmatrix}=
AB
\begin{pmatrix}
    x_1 \\
    x_2 \\
    \vdots\\
    x_n\\
\end{pmatrix}=0$$
于是$x_1=x_2=...=x_n=0$，故$\beta_1,...,\beta_n$线性无关.