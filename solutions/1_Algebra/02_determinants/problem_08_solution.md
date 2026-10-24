# Exercise 8 — Determinant of a Product

## Problem Statement

For square matrices of the same size with $\det A=3$ and $\det B=-5$, compute $\det(AB),\det(BA),\det(A^{-1}B)$ and explain equality of the first two.

## Theoretical Background and Concepts

Determinants are multiplicative; if $\det A\ne0$, then $A^{-1}$ exists and $\det(A^{-1})=1/\det A$.

## Detailed Step-by-Step Solution

$$\det(AB)=3(-5)=\boxed{-15},\qquad \det(BA)=(-5)3=\boxed{-15}.$$
Since $\det A=3\ne0$, the inverse exists and
$$\det(A^{-1}B)=\frac13(-5)=\boxed{-\frac53}.$$
The first two determinants are equal because their scalar factors commute. This does not imply that the matrix products themselves are equal.

## Verification and Consistency Checks

Multiplying $\det(A^{-1}B)$ by $\det A$ gives $3(-5/3)=-5=\det B$, consistent with $A(A^{-1}B)=B$.
