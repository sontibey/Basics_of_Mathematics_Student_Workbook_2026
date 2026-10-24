# Exercise 9 — Composing Transformations

## Problem Statement

For $S=\begin{pmatrix}2&0\\0&1\end{pmatrix}$, $R=\begin{pmatrix}0&-1\\1&0\end{pmatrix}$, $x=(1,2)^T$, compare $RSx$ and $SRx$ geometrically.

## Theoretical Background and Concepts

In a product acting on a vector, the rightmost transformation acts first. $S$ doubles the horizontal coordinate and $R$ rotates counterclockwise through $90^\circ$.

## Detailed Step-by-Step Solution

First scale, then rotate:
$$Sx=(2,2)^T,\qquad RSx=(-2,2)^T.$$
First rotate, then scale:
$$Rx=(-2,1)^T,\qquad SRx=(-4,1)^T.$$
The outputs differ. Scaling along the fixed horizontal axis before rotation stretches a different original direction than scaling along that axis after rotation.

## Verification and Consistency Checks

$$RS=\begin{pmatrix}0&-1\\2&0\end{pmatrix},\qquad SR=\begin{pmatrix}0&-2\\1&0\end{pmatrix}.$$
Applying these products directly to $(1,2)^T$ reproduces $(-2,2)^T$ and $(-4,1)^T$.
