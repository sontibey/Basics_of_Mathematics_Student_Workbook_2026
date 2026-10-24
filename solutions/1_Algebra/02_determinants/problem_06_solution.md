# Exercise 6 — Parameter and Invertibility

## Problem Statement

Find the real values of $t$ for which $A(t)=\begin{pmatrix}t&1\\2&t\end{pmatrix}$ is not invertible.

## Theoretical Background and Concepts

A square matrix is singular exactly when its determinant is zero.

## Detailed Step-by-Step Solution

$$\det A(t)=t\cdot t-1\cdot2=t^2-2.$$
Thus $A(t)$ is not invertible exactly when $t^2=2$, or
$$\boxed{t=\sqrt2\text{ or }t=-\sqrt2}.$$
For every other real value, $t^2-2\ne0$ and the matrix is invertible.

## Verification and Consistency Checks

For either root, the nonzero vector $(1,-t)^T$ satisfies $A(t)(1,-t)^T=(0,2-t^2)^T=(0,0)^T$, directly confirming a nontrivial kernel.
