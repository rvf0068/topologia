---
layout: post
title: Continuous functions
date: 2016-02-15 9:00 -0500 
comments: true
published: true
categories: 
---

# Definition, examples and properties



1.  Continuous functions

    Let $$X$$ and $$Y$$ be topological spaces. The function $$f\colon
        X\to Y$$ is *continuous* if for any open set $$V$$ in $$Y$$, we have
    that $$f^{-1}(V)$$ is open in $$X$$.
    
    {: .center}
![img]({{ site.baseurl }}ntinuous.png)



1.  Properties
    -   If the topology of $$Y$$ is given by a basis $$\mathcal{B}$$,
        then $$f\colon X\to Y$$ is continuous if and only if
        $$f^{-1}(V)$$ is open in $$X$$ for every $$V\in \mathcal{B}$$.
    -   If the topology of $$Y$$ is given by a subbasis $$\mathcal{S}$$,
        then $$f\colon X\to Y$$ is continuous if and only if
        $$f^{-1}(V)$$ is open in $$X$$ for every $$V\in \mathcal{S}$$.
    -   A function $$f\colon \mathbb{R}\to \mathbb{R}$$ is continuous if
        and only if for every $$x_{0}\in \mathbb{R}$$ and $$\epsilon>0$$,
        there is a $$\delta>0$$ such that $$\vert x-x_{0}\vert <\delta$$ implies
        $$\vert f(x)-f(x_{0})\vert <\epsilon$$.

## Examples

1.  Examples
    -   Any continuous function $$f\colon \mathbb{R}\to \mathbb{R}$$
        from calculus courses is continuous in this sense.
    -   Let $$\mathbb{R}_{l}$$ be the set of real numbers with
        the Sorgenfrey topology. Then the identity function
        $$1_{\mathbb{R}}\colon \mathbb{R}\to \mathbb{R}_{l}$$
        is not continuous.
    -   On the other hand, the identity $$1_{\mathbb{R}}\colon
              \mathbb{R}_{l}\to \mathbb{R}$$ is continuous.

## Equivalences of continuity

1.  Teorema

    Let $$X,Y$$ be topological spaces and $$f\colon X\to Y$$. Then the
    following are equivalent:
    
    -   $$f$$ is continuous.
    -   For every $$A\subseteq X$$, one has $$f(\overline{A})\subseteq \overline{f(A)}$$.
    -   For every closed set $$C$$ in $$Y$$, one has $$f^{-1}(C)$$ is
        closed in $$X$$.
    -   For each $$x\in X$$ and each neighborhood $$V$$ of $$f(x)$$,
        there is a neighborhood $$U$$ of $$x$$ such that $$f(U)\subseteq
              V$$.

2.  Proof

# Homeomorphisms



1.  Homeomorphism

    A bijective and continuous map $$f\colon X\to Y$$ is a
    *homeomorphism* if the inverse map $$f^{-1}\colon Y\to X$$ is also
    continuous 

2.  

    Equivalently, the continuous and bijective map $$f\colon X\to Y$$
    is a homeomorphism if and only if $$U\subseteq X$$ open implies
    that $$f(U)\subseteq Y$$ is open.

3.  Embedding

    If $$f\colon X\to Y$$ is injective and the bijection $$f\colon
        X\to f(X)$$ (where $$f(X)\subseteq Y$$ is a subspace) is a
    homeomorphism, we say that $$f$$ is an *embedding*.

# Constructing continuous functions

## Theorem

1.  Constructing continuous functions

    Let $$X,Y,Z$$ be topological spaces. 
    
    -   If $$f\colon X\to Y$$ is such that $$f(X)=\{y_0\}$$ for
        $$y_{0}\in Y$$, then $$f$$ is continuous.
    -   If $$A\subseteq X$$ is a subspace, the inclusion $$i_{A}\colon
              A\to X$$ is continuous.
    -   If $$f\colon X\to Y$$ and $$g\colon Y\to Z$$ are continuous,
        then the composition $$g\circ f$$ is continuous.



1.  Continuation
    -   If $$f\colon X\to Y$$ is continuous and $$A\subseteq X$$ is a
        subspace, the restriction $$f\mid_{A}\colon A\to Y$$ is
        continuous.
    -   If $$f\colon X\to Y$$ is continuous and $$Z\subseteq Y$$ is a
        subspace such that $$f(X)\subseteq Z$$, then $$f\mid \colon X\to Z$$
        is continuous. If $$Z$$ is a space containing $$Y$$ as a
        subspace, then $$f\colon X\to Z$$ is continuous.
    -   If $$X=\cup U_{\alpha}$$, where each $$U_{\alpha}$$ is open and
        $$f\mid_{U_{\alpha}}\colon U_{\alpha}\to Y$$ is continuous for
        each $$\alpha$$, then $$f$$ is continuous.

## Pasting lemma

1.  The pasting lemma

    Let $$X=A\cup B$$ be a space, with $$A,B$$ closed in $$X$$. Let
    $$f\colon A\to Y$$ and $$g\colon B\to Y$$ be continuous. Suppose
    that $$f(x)=g(x)$$ for every $$x\in A\cap B$$, and define
    $$h\colon X\to Y$$ by:
    
    $$
    h(x)=
    \begin{cases}
    f(x) & \text{if \(x\in A\)},\\
    g(x) & \text{if \(x\in B\)}.
    \end{cases}
    $$
    
    Then $$h$$ is continuous.

2.  Proof

## Maps into products

1.  Maps into products

    Let $$f\colon A\to X\times Y$$ be given by:
    
    $$
    f(a)=(f_{1}(a),f_{2}(a)). 
    $$
    
    Then $$f$$ is continuous if and only if the functions:
    
    $$
    f_1\colon A\to X,\quad f_2\colon A\to Y
    $$
    
    are continuous.

2.  Proof

# Exercises

## Exercises

1.  Let $$f\colon X\to Y$$ continuous. If $$A\subseteq X$$ and $$x$$
    is a limit point of $$A$$, is $$f(x)$$ a limit point of $$f(A)$$?
2.  If $$x_{0}\in X$$, show that the map $$f_{x_{0}}\colon Y\to
          X\times Y$$ given by $$f_{x_{0}}(y)=(x_{0},y)$$ is an embedding.
3.  Let $$a,b\in \mathbb{R}$$ with $$a<b$$. Show that $$(a,b)$$ is
    homeomorphic to $$(0,1)$$.
4.  Let $$Y$$ be an ordered set with the order topology, and
    $$f,g\colon X\to Y$$ be continuous. Show that:
    -   $$\{x\in X\mid f(x)\leq g(x)\}$$ is closed in $$X$$.
    -   the map $$h\colon X\to Y$$ given by $$h(x)=\min\{f(x),g(x)\}$$
        is continuous.
5.  Let $$f\colon A\to B$$ and $$g\colon C\to D$$ be continuous
    functions between topological spaces. Show that the map $$f\times
          g\colon A\times C\to B\times D$$ given by $$(a,c)\mapsto
          (f(a),f(c))$$ is continuous.
