# Exercise Set 1 for the Financial Markets Course

Commit with your solutions.

---
title: "Financial Markets Exercise 1"
author: "J. Krogsgaard"
date: "2024-02-07"
output:
  pdf_document: default
  html_document: default
---

Proposition proof:
The $\succsim$ relation is rational, meaning that it satisfies the two requirements of rationality:
Completeness, and Transitivity. (Also just going to assume continuity, we do not need to, as they can
all be solved with just using the relations, just easier to explain).

i. Prove that strongly prefered is both irreflexive and transitive. 
To be strongly prefered, it means that x is weakly prefered over y, but y is not weakly prefered over x

To be irreflexive in this case, is saying that x is weakly prefered to x, but also not weakly prefered to x.
As is the definition for strong preference, but this obviosuly does not hold, as it would contradict itself
and is therefore not reflexive.

Finally for it to be transitive, it needs to follow that if we have $x,y,z$, and have the relations 
$x \succ y$, and $y \succ z$, it would follow that $x \succ z$. 
Due to $\succeq$ being rational, it already is transitive, and when used for this case it would keep
its condition.

ii. The indifference relation $\sim$ is defined, when x,y have the relations:
$x \succeq y$, and $y \succeq x$.

To prove it is reflexive, we can simply state for $x \sim x$, that is has the relations
$x \succeq x$, and $x \succeq x$, which are the same, and is therefore reflexive.

To prove its transitivity, it should be enough to state the definition which involves the use 
of the weakly prefered relation, which is sat to be rational in this proof.

Finally for symmetry, we can prove it by thinking of it in terms of utility functions.
If we set up two utility functions for the relation $x \sim y$, we can get $u(x) = 2 = u(y)$
Where the indifference is showing that $2 \geq 2$ and $2 \geq 2$. As they are the same
on either side, it is easy to say they are symmetric. 

iii. We can again use utility functions to show this relation.
If we set up utility functions, such that the relation holds, fx. 
$u(x) = 5, u(y) = 3 < 5, u(z) = 3 \leq u(y)$ then it is easy to see that
it should hold, that $u(x) < u(z)$, or $x \succ z$.


Lexicographic preference proof:
We define the lexicographic preference relation $\succsim$ over $R^2$ as 
$(x_1,x_2) \succsim (y_1,y_2)$ if either $x_1 > y_1$ or $x_1=y_1$ and $x_2 \geq y_1$.

i. Add a third $(z_1,z_2)$ which has the relation $(y_1,y_2) \succsim (z_1,z_2)$.
For it to be transitive, it should mean that: 
$x_1 > y_1$ and $y_1 > z_1$ then $x_1 > z_1$.

or $\geq$ for the second variable using the second definition.


ii. To be considered continuous, it needs to satisfy the continuity assumption,
wich says that the lower and upper contours sets are closed. We can figure this out
by looking at the limit. Considering the sequence, which we can write on the form
of the lexicographic preference: $(x_1^n,x_2^n)=(1-\frac{1}{n},1)$ and $(y_1,y_2)=(1,0)$.

We can see from just the sequence itself, we should have that $(1,0) \geq (1-\frac{1}{n},1)$
for any $n \in N$, but as we go towards the limit, $lim_{n \rightarrow \infty}$, 
we see that at the limit of our sequence, we have that $lim_{n \rightarrow \infty}(1-\frac{1}{n},1) \geq (1,0)$.
Therefore, for our definition of continuity, it is not valid.


Exercise 3 with plotting:
$U(x):=(a_1 \times x_1^p + a_2 \times x_2^p)^(1/p)$

i. $p=1$
Without needing to plot the function, we can see by inserting $p=1$ into the function
that we would simply be left with $U(x)=a_1 \times x_1 + a_2 \times x_2)$, which
we know to be a linear function.

ii. $p \rightarrow 0$
