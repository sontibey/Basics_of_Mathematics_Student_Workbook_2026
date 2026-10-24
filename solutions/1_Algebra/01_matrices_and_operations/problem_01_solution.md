# Exercise 1 — Matrix Size and Entries

## Problem Statement

Given
$$
A=\begin{pmatrix}2&-1&3\\0&4&5\end{pmatrix},\qquad
B=\begin{pmatrix}1&0\\-2&3\\4&1\end{pmatrix},
$$
state their sizes, identify $a_{12}$, $a_{23}$, $b_{21}$ and $b_{32}$, and write the second row of $A$ and the first column of $B$ as vectors.

## Theoretical Background and Concepts

A matrix with $m$ rows and $n$ columns has size $m\times n$. The entry $a_{ij}$ is in row $i$ and column $j$, with indices starting at 1. A row vector has size $1\times n$, and a column vector has size $m\times1$.

## Detailed Step-by-Step Solution

1. $A$ has 2 rows and 3 columns, so its size is $2\times3$. $B$ has 3 rows and 2 columns, so its size is $3\times2$.
2. Reading the indicated row and column gives
   $$a_{12}=-1,\qquad a_{23}=5,\qquad b_{21}=-2,\qquad b_{32}=1.$$
3. The second row of $A$ is the row vector
   $$\begin{pmatrix}0&4&5\end{pmatrix}.$$
   The first column of $B$ is the column vector
   $$\begin{pmatrix}1\\-2\\4\end{pmatrix}.$$

## Verification and Consistency Checks

Both matrices contain 6 entries: $2\cdot3=3\cdot2=6$. The second row of $A$ has 3 components, matching its number of columns; its third component is $a_{23}=5$. The first column of $B$ has 3 components, matching its number of rows; its second component is $b_{21}=-2$. The remaining requested entries are the second component of the first row of $A$ ($-1$) and the second component of the third row of $B$ ($1$).
