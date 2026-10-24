# Exercise 6 — Transpose

## Problem Statement

For $A=\begin{pmatrix}1&2&3\\4&5&6\end{pmatrix}$ and $B=\begin{pmatrix}1&0\\2&1\\-1&3\end{pmatrix}$, compute transposes and $AB$, then verify $(AB)^T=B^TA^T$.

## Theoretical Background and Concepts

Transposition exchanges rows and columns: $(A^T)_{ij}=a_{ji}$. Transposing a product reverses factor order.

## Detailed Step-by-Step Solution

$$A^T=\begin{pmatrix}1&4\\2&5\\3&6\end{pmatrix},\qquad B^T=\begin{pmatrix}1&2&-1\\0&1&3\end{pmatrix}.$$
$$AB=\begin{pmatrix}1+4-3&0+2+9\\4+10-6&0+5+18\end{pmatrix}=\begin{pmatrix}2&11\\8&23\end{pmatrix}.$$
Consequently $(AB)^T=\begin{pmatrix}2&8\\11&23\end{pmatrix}$.

## Verification and Consistency Checks

Direct multiplication gives
$$B^TA^T=\begin{pmatrix}1+4-3&4+10-6\\0+2+9&0+5+18\end{pmatrix}=\begin{pmatrix}2&8\\11&23\end{pmatrix}=(AB)^T.$$
Both sides have size $2\times2$.
