# Exercise 10 — Detecting Dependence

## Problem Statement

Explain without full expansion why $\det M=0$ for

```math
M=\begin{pmatrix}1&2&3\\2&4&6\\0&1&5\end{pmatrix}
```

and relate this to noninvertibility.

## Theoretical Background and Concepts

A square matrix with linearly dependent rows has zero determinant and is not invertible. A zero row also forces determinant zero.

## Detailed Step-by-Step Solution

The rows satisfy $R_2=2R_1$, so $R_2-2R_1=0$ is a nontrivial dependence. The determinant-preserving operation $R_2\leftarrow R_2-2R_1$ produces

```math
\begin{pmatrix}1&2&3\\0&0&0\\0&1&5\end{pmatrix}.
```

Its determinant is zero, hence $\boxed{\det M=0}$ and $M$ is not invertible.

## Verification and Consistency Checks

The nonzero vector $(7,-5,1)^T$ lies in the kernel: its row dot products are $7-10+3=0$, $14-20+6=0$, and $-5+5=0$. Thus the linear map cannot have an inverse.
