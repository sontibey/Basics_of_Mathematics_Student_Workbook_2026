# Exercise 7 — Identity, Zero, and Powers

## Problem Statement

For $A=\begin{pmatrix}2&1\\0&2\end{pmatrix}$, compute $AI,IA,A+0,A^2,A^3$ and describe the power pattern.

## Theoretical Background and Concepts

$I=I_2$ is the multiplicative identity; the $2\times2$ zero matrix is the additive identity. Write $A=2I+N$, where $N=\begin{pmatrix}0&1\\0&0\end{pmatrix}$ satisfies $N^2=0$.

## Detailed Step-by-Step Solution

$$AI=IA=A+0=\begin{pmatrix}2&1\\0&2\end{pmatrix}.$$
$$A^2=\begin{pmatrix}4&2+2\\0&4\end{pmatrix}=\begin{pmatrix}4&4\\0&4\end{pmatrix},\qquad
A^3=A^2A=\begin{pmatrix}8&4+8\\0&8\end{pmatrix}=\begin{pmatrix}8&12\\0&8\end{pmatrix}.$$
The binomial expansion has only two nonzero terms because $N^2=0$:
$$A^n=2^nI+n2^{n-1}N=\begin{pmatrix}2^n&n2^{n-1}\\0&2^n\end{pmatrix}\quad(n\ge1).$$

## Verification and Consistency Checks

The formula gives off-diagonal entries $1,4,12$ for $n=1,2,3$. Multiplication by $A$ sends that entry to $2^n+2n2^{n-1}=(n+1)2^n$, confirming the next power; $A^0=I$ separately.
