---
sidebar_position: 1
---
# 1.1 Euclidean Space

A special vector space equipped with distance function.

## 1.1.1 Vector Space
Note for vectors $X, Y \in \mathbb{R}^n$ we could perform **vector addition** and **scalar multiplication**, namely:
:::note
In this textbook, we use notations below to represents a vector:
$$X \in \mathbb{R}^n = (X^1,X^2,\dots,X^n)$$
:::
$$
X+Y = (X^1+Y^1,X^2+Y^2,\dots,X^n+Y^n)
$$
$$
aX = (aX^1, aX^2, \dots, aX^n)
$$
If for all vectors $X,Y,Z\in\mathbb{V}$ and for all scalars $a,b \in \mathbb{F}$, the following eight equations stand, we say $\mathbb{V}$ is a **vector space** over field $\mathbb{F}$:
- Associative: $(X+Y)+Z = X+(Y+Z)$
- Commutative: $X+Y = Y+X$
- Additive Identity: $X+\mathbf{0} = X$
- Inverse: $X + (-X) = \mathbf{0}$
- Compatibility of scalar multiplication: $a(bX) = (ab)X$
- Vector Distributive: $a(X+Y) = aX + aY$
- Scalar Distributive: $X(a+b) = aX + bX$
- Multiplication Identity: $\mathbf{1}X = X$

## 1.1.2 Inner Product
Inner product, also called the Euclidean inner product is defined as following:
$$
\text{If }X=(X^1,X^2,\dots,X^n),Y=(Y^1,Y^2,\dots,Y^n),X\cdot Y=\sum_{i=1}^nX^iY^i 
$$
where $X\cdot Y$is the inner product.

## 1.1.3 Inner Product Space
Assume we have a vector space $\mathbb{V}$ over a field $\mathbb{F}$, if for all $a,b \in \mathbb{F}$ and for all $X,Y,Z \in \mathbb{V}$, $W \in \mathbb{V}-\{\mathbf{0}\}$ we have the following statements satisfied, then we say $(\mathbb{V},\cdot)$ is a inner product space over field $\mathbb{F}$, where $\cdot$ is the inner product,
- Well-defined: $X\cdot Y \in \mathbb{F}$
- Symmetry: $X\cdot Y = Y\cdot X$
- Bilinearity: $(aX + bY)\cdot Z = a(X \cdot Y)+b(Y\cdot Z)$
- Positive-definite: $W\cdot W > 0$

## 1.1.4 Euclidean Space
An **Euclidean vector space** is a finite-dimensional inner product space over the real numbers.

## 1.1.5 Euclidean Distance and Angles
Assume $\mathbb{V} \subset \mathbb{R}^n$ is an euclidean space and we have $X,Y,Z\in \mathbb{V}$.

Then the **length** of $X$ is defined by:
$$
\lVert X \rVert :=  \sqrt{X \cdot X}
$$
the **distance** between $X$ and $Y$ is defined by:
$$
d(X,Y) := \lVert X-Y\rVert 
$$

:::tip Properties
- Symmetry: $d(X,Y) = d(Y,X)$
- Positive definite: $d(X,Y) \geq 0$, and $d(X,Y) = 0 \iff X=Y$.
- Triangle inequality: $d(X,Z) \leq d(X,Y) + d(Y,Z)$
:::