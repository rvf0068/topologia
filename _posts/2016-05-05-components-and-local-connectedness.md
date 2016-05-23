---
layout: post
title: Components and local connectedness
date: 2016-05-05 10:00 
comments: true
published: true
categories: 
---

# Connected components

## Definition

1.  Equivalence relation

    Let $$X$$ be a topological space. We define a relation $$\sim$$ on
    $$X$$ by declaring $$x\sim y$$ if there is $$Y\subseteq X$$
    connected, such that $$x,y\in Y$$.

2.  Connected components

    One can prove that $$\sim$$ is an equivalence relation. The
    equivalence classes are called **connected components** of $$X$$.

## Properties

1.  Teorema

    The connected components of $$X$$ have the following properties:
    
    -   They are connected, disjoint subsets of $$X$$ with union $$X$$.
    -   Each connected nonempty subset of $$X$$ intersects exactly one
        of them.
    -   They are closed, and if there are finitely many components,
        they are also open.

# Path components

## Definition

1.  A new equivalence relation

    We define a relation $$\sim$$ on the topological space $$X$$, by
    setting $$x\sim y$$ if there is a path from $$x$$ to $$y$$.

2.  Path components

    One can prove that $$\sim$$ is an equivalence relation. The
    equivalance classes are called **path components** of $$X$$.

## Properties

1.  Teorema

    The path components of $$X$$ have the following properties:
    
    -   They are path-connected, disjoint subsets of $$X$$ with union
        $$X$$.
    -   Each nonempty path-connected subset of $$X$$ intersects exactly
        one of them.

## The topologist's sine curve

{: .center}
![img]({{ site.baseurl }}mponents-01.png)

# Local conectedness

## Definition

1.  Locally connected space
    -   $$X$$ is **locally connected at $$x\in X$$** if for any neighborhood
        $$U$$ of $$x$$, there is a connected neighborhood of $$x$$
        contained in $$U$$.
    -   If $$X$$ is locally connected at every point, then we say that
        $$X$$ is **locally connected**.

2.  Locally path connected space
    -   $$X$$ is **locally path connected at $$x\in X$$** if for any
        neighborhood $$U$$ of $$x$$, there is a path
        connected neighborhood of $$x$$ contained in $$U$$.
    -   If $$X$$ is locally path connected at every point, then we say
        that $$X$$ is **locally path connected**.

## Examples

1.  :B<sub>exampleblock</sub>:
    -   Any interval in $$\mathbb{R}$$ is connected and locally
        connected.
    -   The subspace $$[0,1]\cup [2,3]\subseteq \mathbb{R}$$ is locally
        connected and not connected.
    -   The topologist's sine curve is connected but not locally connected.
    -   $$\mathbb{Q}$$ as a subspace of $$\mathbb{R}$$ is neither
        connected nor locally connected.



1.  Teorema

    A space $$X$$ is locally connected if and only if for every open
    set $$U$$ of $$X$$, each component of $$U$$ is open in $$X$$.

2.  Proof
    -   Suppose that $$X$$ is locally connected, and let $$C$$ be a
        component of the open set $$U\subseteq X$$.
    -   Let $$x\in C$$, and choose $$V$$ a connected neighborhood of
        $$x$$ with $$V\subseteq U$$.
    -   Since $$V$$ is connected, it must be contained in $$C$$.
    -   Now suppose the components of open sets in $$X$$ are open.
    -   Let $$x\in X$$ and a neighborhood $$U$$ of $$x$$. If $$C$$ is
        the component of $$U$$ that contains $$x$$, then $$C$$ is a
        connected neighborhood of $$x$$.\qed



The proof of the following theorem is similar and left as an
exercise. 

1.  Teorema

    A space $$X$$ is locally path connected if and only if for every
    open set $$U$$ of $$X$$, each path component of $$U$$ is open in
    $$X$$.

## Components and path components

1.  Teorema
    -   For any space $$X$$, each path component of $$X$$ is contained
        in a component of $$X$$.
    -   If $$X$$ is locally path connected, the components and the
        path components are the same.

2.  Proof
    -   Let $$C$$ be a component of $$X$$, let $$x\in C$$, and let $$P$$
        be the path component of $$X$$ containg $$x$$. Since $$P$$ is
        connected, $$P\subseteq C$$.
    -   Suppose now that $$X$$ is locally path connected, and we wish to
        prove $$P=C$$. Assume that $$P\subsetneq C$$.



1.  Proof (continuation)
    -   Let $$S$$ be the union of all the path components of $$X$$
        different from $$P$$ that intersect $$C$$. Since such components
        must lie in $$C$$, we have $$C=P\cup S$$.
    -   Since $$X$$ is locally path connected, each path component of
        $$X$$ is open in $$X$$. Hence $$P$$ and $$S$$ are open, disjoint
        and nonempty sets with union $$C$$. This contradicts that $$C$$
        is connected.\qed
