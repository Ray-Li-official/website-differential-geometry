---
sidebar_position: 4
---

# 1.4 HyperPlanes

## 1.4.1 Bijection

Recall that if we have a function $f$ that maps from set $A$ to $B$, then we could desribe as following:
- Not a map: $\exist x \in A$, such that $x$ points to many $y \in B$.
- Injective: $\forall x_1, x_2 \in A$, $f(x_1) \neq f(x_2) \iff x_1 \neq x_2$.
- Surjective: $\forall y \in B$, we can find some $x \in A$ such that $f(x) = y$.
- Bijective: both injective and surjective.

That being said, a function $f:A\to B$ is bijective if and only if it has an inverse function $g: B \to A$.

If we have a function $f: A \to B$ that's bijective, then $A$ is global euclidean.

## 1.4.2 Hyperplane

:::note Definition of hyperplane
A hyperplane is a subplace that is one less dimension than the space around it.
:::
For example, a hyperplane of a **3-dimensional space** is a **2-dimensional plane**.

## 1.4.3 Cordinate Hyperplane
:::note Definition of cordinate hyperplane
We define the j-th cordinate hyperplace of $\mathbb{R}^{n+1}$ as following:
$$
\mathbb{C}_{j} = {X \in \mathbb{R}^{n+1}, X^j = 0}
$$
where $1 \leq j \leq n+1$
:::
Note we have a linear mapping $f$ from $\mathbb{C}_j$ to $\mathbb{R}^n$:
$$
f: \mathbb{C}_j \to \mathbb{R}^n = (X^1,\dots,X^{j-1},X^{j+1},\dots,X^{n+1})
$$
and its reverse function $g$:
$$
g: \mathbb{R}^n \to \mathbb{C}_j = (X^1,\dots,X^{j-1},0,X^{j+1},\dots,X^{n+1})
$$
We conclude that $f$ is bijective and thus the j-th cordinate hyperplace is **globally euclidean**.
## 1.4.4 Affine Hyperplane
:::note Definition of affine hyperplane
An affine hyperplane in $\mathbb{R}^{n+1}$ is defined as:
$$
\mathbb{A} = \{X \in \mathbb{R}^{n+1}, X \cdot N = a \}
$$
where $a \in \mathbb{R}$ and $N$ is called a norm to $\mathbb{A}$, a fixed non-zero vector.
:::

## 1.4.5 Linear Hyperplane
:::note Definition of linear hyperplane
A linear hyperplane is a special case of affine hyperplane such that:
$$
\mathbb{A} = \{X \in \mathbb{R}^{n+1}, X \cdot N = 0 \}
$$
:::