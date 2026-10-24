# Exercise 15 — Combining Determinant Properties

## Problem Statement

For invertible $2\times2$ matrices with $\det A=-2$, $\det B=3$, compute $\det(B^{-1}A^TB)$ without finding matrix entries.

## Theoretical Background and Concepts

Use multiplicativity for the three-factor product, then the inverse determinant rule and invariance under transpose.

## Detailed Step-by-Step Solution

First separate the factors:
$$\det(B^{-1}A^TB)=\det(B^{-1})\det(A^T)\det B.$$
Since $B$ is invertible, $\det(B^{-1})=1/\det B=1/3$. Transposition gives $\det(A^T)=\det A=-2$. Hence
$$\det(B^{-1}A^TB)=\frac13(-2)3=\boxed{-2}.$$
The factors involving $B$ cancel because they are reciprocal nonzero scalar determinants: $(\det B)^{-1}\det B=1$. No commutativity of the matrices is assumed.

## Verification and Consistency Checks

The expression $B^{-1}A^TB$ is similar to $A^T$. Similarity preserves determinants, agreeing with $\det(A^T)=\det A=-2$. The result is nonzero, consistent with a product of invertible matrices.
