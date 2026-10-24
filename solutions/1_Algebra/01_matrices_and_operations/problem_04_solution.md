# Exercise 4 — Noncommutativity

## Problem Statement

Compute $AB$ and $BA$ for

```math
A=\begin{pmatrix}1&2\\0&1\end{pmatrix},\qquad
B=\begin{pmatrix}2&0\\3&1\end{pmatrix}.
```

## Theoretical Background and Concepts

The entry $(AB)_{ij}$ is the dot product of row $i$ of $A$ and column $j$ of $B$. Commutativity would require $AB=BA$.

## Detailed Step-by-Step Solution

```math
AB=\begin{pmatrix}1\cdot2+2\cdot3&1\cdot0+2\cdot1\\0\cdot2+1\cdot3&0\cdot0+1\cdot1\end{pmatrix}=\begin{pmatrix}8&2\\3&1\end{pmatrix}.
```

```math
BA=\begin{pmatrix}2\cdot1+0\cdot0&2\cdot2+0\cdot1\\3\cdot1+1\cdot0&3\cdot2+1\cdot1\end{pmatrix}=\begin{pmatrix}2&4\\3&7\end{pmatrix}.
```

Thus $AB\ne BA$: changing factor order can change the product.

## Verification and Consistency Checks

For $e_1=(1,0)^T$, $A(Be_1)=(8,3)^T$ whereas $B(Ae_1)=(2,3)^T$. The different actions independently demonstrate noncommutativity.
