---
layout: post
title: Topological spaces
date: 2016-01-25 9:00 -0500 
comments: true
published: true
categories: 
---

# Notation



-   **$$X$$:** a set
-   **$$P(X)$$:** the **power set** of $$X$$, that is, the set of all
    subsets of $$X$$.
-   **$$\mathbb{R}$$:** the set of real numbers.

# Topological spaces

## Definitions

1.  Topology

    A *topology* on $$X$$ is a subset
    $$\tau\subseteq P(X)$$, such that:
    
    -   **(T1):** $$\emptyset,X\in\tau$$.
    -   **(T2):** If $$U_{\alpha}\in\tau$$ for all $$\alpha\in I$$, then
        $$\cup_{\alpha}U_{\alpha}\in\tau$$.
    -   **(T3):** If $$U_{1},U_{2}\in\tau$$, then $$U_{1}\cap U_{2}\in\tau$$.

2.  Topological spaces

    1.  If $$\tau$$ is a topology on $$X$$, the pair $$(X,\tau)$$ is
        called a *topological space*.
    2.  The elements of $$\tau$$ are called *open sets*.

## Examples

-   Let $$X$$ be any set. Then $$\tau_{d}=P(X)$$ is a topology,
    called the *discrete topology*.

-   Let $$X$$ be any set. Then $$\tau_{i}=\{\emptyset,X\}$$ is a
    topology, called the *indiscrete topology*.

-   Let $$X=\{1,2\}$$. Then $$\tau=\{\emptyset,X,\{1\}\}$$ is a
    topology, and $$(X,\tau)$$ is called the *Sierpiński space*.

## More examples

-   Let 
    -   $$X=\mathbb{R}$$,
    -   $$\tau=\{U\subseteq X\mid \forall x\in U\,\exists\epsilon>0,
              \text{such that } (x-\epsilon,x+\epsilon)\subseteq U\}$$.
    -   Then  $$\tau$$ is called the *usual topology* on $$\mathbb{R}$$.

-   Let
    -   $$(X,d)$$ be any metric space. For $$x\in X$$, let
        $$B_{\epsilon}(x)=\{y\in X\mid d(x,y)<\epsilon\}$$.
    -   $$\tau=\{U\subseteq X\mid \forall x\in U\,\exists\epsilon>0,
              \text{such that } B_{\epsilon}(x)\subseteq U\}$$.
    -   Then $$\tau$$ is called the *metric topology* on $$X$$.

## Cofinite topology

1.  Cofinite topology

    Let $$\tau=\{U\subseteq X\mid X-U \text{ is
        finite}\}\cup\{\emptyset\}$$. Then $$\tau$$ is a topology on $$X$$.

2.  Sketch of proof
    -   $$\emptyset\in\tau$$ immediately. $$X\in\tau$$ because
        $$X-X=\emptyset$$ is finite.
    -   Let $$U_{\alpha}\in\tau$$ for all $$\alpha\in I$$. We need to
        show that either $$\cup_{\alpha}U_{\alpha}$$ is empty or
        $$X-\cup_{\alpha}U_{\alpha}$$ is finite.
    -   Let $$U_{1},U_{2}\in\tau$$. We need to show that either
        $$U_{1}\cap U_{2}$$ is empty or $$X-(U_{1}\cap U_{2})$$ is
        finite.



## Exercises

1.  Show that if $$X$$ is any set, there is a metric on $$X$$ such
    that the metric topology is the same as the discrete topology.
2.  Show that in general there is no metric on $$X$$ such that the
    metric topology is the same as the indiscrete topology.
3.  Show that if $$\tau$$ is any topology on $$X$$, then
    $$\tau_{i}\subseteq\tau\subseteq\tau_{d}$$.
4.  Show that if $$\tau_{\alpha}$$ is a topology on $$X$$ for each
    $$\alpha\in I$$, then $$\tau=\cap\tau_{\alpha}$$ is a topology
    on $$X$$.
5.  Give an example of a set $$X$$ and topologies
    $$\tau_{1},\tau_{2}$$ such that $$\tau_{1}\cup\tau_{2}$$ is not
    a topology on $$X$$.
6.  Let $$\tau=\{(a,\infty)\mid a\in
          \mathbb{R}\}\cup\{\mathbb{R},\emptyset\}$$. Prove that $$\tau$$
          is a topology on $$\mathbb{R}$$.
7.  Let $$a\in X$$, and $$\tau_{a}=\{U\subseteq X\mid a\in
          X\}\cup\{\emptyset\}$$. Prove that $$\tau_{a}$$ is a topology on
    $$X$$.
8.  Let $$a\in X$$, and $$\rho_{a}=\{U\subseteq X\mid a\not\in
          X\}\cup\{X\}$$. Is $$\rho_{a}$$ a topology on $$X$$?
9.  Let $$X=\{1,2,3\}$$. Enumerate all topologies on $$X$$.



## Links

-   [Topological space - Wikipedia, the free encyclopedia](http://en.wikipedia.org/wiki/Topological_space)
-   [How to get intuition in topology concerning the definitions? - Mathematics Stack Exchange](http://math.stackexchange.com/questions/1598409/)
-   [Why is a topology made up of 'open' sets? - MathOverflow](http://mathoverflow.net/questions/19152/why-is-a-topology-made-up-of-open-sets)
-   [Why does topology rarely come up outside of topology? - Mathematics Stack Exchange](http://math.stackexchange.com/questions/1592421/why-does-topology-rarely-come-up-outside-of-topology)
