# Exercise 14 — A System and Its Determinant

## Problem Statement

For $A=\begin{pmatrix}1&2\\k&4\end{pmatrix}$, determine when $Ax=b$ has one solution for every $b$. At the exceptional value, exhibit right-hand sides giving infinitely many solutions and no solution.

## Theoretical Background and Concepts

An invertible coefficient matrix gives exactly one solution for every right-hand side. With dependent rows, consistency requires the same dependence among the corresponding right-hand-side entries.

## Detailed Step-by-Step Solution

$$\det A=4-2k.$$
Therefore there is exactly one solution for every $b$ if and only if $\boxed{k\ne2}$.

For $k=2$, the equations are
$$x_1+2x_2=b_1,\qquad 2x_1+4x_2=b_2.$$
Subtracting twice the first from the second gives $0=b_2-2b_1$.

- Choose $b=(1,2)^T$. The second equation repeats the first, so all solutions are $(x_1,x_2)=(1-2s,s)$, $s\in\mathbb R$: infinitely many.
- Choose $b=(1,3)^T$. The equations require both $2x_1+4x_2=2$ and $2x_1+4x_2=3$, a contradiction: no solution.

## Verification and Consistency Checks

For $(1-2s,s)$, the left sides are 1 and 2 for every $s$. More generally, at $k=2$ consistency is exactly $b_2=2b_1$, giving a line of solutions; otherwise the residual equation is a contradiction.
