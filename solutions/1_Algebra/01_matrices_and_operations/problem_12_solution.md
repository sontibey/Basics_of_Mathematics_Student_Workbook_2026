# Exercise 12 — Formula for a Matrix Power

## Problem Statement

For

```math
A=\begin{pmatrix}1&1\\0&1\end{pmatrix}
```

compute $A^2,A^3,A^4$ and prove a formula for $A^n$ by induction.

## Theoretical Background and Concepts

Mathematical induction requires a base case and an implication from the formula at $n$ to the formula at $n+1$.

## Detailed Step-by-Step Solution

Successive multiplications give

```math
A^2=\begin{pmatrix}1&2\\0&1\end{pmatrix},\quad A^3=\begin{pmatrix}1&3\\0&1\end{pmatrix},\quad A^4=\begin{pmatrix}1&4\\0&1\end{pmatrix}.
```

Conjecture:

```math
A^n=\begin{pmatrix}1&n\\0&1\end{pmatrix}
```

for every integer $n\ge0$.

For $n=0$, this is $A^0=I$. Assume the formula for some $n\ge0$. Then

```math
A^{n+1}=A^nA=\begin{pmatrix}1&n\\0&1\end{pmatrix}\begin{pmatrix}1&1\\0&1\end{pmatrix}=\begin{pmatrix}1&n+1\\0&1\end{pmatrix}.
```

This is exactly the proposed formula at $n+1$, completing the induction.

## Verification and Consistency Checks

The formula reproduces all three computed powers. Also $A=I+N$ with $N^2=0$, so the binomial expansion independently yields $(I+N)^n=I+nN$.
