# Exercise 8 — Reversible Row Operations

## Problem Statement

Start with

```math
A=\begin{pmatrix}1&2&-1\\2&4&1\\-1&1&3\end{pmatrix}
```

Apply $R_2\leftarrow R_2-2R_1$, then $R_3\leftarrow R_3+R_1$, then swap $R_2,R_3$. State the inverses.

## Theoretical Background and Concepts

Adding a multiple of another row is undone by adding its negative. A row swap is its own inverse.

## Detailed Step-by-Step Solution

After the first operation,

```math
A_1=\begin{pmatrix}1&2&-1\\0&0&3\\-1&1&3\end{pmatrix}.
```

After the second operation,

```math
A_2=\begin{pmatrix}1&2&-1\\0&0&3\\0&3&2\end{pmatrix}.
```

After the swap,

```math
A_3=\begin{pmatrix}1&2&-1\\0&3&2\\0&0&3\end{pmatrix}.
```

The respective inverse operations are $R_2\leftarrow R_2+2R_1$, $R_3\leftarrow R_3-R_1$, and swapping $R_2,R_3$.

## Verification and Consistency Checks

To undo the whole sequence, reverse the order: swap rows 2 and 3 to recover $A_2$, subtract row 1 from row 3 to recover $A_1$, then add twice row 1 to row 2 to recover $A$.
