# Exercise 11 — Creating Zeros

## Problem Statement

Compute the determinant of

```math
A=\begin{pmatrix}1&2&3\\1&3&4\\1&4&6\end{pmatrix}
```

using row operations that create zeros.

## Theoretical Background and Concepts

Adding any multiple of a different row to a row preserves the determinant. After triangularization, multiply the diagonal entries.

## Detailed Step-by-Step Solution

Apply $R_2\leftarrow R_2-R_1$ (determinant unchanged):

```math
\begin{pmatrix}1&2&3\\0&1&1\\1&4&6\end{pmatrix}.
```

Apply $R_3\leftarrow R_3-R_1$ (unchanged):

```math
\begin{pmatrix}1&2&3\\0&1&1\\0&2&3\end{pmatrix}.
```

Apply $R_3\leftarrow R_3-2R_2$ (unchanged):

```math
\begin{pmatrix}1&2&3\\0&1&1\\0&0&1\end{pmatrix}.
```

Therefore $\boxed{\det A=1\cdot1\cdot1=1}$.

## Verification and Consistency Checks

A direct expansion gives $1(18-16)-2(6-4)+3(4-3)=2-4+3=1$. Every row operation used was a row replacement, with no sign or scale correction needed.
