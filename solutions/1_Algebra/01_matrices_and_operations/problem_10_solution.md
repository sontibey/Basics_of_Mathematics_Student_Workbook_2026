# Exercise 10 — Columns of a Product

## Problem Statement

For

```math
A=\begin{pmatrix}1&2&0\\0&1&1\end{pmatrix},\qquad
B=\begin{pmatrix}1&2\\-1&0\\3&1\end{pmatrix}=[b_1\ b_2]
```

compute $Ab_1,Ab_2,AB$ and explain their relationship.

## Theoretical Background and Concepts

The $j$th column of $AB$ is $A$ times the $j$th column of $B$, since $(AB)_{ij}=\sum_k a_{ik}b_{kj}$.

## Detailed Step-by-Step Solution

```math
Ab_1=\begin{pmatrix}1-2+0\\0-1+3\end{pmatrix}=\begin{pmatrix}-1\\2\end{pmatrix},\qquad
Ab_2=\begin{pmatrix}2+0+0\\0+0+1\end{pmatrix}=\begin{pmatrix}2\\1\end{pmatrix}.
```

Thus

```math
AB=\begin{pmatrix}-1&2\\2&1\end{pmatrix}=[Ab_1\ Ab_2].
```

Each product column uses the same column of $B$ in every row dot product, so the column identity follows entry by entry.

## Verification and Consistency Checks

For $e_1=(1,0)^T$ and $e_2=(0,1)^T$, $Be_j=b_j$ and $(AB)e_j=Ab_j$. This selects exactly the two displayed columns. Dimensions are $(2\times3)(3\times2)=2\times2$.
