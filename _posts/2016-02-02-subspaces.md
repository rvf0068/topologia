---
layout: post
title: The subspace topology
date: 2016-02-02 11:00 -0500 
comments: true
published: true
categories: 
---

# Subspace topology

## Definition

1.  Subspace topology

    Let $$(X,\tau)$$ be a topological space and $$Y\subseteq X$$. Then
    
    $$
    \tau_Y=\{Y\cap U\mid U\in \tau\}
    $$
    
    is a topology on $$Y$$, called **subspace topology**.

2.  Proof
    -   Since $$\emptyset=Y\cap\emptyset$$, and $$Y=Y\cap X$$, we have (T1).
    -   Let $$V_{\alpha}\in\tau_{Y}$$ for $$\alpha\in I$$. For each
        $$\alpha\in I$$, there is $$U_{\alpha}\in\tau$$ such that
        $$V_{\alpha}=Y\cap U_{\alpha}$$.
    -   Then:
        
        $$
        Y\cap (\cup U_{\alpha})=\cup (Y\cap U_{\alpha})=\cup V_{\alpha},
        $$
        
        and we obtain (T2). The proof of (T3) is an exercise.



1.  Open sets relative to $$Y$$

    If $$Y$$ is a subspace of $$X$$, and $$U\subseteq Y$$, it could be
    that $$U$$ is open in $$Y$$ but not open in $$X$$.

## Base of the subspace topology

1.  Lemma

    Let $$\mathcal{B}$$ be a base for the topology of $$X$$. Then
    
    $$
    \mathcal{B}_Y=\{Y\cap B\mid B\in \mathcal{B}\}    
    $$
    
    is a base for the subspace topology on $$Y$$.

2.  Proof

    Let $$U$$ be open in $$X$$ and $$y\in Y\cap U$$. Let $$B\in
        \mathcal{B}$$ such that $$y\in B\subseteq U$$. Then $$Y\cap B\in
        \mathcal{B}_{Y}$$, and $$y\in Y\cap B\subseteq Y\cap U$$. $$\Box$$

## Example

1.  Subspace of the real line
    -   Consider $$Y=[0,1]\subseteq X=\mathbb{R}$$, where $$X$$ has the
        standard topology.
    -   A base for the subspace topology on $$Y$$ is the collection of
        all sets of the form $$(a,b)\cap Y$$.
    -   They all are of one of the following forms: $$(a,b)$$,
        $$[0,b)$$, $$(a,1]$$, $$Y$$, $$\emptyset$$.
    -   We obtain that these elements generate the order topology on
        $$[0,1]$$.

## Example

1.  Subspace and order topology not always the same
    -   Consider now $$Y=[0,1)\cup\{2\}\subseteq X=\mathbb{R}$$.
    -   In the subspace topology, the set $$\{2\}$$ is open.
    -   But in the order topology on $$Y$$, considering that $$2$$ is $$\max
              Y$$, any open set that contains $$2$$ has to contain other points.

## Order topology in intervals

1.  Order topology in intervals

    If $$X$$ is an ordered set that has the order topology, and
    $$Y\subseteq X$$ is an interval, then the order topology and the
    subspace topology on $$Y$$ are the same.

2.  Proof

    Exercise



## Exercises

-   Show that if we consider in $$\mathbb{R}$$ the usual topology,
    then the topology on $$\mathbb{N}$$ as a subspace of
    $$\mathbb{R}$$ is discrete.
-   Let $$Y\subseteq X$$ be open. Show that $$A\subseteq Y$$ is open
    in Y if and only if it is open in $$X$$.
-   Let $$A\subseteq Y\subseteq X$$, where $$X$$ is a topological
    space. Show that the topology of $$A$$ as a subspace of $$X$$ is
    the same as $$(\tau_{Y})_{A}$$.
-   Show that if $$X$$ is a topological space, and $$A\subseteq
         Y\subseteq X$$, then the topology of $$A$$ as a subspace of $$Y$$
    is the same as a subspace of $$X$$ ($$Y$$ is a subspace of $$X$$).



## Links

-   [Subspace topology - Wikipedia, the free encyclopedia](http://en.wikipedia.org/wiki/Subspace_topology)
