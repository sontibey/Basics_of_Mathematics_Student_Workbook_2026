# Exercise 13 — A Recurrence in Matrix Form

## Problem Statement

For

```math
F=\begin{pmatrix}1&1\\1&0\end{pmatrix}
```

compute powers 2 through 5, relate them to Fibonacci numbers, and explain $F(a,b)^T$.

## Theoretical Background and Concepts

Define Fibonacci numbers by $f_0=0$, $f_1=1$, and $f_{n+1}=f_n+f_{n-1}$ for $n\ge1$. A matrix can update a pair of consecutive terms.

## Detailed Step-by-Step Solution

```math
F^2=\begin{pmatrix}2&1\\1&1\end{pmatrix},\quad F^3=\begin{pmatrix}3&2\\2&1\end{pmatrix},
```

```math
F^4=\begin{pmatrix}5&3\\3&2\end{pmatrix},\quad F^5=\begin{pmatrix}8&5\\5&3\end{pmatrix}.
```

The pattern is

```math
F^n=\begin{pmatrix}f_{n+1}&f_n\\f_n&f_{n-1}\end{pmatrix}\quad(n\ge1).
```

For any pair,

```math
F\begin{pmatrix}a\\b\end{pmatrix}=\begin{pmatrix}a+b\\a\end{pmatrix}.
```

Thus $(f_n,f_{n-1})^T$ becomes $(f_{n+1},f_n)^T$: the new term is the sum and the previous first term is retained.

## Verification and Consistency Checks

The power formula holds at $n=1$. Multiplying its right side by $F$ gives rows $(f_{n+1}+f_n,f_{n+1})$ and $(f_n+f_{n-1},f_n)$, precisely the formula at $n+1$. This proves the pattern by induction.
