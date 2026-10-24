# Exercise 3 — When Can Matrices Be Multiplied?

## Problem Statement

Determine the validity and sizes of $AB,BA,BC,CB,AC,CA,AD,DA$ for $A:2\times3$, $B:3\times4$, $C:4\times2$, $D:2\times2$.

## Theoretical Background and Concepts

An $m\times n$ matrix times an $n\times p$ matrix produces an $m\times p$ matrix. The inner dimensions must agree.

## Detailed Step-by-Step Solution

| Product | Inner dimensions | Result |
| --- | --- | --- |
| $AB$ | $3=3$ | $2\times4$ |
| $BA$ | $4\ne2$ | Undefined |
| $BC$ | $4=4$ | $3\times2$ |
| $CB$ | $2\ne3$ | Undefined |
| $AC$ | $3\ne4$ | Undefined |
| $CA$ | $2=2$ | $4\times3$ |
| $AD$ | $3\ne2$ | Undefined |
| $DA$ | $2=2$ | $2\times3$ |

## Verification and Consistency Checks

For example, each entry of $AB$ pairs a length-3 row of $A$ with a length-3 column of $B$. In $BA$, lengths 4 and 2 cannot be paired. All valid result sizes retain the outer dimensions.
