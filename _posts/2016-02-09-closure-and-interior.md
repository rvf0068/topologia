---
layout: post
title: Closure and interior
date: 2016-02-09 11:00 -0500 
comments: true
published: true
categories: 
---

# Closure and interior

## Closure

1.  Closure

    Let $$X$$ be a space and $$D\subseteq X$$. The **closure** of $$D$$ is
    the intersection of all closed sets that contain $$D$$. It is
    denoted by $$\overline{D}$$

2.  Examples
    -   If $$X$$ has indiscrete topology, then $$\overline{A}=X$$ if and
        only if $$A\ne\emptyset$$.
    -   If $$X$$ has discrete topology, then for all $$A\subseteq X$$ we
        have $$\overline{A}=A$$.
    -   If $$X$$ has cofinite topology, then $$\overline{A}=A$$ if and
        only if $$A$$ is finite.

3.  Lemma

    $$D$$ is closed if and only if $$D=\overline{D}$$.

## Characterization of closure

1.  Properties of closure

    The closure of $$D\subseteq X$$ satisfies:
    
    -   $$\overline{D}$$ is closed.
    -   $$D\subseteq \overline{D}$$.
    -   If $$A\subseteq X$$ is closed and $$D\subseteq A$$, then
        $$\overline{D}\subseteq A$$.

2.  Characterization of closure

    The first three properties in the last theorem characterize
    $$\overline{D}$$, in the sense that if $$R$$ is a closed set that
    contains $$D$$, and that is contained in any closed set that
    contains $$D$$, then we must have $$R=\overline{D}$$.

## Closure and subspaces

1.  Note

    If $$Y$$ is a subspace of $$X$$ and $$D\subseteq Y$$, the closure
    of $$D$$ in $$Y$$ and the closure of $$D$$ in $$X$$ might be
    different. The notation $$\overline{D}$$ will always denote the
    closure in $$X$$.

2.  Closure and subspaces

    Let $$Y$$ be a subspace of $$X$$ and $$D\subseteq Y$$. Then the
    closure of $$D$$ in $$Y$$ equals $$\overline{D}\cap Y$$.

3.  Proof

    We prove that $$\overline{D}\cap Y$$ satisfies the properties that
    characterize the closure of $$D$$ in $$Y$$.

## Other characterizations of closure

1.  Intersecting sets

    We will say that the set $$A$$ **intersects** the set $$B$$ if $$A\cap
        B\ne\emptyset$$

2.  Neighborhood

    If $$x\in X$$, a **neigborhood** of $$x$$ is an open set $$U$$ such
    that $$x\in U$$.

3.  Points in closure

    Let $$X$$ be a space, $$A\subseteq X$$ and $$x\in X$$. Then
    
    -   $$x\in \overline{A}$$ if and only if every neighborhood of $$x$$
        intersects $$A$$.
    -   If the topology of $$X$$ is given by the basis $$\mathcal{B}$$,
        then $$x\in \overline{A}$$ if and only if every $$B\in
              \mathcal{B}$$ that contains $$x$$ intersects $$A$$.

## Limit points

1.  Limit point

    Let $$X$$ be a space, $$A\subseteq X$$ and $$x\in X$$. We say that
    $$x$$ is a **limit point** of $$A$$ if every neighborhood of $$x$$
    intersects $$A$$ in a point different from $$x$$. We denote the
    set of all limit points of $$A$$ by $$A'$$.

2.  Closure and limit points

    Let $$X$$ be a space and $$A\subseteq X$$. Then
    $$\overline{A}=A\cup A'$$.

3.  Proof
    -   Let $$x\in \overline{A}$$. If $$x\in A$$, then $$x$$ is in the
        set on the right side. If $$x\not\in A$$, let $$U$$ be a
        neighborhood of $$x$$. Then $$U$$ intersects $$A$$ in a point
        different from $$x$$.
    -   From the definition it follows immediately that $$A'\subseteq
              \overline{A}$$, and also $$A\subseteq \overline{A}$$ always. $$\Box$$



1.  Remark

    It follows that $$A$$ is closed if and only if $$A'\subseteq A$$.

## Interior

1.  Interior

    Let $$X$$ be a space and $$D\subseteq X$$. The **interior** of $$D$$
    is the union of all open sets contained in $$D$$. It is denoted by
    $$D^{\circ}$$.

2.  Properties of interior

    The interior of $$D\subseteq X$$ satisfies:
    
    -   $$D^{\circ}$$ is open.
    -   $$D^{\circ}\subseteq D$$.
    -   If $$U\subseteq X$$ is open and $$U\subseteq D$$, then
        $$U\subseteq D^{\circ}$$.
    -   $$U$$ is open if and only if $$U=U^{\circ}$$.



## Links

-   [Closure (topology) - Wikipedia, the free encyclopedia](https://en.wikipedia.org/wiki/Closure_(topology))
-   [Interior (topology) - Wikipedia, the free encyclopedia](https://en.wikipedia.org/wiki/Interior_(topology))
-   [Limit point - Wikipedia, the free encyclopedia](https://en.wikipedia.org/wiki/Limit_point)



## Exercises

-   True or false? For all $$A,B\subseteq X$$, $$\overline{A\cap
         B}=\overline{A}\cap \overline{B}$$.
-   True or false? For all $$A,B\subseteq X$$, $$\overline{A\cup
         B}=\overline{A}\cup \overline{B}$$.
-   True or false? For all $$A,B\subseteq X$$, $$(A\cap
         B)^{\circ}=A^{\circ}\cap B^{\circ}$$.
-   True or false? For all $$A,B\subseteq X$$, $$(A\cup
         B)^{\circ}=A^{\circ}\cup B^{\circ}$$.
-   We define the **boundary** $$\partial A$$ as $$\partial A=
         \overline{A}\cap \overline{X-A}$$. Prove that
    $$\overline{A}=A\cup\partial A$$, that $$A$$ is closed if and
    only if $$\partial A\subseteq A$$, and that $$A$$ is open if and
    only if $$\partial A\cap A=\emptyset$$.
-   We define the **exterior** $$\mathrm{ext}(A)$$ as
    $$\mathrm{ext}(A)=(X-A)^{\circ}$$. Prove that for all
    $$A\subseteq X$$, $$X=A^{\circ}\cup \partial A\cup
         \mathrm{ext}(A)$$, and this union is disjoint.
-   Let $$X$$ be a totally ordered set with the order topology. Show
    that $$\overline{(a,b)}\subseteq [a,b]$$. Is equality always true?
-   Show that $$A'$$ is closed for any $$A\subseteq X$$.
