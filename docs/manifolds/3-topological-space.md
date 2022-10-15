---
sidebar_position: 3
---

# 1.3 Topological Space
Tolological space is a space where **closeness** is defined. 

Obviously the statement above is not a precise and formal definition of topological space. We'll introduce some formal definition of topological space later in this chapter. But, let's talking about **closeness** for now.

## 1.3.1 Clossness
Assume we are in a space $\mathbb{V}$, and there are three points $X,Y,P \in \mathbb{V}$. How could we know which point is closer to $P$?

### Euclidean
It would be easy if we are in an euclidean space: $X$ is closer to $P$ if $\lVert X-P\rVert < \lVert Y-P \rVert$

### Metric
Remember we have distance function for metric space? So $X$ is closer to $P$ if $d(X,P) < d(Y,P)$

### No Distance Function?
But if we are in a space where there's no distance function, how should we answer the above question?

Let's starting from the **metric space** and trying to generize it: firstly think about an open ball around point $P$ with radius $r$.

:::note Definition of Open Ball
$$
B_r(P) = \{Q:d(Q,P) < r\}
$$
:::

And there would be different open balls around point $P$ with different radius. We claim that $X$ is closer to $P$ if $X$ is in a smaller open ball.

This is the **core** of topology! We could define something like an open ball but without distance function. Just like we could create a consistent sequence of open balls around point $P$ with different radius, we could create a consistent sequence of some structs of point $P$ where the latter is strictly larger than(or we can say strictly include) the former one. 

And finally we could say $X$ is closer to $P$ if $X$ is in the smaller struct. We will refer to the term **struct** as **neigborhood** from now on in this textbook.

## 1.3.2 Precise Definition of Topological Space
:::note Definition of Topological Space
Let $\mathbb{V}$ be a set and $\mathcal{N}$ be the function that create a consistent sequence of neigborhoods around $X, X\in\mathbb{V}$. If $\mathbb{V}$ with $\mathcal{N}$ could satisfy all the following axioms, then we define $(\mathbb{V},\mathcal{N})$ as topological space:
- $\forall N \in \mathcal{N}(X),  X \in N$. All points belongs to every of its neigborhoods.
- $N_1 \subset \mathbb{V}, N_2 \in \mathcal{N}(X), N_2 \subset N_1 \to N_1 \in \mathcal{N}(X)$. Every superset of a neighbourhood of a point is again a neighbourhood of this point.
- $\forall N_1,N_2 \in \mathcal{N}(X), N_1\cap N_2 \in \mathcal{N}(X)$. The intersection of two neighbourhoods of a point is a neighbourhood of this point.
- $\forall N_1 \in \mathcal{N}(X), \exist N_2\in \mathcal{N}(X), \forall Y \in N_2, N_1 \in \mathcal{N}(Y)$. For all neighbourhoods of a points, named $N$, there exists another neighbourhood whose points'neighbourhoods contains $N$.
:::