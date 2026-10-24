# Exercise 14 — Rotation Matrices

## Problem Statement

For $R(\theta)=\begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix}$, prove $R(\alpha)R(\beta)=R(\alpha+\beta)$ and interpret it.

## Theoretical Background and Concepts

Use $\cos(\alpha+\beta)=\cos\alpha\cos\beta-\sin\alpha\sin\beta$ and $\sin(\alpha+\beta)=\sin\alpha\cos\beta+\cos\alpha\sin\beta$.

## Detailed Step-by-Step Solution

Writing $c_\alpha=\cos\alpha$, $s_\alpha=\sin\alpha$ and similarly for $\beta$,
$$R(\alpha)R(\beta)=\begin{pmatrix}c_\alpha c_\beta-s_\alpha s_\beta&-c_\alpha s_\beta-s_\alpha c_\beta\\s_\alpha c_\beta+c_\alpha s_\beta&-s_\alpha s_\beta+c_\alpha c_\beta\end{pmatrix}.$$
The angle-sum identities transform this into
$$\begin{pmatrix}\cos(\alpha+\beta)&-\sin(\alpha+\beta)\\\sin(\alpha+\beta)&\cos(\alpha+\beta)\end{pmatrix}=R(\alpha+\beta).$$
Geometrically, rotating first through $\beta$ and then through $\alpha$ about the same origin adds the two directed angles while preserving length.

## Verification and Consistency Checks

With $\beta=-\alpha$, the product is $R(0)=I$, as expected for inverse rotations. With $\alpha=\beta=\pi/2$, the product is $R(\pi)=-I$, a half-turn.
