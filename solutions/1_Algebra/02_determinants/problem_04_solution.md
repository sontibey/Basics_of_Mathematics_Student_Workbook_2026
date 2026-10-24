# Exercise 4 — Triangular Matrix

## Problem Statement

Without expanding, compute the determinant of $T=\begin{pmatrix}2&4&1\\0&-3&5\\0&0&7\end{pmatrix}$ and state the general rule.

## Theoretical Background and Concepts

The determinant of any upper or lower triangular square matrix is the product of its diagonal entries.

## Detailed Step-by-Step Solution

Since all entries below the diagonal are zero,
$$\boxed{\det T=2(-3)7=-42}.$$
In general, $\det T=\prod_{i=1}^{n}t_{ii}$. In this upper triangular example, a nonzero permutation product must choose column 1 in row 1, then column 2 in row 2, then column 3 in row 3: row 3 can only use column 3, forcing row 2 to use column 2 and row 1 to use column 1. Thus only the diagonal product survives. For arbitrary size the same argument proceeds backward from the last row; for lower triangular matrices it proceeds from the first row.

## Verification and Consistency Checks

The determinant is negative because exactly one diagonal factor is negative. Every diagonal entry is nonzero, so the triangular system has a pivot in each row and the matrix is invertible, consistent with $-42\ne0$.
