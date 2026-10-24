# Exercise 11 — When Do Matrices Commute?

## Problem Statement

Find all

```math
B=\begin{pmatrix}a&b\\c&d\end{pmatrix}
```

commuting with

```math
A=\begin{pmatrix}1&1\\0&1\end{pmatrix}.
```

## Theoretical Background and Concepts

Two matrices are equal precisely when their corresponding entries are equal. This turns $AB=BA$ into scalar equations.

## Detailed Step-by-Step Solution

```math
AB=\begin{pmatrix}a+c&b+d\\c&d\end{pmatrix},\qquad BA=\begin{pmatrix}a&a+b\\c&c+d\end{pmatrix}.
```

Comparing entries gives $c=0$ from the top left, $d=a$ from the top right, the identity $c=c$ from the bottom left, and again $c=0$ from the bottom right.
Therefore

```math
\boxed{B=\begin{pmatrix}a&b\\0&a\end{pmatrix},\quad a,b\in\mathbb R.}
```

There are no further restrictions on $a$ or $b$.

## Verification and Consistency Checks

Substitution gives

```math
AB=BA=\begin{pmatrix}a&a+b\\0&a\end{pmatrix}
```

for every such $B$, proving sufficiency as well as necessity.
