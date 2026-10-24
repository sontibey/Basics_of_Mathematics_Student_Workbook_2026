# Exercise 1 — Determinant of a 2×2 Matrix

## Problem Statement

Compute the determinants of $A=\begin{pmatrix}3&-2\\5&4\end{pmatrix}$ and $B=\begin{pmatrix}1&7\\2&14\end{pmatrix}$, and determine invertibility.

## Theoretical Background and Concepts

For $M=\begin{pmatrix}a&b\\c&d\end{pmatrix}$, $\det M=ad-bc$. A square matrix is invertible exactly when its determinant is nonzero.

## Detailed Step-by-Step Solution

$$\det A=3\cdot4-(-2)\cdot5=12+10=22,$$
$$\det B=1\cdot14-7\cdot2=14-14=0.$$
Therefore $A$ is invertible and $B$ is not.

## Verification and Consistency Checks

The second row of $B$ is twice its first, confirming dependence. For $A$, the inverse is $\frac1{22}\begin{pmatrix}4&2\\-5&3\end{pmatrix}$; multiplying $A$ by its numerator gives $22I$.
