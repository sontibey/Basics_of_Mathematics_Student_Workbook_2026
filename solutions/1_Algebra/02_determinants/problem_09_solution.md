# Exercise 9 — Area and Orientation

## Problem Statement

Find the area of the parallelogram spanned by $u=(3,1)^T$, $v=(1,4)^T$ and explain the effect of reversing their order.

## Theoretical Background and Concepts

The signed area is $\det[u\ v]$. The geometric area is its absolute value. Swapping columns reverses the determinant sign.

## Detailed Step-by-Step Solution

```math
\det[u\ v]=\det\begin{pmatrix}3&1\\1&4\end{pmatrix}=3\cdot4-1\cdot1=11.
```

Therefore the area is $\boxed{11}$ square units.

Reversing the order gives

```math
\det[v\ u]=\det\begin{pmatrix}1&3\\4&1\end{pmatrix}=1-12=-11.
```

The orientation reverses, but the geometric area remains $|-11|=11$.

## Verification and Consistency Checks

The Gram formula gives area squared $\|u\|^2\|v\|^2-(u\cdot v)^2=10\cdot17-7^2=121$. Its positive square root is 11, independently confirming the area.
