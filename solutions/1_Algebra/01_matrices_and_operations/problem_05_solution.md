# Exercise 5 — Matrix Times Vector

## Problem Statement

For

```math
A=\begin{pmatrix}2&-1\\1&3\end{pmatrix}
```

and $x=(4,2)^T$, compute $Ax$ and express it using columns.

## Theoretical Background and Concepts

If $A=[a_1\ a_2]$, then $Ax=x_1a_1+x_2a_2$.

## Detailed Step-by-Step Solution

```math
Ax=\begin{pmatrix}2\cdot4-1\cdot2\\1\cdot4+3\cdot2\end{pmatrix}=\begin{pmatrix}6\\10\end{pmatrix}.
```

The columns are $a_1=(2,1)^T$, $a_2=(-1,3)^T$, hence

```math
Ax=4\begin{pmatrix}2\\1\end{pmatrix}+2\begin{pmatrix}-1\\3\end{pmatrix}.
```

## Verification and Consistency Checks

The column calculation gives $(8,4)^T+(-2,6)^T=(6,10)^T$, agreeing with both row dot products. The result has size $2\times1$.
