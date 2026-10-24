# Exercise 2 — Sarrus’ Rule

## Problem Statement

Compute $\det A$ for

```math
A=\begin{pmatrix}1&2&-1\\0&3&4\\2&1&5\end{pmatrix}
```

using Sarrus’ rule and check with a determinant property.

## Theoretical Background and Concepts

For a $3\times3$ matrix, Sarrus’ rule adds the three downward diagonal products and subtracts the three upward diagonal products. Adding a multiple of one row to another preserves the determinant.

## Detailed Step-by-Step Solution

The downward products sum to

```math
1\cdot3\cdot5+2\cdot4\cdot2+(-1)\cdot0\cdot1=15+16+0=31.
```

The upward products sum to

```math
(-1)\cdot3\cdot2+2\cdot0\cdot5+1\cdot4\cdot1=-6+0+4=-2.
```

Thus $\boxed{\det A=31-(-2)=33}$.

## Verification and Consistency Checks

Use $R_3\leftarrow R_3-2R_1$ without changing the determinant. The last row becomes $(0,-3,7)$, so expansion along the first column gives

```math
1\det\begin{pmatrix}3&4\\-3&7\end{pmatrix}=21+12=33.
```
