# Exercise 13 — Determinant by Elimination

## Problem Statement

Compute $\det A$ for

```math
A=\begin{pmatrix}1&2&3\\2&5&7\\1&0&2\end{pmatrix}
```

by elimination, recording each determinant effect.

## Theoretical Background and Concepts

Row replacement leaves the determinant unchanged. For triangular matrices the determinant is the product of the diagonal entries.

## Detailed Step-by-Step Solution

Apply $R_2\leftarrow R_2-2R_1$ (no change):

```math
\begin{pmatrix}1&2&3\\0&1&1\\1&0&2\end{pmatrix}.
```

Apply $R_3\leftarrow R_3-R_1$ (no change):

```math
\begin{pmatrix}1&2&3\\0&1&1\\0&-2&-1\end{pmatrix}.
```

Apply $R_3\leftarrow R_3+2R_2$ (no change):

```math
\begin{pmatrix}1&2&3\\0&1&1\\0&0&1\end{pmatrix}.
```

Thus $\boxed{\det A=1}$, with no sign or scale adjustments.

## Verification and Consistency Checks

Reversing the replacements reconstructs the original matrix: subtract twice row 2 from row 3, add row 1 to row 3, then add twice row 1 to row 2. Each reverse step also preserves the determinant. The three nonzero pivots confirm invertibility.
