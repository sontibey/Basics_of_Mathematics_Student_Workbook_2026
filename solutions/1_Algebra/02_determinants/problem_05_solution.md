# Exercise 5 — Row Operations

## Problem Statement

Find $\det A$ for $A=\begin{pmatrix}1&2&3\\2&1&0\\-1&4&2\end{pmatrix}$ by row operations, recording their effects.

## Theoretical Background and Concepts

Replacing a row by itself plus a multiple of a different row leaves the determinant unchanged. A triangular determinant is the product of its diagonal entries.

## Detailed Step-by-Step Solution

Apply $R_2\leftarrow R_2-2R_1$ (no change):
$$\begin{pmatrix}1&2&3\\0&-3&-6\\-1&4&2\end{pmatrix}.$$
Apply $R_3\leftarrow R_3+R_1$ (no change):
$$\begin{pmatrix}1&2&3\\0&-3&-6\\0&6&5\end{pmatrix}.$$
Apply $R_3\leftarrow R_3+2R_2$ (no change):
$$\begin{pmatrix}1&2&3\\0&-3&-6\\0&0&-7\end{pmatrix}.$$
No swaps or row scalings occurred, so $\boxed{\det A=1(-3)(-7)=21}$.

## Verification and Consistency Checks

First-row cofactor expansion independently gives $1(2)-2(4)+3(8+1)=2-8+27=21$.
