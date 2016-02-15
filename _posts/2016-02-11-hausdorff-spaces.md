---
layout: post
title: Hausdorff spaces
date: 2016-02-11 9:00 -0500 
comments: true
published: true
categories: 
---

# Hausdorff spaces

## Definition

1.  Hausdorff space

    We say that the space $$X$$ is **Hausdorff** if for any $$x,y\in X$$
    such that $$x\ne y$$, there are disjoint neigborhoods $$U,V$$ of
    $$x,y$$, respectively.

2.  Examples
    -   If $$d$$ is a metric on $$X$$, $$(X,\tau_{d})$$ is Hausdorff.
    -   Any totally ordered set with the order topology is Hausdorff.
    -   The product of two Hausdorff spaces is Hausdorff.
    -   Any subspace of a Hausdorff space is Hausdorff.
    -   The Sierpiński space is not Hausdorff.
    -   Is the cofinite topology on $$\mathbb{N}$$ Hausdorff?

## Properties of Hausdorff spaces

1.  Points in Hausdorff

    Every singleton in a Hausdorff space $$X$$ is a closed set.

2.  Proof

    For $$x\in X$$, let $$y\not\in\{x\}$$. If $$U,V$$ are disjoint
    neigborhoods of $$x,y$$ respectively, then $$V\subseteq
        X-\{x\}$$. Hence $$X-\{x\}$$ is open.

3.  Limit points in Hausdorff

    Let $$X$$ be a Hausdorff space and $$A\subseteq X$$. Then $$x\in X$$ is
    a limit point of $$A$$ if and only if every neigborhood of $$x$$
    contains infinitely many points of $$A$$.

4.  Proof

# Exercises

## Exercises

-   We say that a space is a **$$T_{1}$$ space** if for any two
    different points $$x,y$$, each has a neighborhood that does not
    contain the other point. Show that all singletons are closed in
    $$X$$ if and only if $$X$$ is $$T_{1}$$.

-   Show that If $$X$$ is Hausdorff, then $$X$$ is $$T_{1}$$. Give an
    example of a $$T_{1}$$ space that is not Hausdorff.

-   We say that a space is a **$$T_{0}$$ space** if for any two
    different points $$x,y$$, one of them has a neighborhood that does not
    contain the other point. Show that a $$T_{1}$$ space is
    $$T_{0}$$. Give an example of a $$T_{0}$$ space that is not
    $$T_{1}$$. Give an example of a space that is not $$T_{0}$$.



## Links

-   [Hausdorff space - Wikipedia, the free encyclopedia](https://en.wikipedia.org/wiki/Hausdorff_space)
