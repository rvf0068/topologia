---
layout: post
title: Closed sets
date: 2016-02-08 9:00 -0500 
comments: true
published: true
categories: 
---

# Definition and properties

## Closed sets

1.  Closed sets

    Let $$X$$ be a space. We say that $$A$$ is *closed* if $$X-A$$ is open.

2.  Remark

    Unless we explicitly say otherwise, $$\mathbb{R}$$ will denote the
    space of the real numbers with usual topology.

3.  Examples
    -   Any interval of the form $$[a,b]\subseteq X$$, where $$X$$ has
        the order topology, is closed.
    -   The set $$[0,1)\subseteq \mathbb{R}$$ is not closed (nor open).
    -   In a discrete topology, any set is closed.
    -   In a cofinite topology on $$X$$, exactly $$X$$ and their finite
        subsets are closed.

## Properties of closed sets

1.  Properties of closed sets

    Let $$X$$ be a space. Then:
    
    -   **(C1):** $$\emptyset$$ and $$X$$ are closed.
    -   **(C2):** If $$A_{\alpha}$$ is closed for each $$\alpha\in I$$,
        then $$\cap_{\alpha\in I} A_{\alpha}$$ is closed.
    -   **(C3):** If $$A_1, A_2$$ are closed, then $$A_{1}\cup A_2$$ is
        closed.

2.  Proof

    Exercise.

3.  Remark

    We can prove that if a collection of subsets of $$X$$ satisfies the
    previous conditions, then their complements form a topology.

## Properties of closed sets

1.  Closed in subspaces

    Let $$Y$$ be a subspace of $$X$$. Then $$A\subseteq Y$$ is closed
    in $$Y$$ if and only if there is $$C\subseteq X$$ closed in $$X$$
    such that $$A=C\cap Y$$.

2.  Proof
    -   Let $$A$$ closed in $$Y$$. Then $$Y-A$$ is open in $$Y$$, so
        there is $$U$$ open in $$X$$ with $$Y-A=Y\cap U$$.
    -   We prove then that $$A=(X-U)\cap Y$$.
    -   The proof of the converse is an exercise. $$\Box$$

3.  Closed in closed

    Let $$Y$$ be a subspace of $$X$$. If $$Y$$ is closed in $$X$$ and
    $$A\subseteq Y$$ is closed in $$Y$$, then $$A$$ is closed in $$X$$.



## Links

-   [Closed set - Wikipedia, the free encyclopedia](https://en.wikipedia.org/wiki/Closed_set)



## Exercises

-   Is there a nondiscrete space where the open sets are the same as
    the closed sets?
-   Show that if $$A$$ is closed in $$X$$ and $$B$$ is closed in
    $$Y$$, then $$A\times B$$ is closed in $$X\times Y$$.
