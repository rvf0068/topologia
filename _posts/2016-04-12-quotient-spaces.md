---
layout: post
title: Quotient spaces
date: 2016-04-12 11:00 
comments: true
published: true
categories: 
---

# Definition

## Quotient maps

1.  Quotient map

    Let $$X,Y$$ be topological spaces and  $$p\colon X\to Y$$ a
    *surjective* map. Then $$p$$ is called a **quotient map** if
    $$U\subseteq Y$$ is open if and only if $$p^{-1}(U)$$ is open in
    $$X$$. 

2.  Remarks
    -   $$p$$ is a quotient map if and only if $$p$$ is surjective and
        $$p^{-1}(A)$$ is closed in $$X$$ if and only if $$A\subseteq Y$$
        closed.
    -   Maps which are open, continuous and surjective are quotient maps.
    -   Maps which are closed, continuous and surjective are quotient maps.

## Saturated subsets

1.  Fiber

    Let $$p\colon X\to Y$$ be a *surjective* map between sets and $$y\in
        Y$$. The inverse image set
    
    $$
    p^{-1}(\{y\})=\{x\in X\mid p(x)=y\}
    $$
    
    will be denoted as $$p^{-1}(y)$$ and referred to as the **fiber** of $$y$$.

2.  Saturated set

    Let $$p\colon X\to Y$$ be a *surjective* map between sets. We say
    that $$A\subseteq X$$ is **saturated (with respect to $$p$$)** if
    $$A\cap p^{-1}(y)\ne\emptyset$$ implies $$p^{-1}(y)\subseteq A$$



1.  Remarks
    -   $$A$$ is saturated if and only if $$A=p^{-1}(p(A))$$.
    -   If $$U\subseteq Y$$, then $$p^{-1}(U)$$ is saturated.
    -   $$p$$ is a quotient map if and only if $$p$$ is surjective,
        continuous, and $$A$$ saturated and open implies $$p(A)$$ open.
    -   $$p$$ is a quotient map if and only if $$p$$ is surjective,
        continuous, and $$A$$ saturated and closed implies $$p(A)$$
        closed.

## Quotient topology

1.  Quotient topology

    Let $$X$$ be a space, $$A$$ a *set*, and $$p\colon X\to A$$ a
    *surjective* map. Then there is exactly one topology on $$A$$ that
    makes $$p$$ a quotient map, such topology is called **quotient
    topology**.

2.  Remark

    One must check that:
    
    $$
      \tau=\{U\subseteq A\mid \text{\(p^{-1}(U)\) is open in \(X\)}\}
    $$
    
    is a topology on $$A$$.

## Partitions

1.  Partition

    Let $$X$$ be a set. A **partition** $$\tilde{X}$$ of $$X$$ is a collection
    of nonempty disjoint subsets of $$X$$ with union $$X$$

2.  Quotient space

    Let $$X$$ be a topological space, $$\tilde{X}$$ be a partition of
    $$X$$, and $$p\colon X\to \tilde{X}$$ the natural surjection. If we
    give $$\tilde{X}$$ the quotient topology induced by $$p$$, the space
    $$\tilde{X}$$ is called a **quotient space** of $$X$$

## Quotients and subspaces

1.  

    If $$p\colon X\to Y$$ is a quotient map and $$A\subseteq X$$ is a
    subspace, it does not necessarily follow that the restriction of
    $$p$$: $$A\to p(A)$$ is a quotient map. However we have:

2.  Quotients and subspaces

     Let $$p\colon X\to Y$$ be a quotient map and $$A\subseteq X$$ a
    subspace, that is saturated with respect to $$p$$, and let
    $$q\colon A\to p(A)$$ the restriction of $$p$$. Then:
    
    -   if $$A$$ is open or closed, then $$q$$ is a quotient map,
    -   if $$p$$ is open or closed, then $$q$$ is a quotient map.

## Proof

-   We verify the following:
    
    $$
    
    \begin{align*}
    q^{-1}(V)  &=p^{-1}(V)      &\text{if \(V\subseteq p(A)\)},\\
    p(U\cap A) &= p(U)\cap p(A) &\text{if \(U\subseteq X\)}.
    \end{align*}
    
    $$

## Quotients and compositions

1.  Teorema

    Composition of quotient maps is a quotient map.

# Maps going out of quotients

## Fundamental theorem

1.  Fundamental theorem

    Let $$p\colon X\to Y$$ be a quotient map. Let $$Z$$ be a space,
    and $$g\colon X\to Z$$ a continuous map that is constant on each
    fiber of $$p$$, that is $$p(x)=p(x')$$ implies
    $$g(x)=g(x')$$. Then $$g$$ induces a continuous map
    $$\overline{g}\colon Y\to Z$$ such that $$\overline{g}\circ
        p=g$$. The function $$\overline{g}$$ is unique with the property
    that $$\overline{g}\circ p=g$$
    
    {: .center}
![img]({{ site.baseurl }}otients-01.png)

## Fundamental theorem

1.  Fundamental theorem, for equivalence relations

    Let $$X$$ be a space, and $$\sim$$ an equivalence relation on
    $$X$$. Let $$g\colon X\to Z$$ be a continuous map such that
    $$g(x)=g(x')$$ whenever $$x\sim x'$$. Then, if we denote by
    $$p\colon X\to X/\!\!\sim$$ the quotient map, the map $$g$$ induces
    a unique continuous map $$\overline{g}\colon X/\!\!\sim\,\to Z$$ such that
    $$\overline{g}\circ p=g$$
    
    {: .center}
![img]({{ site.baseurl }}otients-02.png)
