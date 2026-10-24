# Exercise 15 — Associativity and Calculation Paths

## Problem Statement

For

```math
A=\begin{pmatrix}1&2&0\\0&1&1\end{pmatrix},\qquad
B=\begin{pmatrix}1&0\\2&1\\-1&3\end{pmatrix},\qquad
C=\begin{pmatrix}2&1\\0&-1\end{pmatrix}
```

compute both parenthesizations and compare work.

## Theoretical Background and Concepts

Associativity means $(AB)C=A(BC)$ whenever dimensions permit. Standard multiplication of an $m\times n$ by an $n\times p$ matrix uses $mnp$ scalar multiplications and $mp(n-1)$ additions, counting zero entries without shortcuts.

## Detailed Step-by-Step Solution

First path:

```math
AB=\begin{pmatrix}1+4+0&0+2+0\\0+2-1&0+1+3\end{pmatrix}=\begin{pmatrix}5&2\\1&4\end{pmatrix},
```

```math
(AB)C=\begin{pmatrix}10&5-2\\2&1-4\end{pmatrix}=\begin{pmatrix}10&3\\2&-3\end{pmatrix}.
```

Second path:

```math
BC=\begin{pmatrix}2&1\\4&1\\-2&-4\end{pmatrix},
```

```math
A(BC)=\begin{pmatrix}2+8+0&1+2+0\\0+4-2&0+1-4\end{pmatrix}=\begin{pmatrix}10&3\\2&-3\end{pmatrix}.
```

For $(AB)C$, the two products use $12+8=20$ multiplications and $8+4=12$ additions. For $A(BC)$ they use $12+12=24$ multiplications and $6+8=14$ additions. The first intermediate matrix is $2\times2$; the second path first forms a $3\times2$ matrix. These counts use the stated standard algorithm; exploiting zeros can reduce them.

## Verification and Consistency Checks

Both independent paths give the same four entries and a $2\times2$ result. The equality changes grouping while keeping the factor order $A,B,C$ fixed; it does not assert that factors can be exchanged.
