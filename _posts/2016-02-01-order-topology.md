---
layout: post
title: The order topology
date: 2016-02-01 9:00 -0500 
comments: true
published: true
categories: 
---

# Order topology

## Total order

1.  Total order

    A relation $$<$$ on a set $$X$$ is called a **total (or linear)
    order** if the following is satisfied:
    
    -   **(O1):** For every $$x,y\in X$$ with $$x\ne y$$, we have that
        $$x<y$$ or $$y<x$$ (**comparability**).
    -   **(O2):** For every $$x\in X$$, we have that $$x\not<x$$
        (**nonreflexivity**).
    -   **(O3):** if $$x<y$$ and $$y<z$$, then $$x<z$$ (**transitivity**).

2.  Totally ordered set

    In this case, the pair $$(X,<)$$ is called a **totally ordered
    set**. If $$x<y$$ or $$x=y$$, we write $$x\leq y$$. An example of a
    total order is given by $$X=\mathbb{R}$$ with usual order.

## Intervals

1.  Intervals

    If $$X$$ is a totally ordered set, and $$a,b\in X$$, we will use
    the following notation for **intervals**:
    
    $$
    
    \begin{align*}
    [a,b] &=\{x\in X\mid a\leq x\leq b\}\\
    (a,b) &=\{x\in X\mid a< x< b\}\\
    (a,b] &=\{x\in X\mid a< x\leq b\}\\
    [a,b) &=\{x\in X\mid a\leq x< b\}\\
    (a,\infty) &=\{x\in X\mid x>a\}\\
    (-\infty,b) &=\{x\in X\mid x<b\}
    \end{align*}
    
    $$

## The order topology

1.  Order topology

    Let $$X$$ be a totally ordered set with more than one element. Let
    $$\mathcal{S}$$ be the collection:
    
    $$
    \mathcal{S}=\{(-\infty,a)\mid a\in X\}\cup\{(b,\infty)\mid b\in X\}.    
    $$
    
    Then $$\mathcal{S}$$ is subbase for a topology on $$X$$, called
    **order topology**.

## Base for the order topology

1.  Base for the order topology

    Let $$X$$ be a totally ordered set with more than one element. Let
    $$\mathcal{B}$$ be the collection of all intervals of the form
    $$(a,b)$$, together with those of the form $$[m,b)$$, in case
    $$X$$ has a minimum $$m$$, and those of the form $$(a,M]$$, in
    case $$X$$ has a maximum $$M$$. Then $$\mathcal{B}$$ is a base
    for the order topology on $$X$$.

2.  Proof

    The set of finite intersections of the intervals in the subbasis
    can be obtained as union of elements of the intervals described.
    $$\Box$$

## Dictionary order

1.  Dictionary order

    Let $$X$$ and $$Y$$ be totally ordered sets. We define an order
    relation on the cartesian product $$X\times Y$$ by:
    
    $$
    (x,y)<(x',y'),
    $$
    
    if either:
    
    -   $$x< x'$$, or
    -   $$x=x'$$ and $$y< y'$$.

2.  The dictionary order is a total order

    The order on $$X\times Y$$ just described is a total order,
    called the **dictionary order**. 

## Proof that the dictionary order is a total order

-   Let $$(x,y)\ne (x',y')$$ with $$(x,y), (x',y')\in X\times Y$$. If
    $$x\ne x'$$, then one of the pairs is less than the
    other. Otherwise $$x=x'$$, and since the pairs are distinct, we
    must have $$y\ne y'$$, and so (O1) follows.
-   If we had $$(x,y)<(x,y)$$, then it would follow that either
    $$x<x$$ or $$x=x,y<y$$. Since none of these is possible, we
    conclude that (O2) is true.
-   The proof of (O3) is left as an exercise.

## Examples

-   The order topology on $$\mathbb{R}$$ is the same as the standard
    topology.
-   The order topology on $$\mathbb{R}\times \mathbb{R}$$ with the
    dictionary order is different from the usual metric topology on
    $$\mathbb{R}^2$$.
-   The order topology on $$\{0,1\}\times \mathbb{N}$$ has almost
    all singletons as open sets.



## Exercises

1.  Let $$(X,<)$$ be a totally ordered set, and let $$Y\subseteq
         X$$. If, for $$y,y'\in Y$$ we define $$y<'y'$$ whenever $$y<y'$$ in
    $$X$$, show that $$(Y,<')$$ is a totally ordered set.
2.  If $$X$$ is a totally ordered set, and $$Y\subseteq X$$, show that
    $$Y$$ can have at most one smallest element.
3.  If $$X$$ is a totally ordered set, and we have that $$x<y$$ and
    there are no $$z\in X$$ such that $$x<z<y$$, we say that $$y$$ is
    an **immediate succesor** of $$x$$. Show that any $$x\in X$$ has
    at most one immediate succesor.
4.  Let $$(X,<)$$ be a totally ordered set with no minimum element,
    and let $$\mathcal{C}=\{(a,\infty)\mid a\in X\}$$. Show that
    $$\mathcal{C}$$ is a basis for a topology on $$X$$. Is
    $$\tau_{\mathcal{C}}$$ in general, the same as the order
    topology?



## Links

-   [Total order - Wikipedia, the free encyclopedia](http://en.wikipedia.org/wiki/Totally_ordered_set)
-   [Order topology - Wikipedia, the free encyclopedia](http://en.wikipedia.org/wiki/Order_topology)
