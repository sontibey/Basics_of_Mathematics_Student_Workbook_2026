# Exercise 3 — Swapping Two Rows

## Problem Statement

Compute the determinant of

```math
A=\begin{pmatrix}1&2&0\\0&3&1\\2&1&1\end{pmatrix}
```

Predict and calculate the determinant of $B$ obtained by swapping rows 1 and 2.

## Theoretical Background and Concepts

A single row interchange multiplies the determinant by $-1$. Cofactor expansion along the first row has signs $+,-,+$.

## Detailed Step-by-Step Solution

```math
\det A=1(3\cdot1-1\cdot1)-2(0\cdot1-1\cdot2)=2+4=6.
```

The swapped matrix is

```math
B=\begin{pmatrix}0&3&1\\1&2&0\\2&1&1\end{pmatrix}.
```

Before calculating, the row-swap rule predicts $\det B=-6$.

## Verification and Consistency Checks

Direct expansion gives $\det B=0-3(1\cdot1-0\cdot2)+1(1\cdot1-2\cdot2)=-3-3=-6$, confirming the prediction.
