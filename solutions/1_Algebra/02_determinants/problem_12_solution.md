# Exercise 12 — A Parameter Revealed by Elimination

## Problem Statement

For

```math
A(t)=\begin{pmatrix}1&2&3\\2&4&t\\0&1&1\end{pmatrix}
```

first apply $R_2\leftarrow R_2-2R_1$ and find all singular cases.

## Theoretical Background and Concepts

Row replacement preserves the determinant. A square matrix is singular exactly when its determinant vanishes.

## Detailed Step-by-Step Solution

The prescribed operation gives

```math
\begin{pmatrix}1&2&3\\0&0&t-6\\0&1&1\end{pmatrix}.
```

Expansion along column 1 leaves

```math
\det A(t)=\det\begin{pmatrix}0&t-6\\1&1\end{pmatrix}=0-(t-6)=6-t.
```

Consequently $\boxed{t=6}$ is the only singular value. At $t=6$, the original second row is exactly twice the first row; after the operation, it becomes a zero row.

## Verification and Consistency Checks

For $t\ne6$, swapping the last two transformed rows yields an upper triangular matrix with diagonal $(1,1,t-6)$ and determinant $t-6$. Undoing the single swap changes the sign, giving $6-t$ as above.
