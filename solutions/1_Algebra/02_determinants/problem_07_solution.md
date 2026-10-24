# Exercise 7 — Using Determinant Properties

## Problem Statement

For a $3\times3$ matrix with $\det A=-4$, compute $\det(2A),\det(A^T),\det(A^2),\det(-A)$.

## Theoretical Background and Concepts

For an $n\times n$ matrix, $\det(cA)=c^n\det A$, $\det(A^T)=\det A$, and $\det(AB)=\det A\det B$.

## Detailed Step-by-Step Solution

1. Scaling all three rows by 2 gives $\det(2A)=2^3(-4)=\boxed{-32}$.
2. Transposition preserves determinants, so $\det(A^T)=\boxed{-4}$.
3. Multiplicativity gives $\det(A^2)=(-4)^2=\boxed{16}$.
4. Scaling all three rows by $-1$ gives $\det(-A)=(-1)^3(-4)=\boxed{4}$.

## Verification and Consistency Checks

The representative matrix $\operatorname{diag}(-4,1,1)$ has determinant $-4$. Scaling, transposing and squaring it gives diagonal products $-32,-4,16,4$, respectively, checking signs and the cubic scaling factor.
