# Exercise 2 — Addition and Scalar Multiplication

## Problem Statement

For

```math
A=\begin{pmatrix}1&2\\-1&3\end{pmatrix},\qquad B=\begin{pmatrix}4&-2\\0&5\end{pmatrix},
```

compute $A+B$, $A-B$ and $3A-2B$. Explain why matrix addition requires matrices of the same size.

## Theoretical Background and Concepts

Addition and subtraction operate on corresponding entries:

```math
(A+B)_{ij}=a_{ij}+b_{ij},\qquad (A-B)_{ij}=a_{ij}-b_{ij}.
```

Scalar multiplication multiplies every entry: $(cA)_{ij}=ca_{ij}$. Matrix addition requires equal numbers of rows and columns so that every entry has a corresponding entry in the other matrix. Both matrices here have size $2\times2$.

## Detailed Step-by-Step Solution

Adding corresponding entries,

```math
A+B=\begin{pmatrix}1+4&2+(-2)\\-1+0&3+5\end{pmatrix}
=\boxed{\begin{pmatrix}5&0\\-1&8\end{pmatrix}}.
```

Subtracting corresponding entries,

```math
A-B=\begin{pmatrix}1-4&2-(-2)\\-1-0&3-5\end{pmatrix}
=\boxed{\begin{pmatrix}-3&4\\-1&-2\end{pmatrix}}.
```

First multiply each matrix by its scalar:

```math
3A=\begin{pmatrix}3&6\\-3&9\end{pmatrix},\qquad
2B=\begin{pmatrix}8&-4\\0&10\end{pmatrix}.
```

Then subtract:

```math
3A-2B=\begin{pmatrix}3-8&6-(-4)\\-3-0&9-10\end{pmatrix}
=\boxed{\begin{pmatrix}-5&10\\-3&-1\end{pmatrix}}.
```

## Verification and Consistency Checks

All results have size $2\times2$, as required. Undoing the addition gives

```math
\begin{pmatrix}5&0\\-1&8\end{pmatrix}-B
=\begin{pmatrix}1&2\\-1&3\end{pmatrix}=A.
```

Undoing the subtraction gives

```math
\begin{pmatrix}-3&4\\-1&-2\end{pmatrix}+B
=\begin{pmatrix}1&2\\-1&3\end{pmatrix}=A.
```

An independent rearrangement confirms the last result:

```math
3A-2B=A+2(A-B)
=\begin{pmatrix}1&2\\-1&3\end{pmatrix}
+\begin{pmatrix}-6&8\\-2&-4\end{pmatrix}
=\begin{pmatrix}-5&10\\-3&-1\end{pmatrix}.
```
