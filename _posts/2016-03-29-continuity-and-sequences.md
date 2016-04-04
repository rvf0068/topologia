---
layout: post
title: Continuity and sequences in metric spaces
date: 2016-03-29 11:00 -0500 
comments: true
published: true
categories: 
---

# Subspaces and products

## Properties

-   If $$X$$ is metrizable and $$Y$$ is a subspace of $$X$$, then
    $$Y$$ is metrizable.
-   If $$X$$ is metrizable, then $$X$$ is Hausdorff.
-   If $$(X_{i})_{i\in I}$$ is a countable family of metrizable
    spaces, then $$\prod_{i\in I} X_{i}$$ is metrizable.

## Continuous functions

1.  $$\epsilon$$ - $$\delta$$ definition

    Let $$f\colon X\to Y$$ a function, with $$X$$, $$Y$$ metrizable
    spaces with metrics
    $$d_{X}$$, $$d_{Y}$$, respectively. Then $$f$$ is continuous
    if and only if  for all $$x\in X$$, $$\epsilon>0$$ there is
    $$\delta>0$$ such that
    
    $$
      d_{Y}(f(x),f(y))<\epsilon \text{ if } d_{X}(x,y)<\delta
    $$

# Sequences

## Definition

1.  Sequence

    If $$X$$ is a topological space, a **sequence** on $$X$$ is a
    function $$\mathbb{N}\to X$$. 

2.  Notation

    We denote a sequence $$(x_n)$$ or $$(x_1,x_2,\ldots)$$.

3.  Convergence

    We say that the sequence $$(x_n)$$ **converges to** $$x\in X$$ if for
    every neighborhood $$U$$ of $$x$$ there is a positive integer $$N$$ such
    that $$x_n\in U$$ for all $$n\geq N$$. We write $$x_n\to x$$.

## Remarks on the definition of convergence

-   A sequence does not necessarily converges, and if it does, the
    limit is not necessarily unique.
-   If $$X$$ is Hausdorff, a sequence on $$X$$ that converges has a
    unique limit.

## Sequence lemma

1.  Sequence lemma

    Let $$X$$ be a topological space, and $$A\subseteq X$$. If
    $$(x_n)$$ is a sequence in $$A$$ that converges to $$x$$, then
    $$x\in\overline{A}$$.
    
    Conversely, if $$x\in\overline{A}$$ and **$$X$$ es metrizable**, then
    there is a sequence on $$A$$ that converges to $$x$$

## Proof of the sequence lemma

1.  Proof
    -   Suppose that $$x_n\to x$$, where $$x_{n}\in A$$ for all
        $$n$$. Let $$U$$ be a neighborhood of $$x$$. By definition of
        convergence, $$x_n\in U$$ for big enough values
        of $$n$$, and so $$x\in\overline{A}$$.
    
    -   Now, let $$X$$ be metrizable with metric $$d$$, and let
        $$x\in\overline{A}$$. For each $$n$$, we choose a point
        $$x_{n}\in A\cap B(x,\frac{1}{n})$$.
    
    -   We claim that $$x_n\to x$$. Because if $$U$$ is a neighborhood
        of $$x$$, let $$\epsilon>0$$ be such that
        $$B(x,\epsilon)\subseteq U$$, and let $$N>\frac{1}{\epsilon}$$.
    
    -   Then, if $$n\geq N$$, we have that $$\frac{1}{n}\leq
              \frac{1}{N}<\epsilon$$, and so $$x_{n}\in U$$ si $$n\geq N$$.

## Remarks to the proof

-   The theorem gives a necessary condition for metrizability. We
    will see examples of $$A\subseteq X$$, $$x\in X$$ with
    $$x\in\overline{A}$$ such that there is no sequence in $$A$$ that
    converges to $$x$$. In such cases, $$X$$ is not metrizable.
-   In the proof of the reciprocal, we do not need the full
    hypothesis of metrizability, but the properties of the collection
    of balls $$\{B(x,\frac{1}{n})\}_{n\in\mathbb{N}}$$.
-   A **countable local base on $$x\in X$$** is a collection
    $$\{B_{n}\}_{n\in\mathbb{N}}$$ of neighborhoods of $$x$$ such
    that for any neighborhood $$U$$ of $$x$$ there is $$n$$ such that
    $$B_{n}\subseteq U$$.
-   The topological space $$X$$ is **first&#x2013;countable** if every $$x\in X$$
    has a countable local base.
-   (Exercise) Prove that if $$X$$ es first&#x2013;countable, $$A\subseteq X$$
    and $$x\in\overline{A}$$, there is a sequence $$(x_n)$$ on $$A$$
    that converges to $$x$$.

## Continuity and sequences

1.  Continuity by sequences

    Let $$f\colon X\to Y$$ with $$X$$ metrizable. Then $$f$$ is
    continuous if and only if for all convergent sequences $$x_{n}\to
        x$$ on $$X$$, the sequence $$f(x_n)$$ converges to $$f(x)$$.

2.  Proof
    -   Suppose $$f$$ continuous and let $$x_n\to x$$. We want to prove
        $$f(x_{n})\to f(x)$$. Let $$V$$ be a neighborhood of
        $$f(x)$$. Then $$f^{-1}(V)$$ is a neighborhood of $$x$$, and so
        there is $$N$$ such that $$x_{n}\in f^{-1}(V)$$ if $$n\geq
              N$$. But then $$f(x_{n})\in V$$ for such values of $$n$$.

## Continuation of the proof

1.  Continuation of the proof
    -   For the converse, suppose that for any convergent sequence
        $$x_{n}\to x$$ in $$X$$, the sequence $$f(x_n)$$ converges to
        $$f(x)$$. We want to prove that $$f$$ is continuous.
    -   Let $$A\subseteq X$$, we want to see that
        $$f(\overline{A})\subseteq \overline{f(A)}$$.
    -   Let $$x\in\overline{A}$$. Since $$X$$ is metrizable, there is a 
        sequence $$x_n$$ on $$A$$ such that $$x_{n}\to x$$.
    -   By hypothesis, we have that $$f(x_{n})\to f(x)$$. Since
        $$f(x_{n})\in f(A)$$, then $$f(x)\in\overline{f(A)}$$. Hence
        $$f(\overline{A})\subseteq \overline{f(A)}$$.

# Examples

## Box topology on $$\mathbb{R}^{\mathbb{N}}$$

-   We will see that the sequence lemma does not hold in
    $$X=\mathbb{R}^{\mathbb{N}}$$ with the box topology.
-   Let $$A$$ be the set of all real sequences where the terms are all
    positive:
    
    $$
      A=\{(x_1,x_2,\ldots)\mid x_i>0\text{ for all \(i\)}\}
    $$
-   Let $$0=(0,0,\ldots)\in X$$. Then $$0\in\overline{A}$$, since if 
    
    $$
      B=(a_1,b_1)\times(a_2,b_2)\times\cdots
    $$
    
    is a basic subset that contains $$0$$, then $$B\cap A\ne\emptyset$$.

## Continuation

-   However, there is no sequence on $$A$$ that converges to $$0$$. 
    Suppose that $$(a_n)$$ is a sequence on $$A$$. Let
    
    $$
      a_{n}=(x_{1n},x_{2n},\ldots,x_{in},\ldots)
    $$

-   Since each $$x_{in}$$ is greater than zero, the basic subset of
    $$X$$:
    
    $$
      B'=(-x_{11},x_{11})\times(-x_{22},x_{22})\times\cdots
    $$
    
    is a neighborhood of $$0\in X$$.
-   However, $$B'$$ does not contain points of the sequence
    $$(a_n)$$. Hence $$(a_n)$$ does not converge to $$0$$.

## Uncountable product of copies of $$\mathbb{R}$$

-   Let $$J$$ be uncountable. We show that $$\mathbb{R}^{J}$$ with
    product topology is not metrizable.
-   Let $$A\subseteq \mathbb{R}^{J}$$, where $$A$$ consists of the
    $$(x_{\alpha})$$ such that $$x_{\alpha}=1$$ for all but a finite
    number of $$\alpha\in J$$, where we have $$x_{\alpha}=0$$. Let
    $$0$$ denote the "origin" of $$\mathbb{R}^{J}$$.
-   We prove that $$0\in \overline{A}$$. Let $$\prod U_{\alpha}$$ be
    a basis element such that $$0\in \prod U_{\alpha}$$. Suppose
    $$U_{\alpha}\ne \mathbb{R}$$ for
    $$\alpha\in\{\alpha_{1},\ldots,\alpha_{n}\}$$.
-   Then, if $$(x_{\alpha})$$ is defined as $$x_{\alpha}=0$$ for
    $$\alpha\in\{\alpha_{1},\ldots,\alpha_{n}\}$$ and
    $$x_{\alpha}=1$$ for all other values of $$\alpha$$, we have that
    $$(x_{\alpha})\in A\cap \prod U_{\alpha}$$.
-   We will show then that there is no sequence of points in $$A$$
    that converges to $$0$$. Let $$(a_{n})$$ a sequence in $$A$$.

## Continuation

-   Each $$a_{n}\in A$$ has only a finite number of values of
    $$\alpha$$ such that the $$\alpha$$th term of $$a_{n}$$ is equal to
    $$0$$. Let $$J_{n}$$ be the set of such values of $$\alpha$$.
-   The union of all the $$J_{n}$$ is a countable union of finite
    sets, hence countable. Since $$J$$ is uncountable, let $$\beta\in
         J$$ that is not in any of the $$J_{n}$$. That means that the
    $$\beta$$th coordinate of all of the $$a_{n}$$ is 1.
-   Let $$U_{\beta}=(-1,1)$$, and let
    $$U=\pi_{\beta}^{-1}(U_{\beta})$$. Then $$U$$ is a neighborhood
    of $$0\in \mathbb{R}^{J}$$, and $$U$$ does not contain any of the
    $$a_{n}$$. Hence $$a_{n}$$ does not converge to $$0$$.

# Well-ordered sets

## Definition and examples

1.  Well-orderet set

    We say that the totally ordered set $$(X,\leq)$$ is **well-ordered**
    if every nonempty subset has a minimum element.

2.  Examples
    -   The set $$\mathbb{N}$$ with the usual order is well-ordered.
    -   The set $$\mathbb{R}$$ with the usual order is not well-ordered.

## Properties

1.  Properties of well-ordered sets
    -   If $$X$$ is well-ordered and $$Y\subseteq X$$ has the induced
        order, then $$Y$$ is well-ordered.
    -   If $$X,Y$$ are well-ordered sets, then $$X\times Y$$ with
        dictionary order is well-ordered.

## Zermelo's theorem

1.  Zermelo

    If $$A$$ is any set, there is a total order $$\leq$$ on $$A$$ that
    is a well-order.

2.  Corolario

    There is a set that is uncountable and well-ordered.

## Sections

1.  Section

    If $$S$$ is an ordered set and $$\alpha\in S$$, we denote by
    $$S_{\alpha}$$ the set:
    
    $$
      S_{\alpha}=\{x\in S\mid x<\alpha\}.
    $$
    
    $$S_{\alpha}$$ is called the **section of $$S$$ by $$\alpha$$**.

# The example



1.  Teorema

    There is a set that is uncountable and well-ordered, but every
    section of it is countable.

2.  Proof
    -   Let $$X$$ be an uncountable, well-ordered set. Then the set
        $$S=\{1,2\}\times X$$ is also uncountable and well-ordered, and
        has sections that are uncountable (for example, those of
        elements of the form $$(2,x)$$.)
    -   The set 
        
        $$
          \{\alpha\in S\mid \text{\(S_{\alpha}\) is uncountable}\}
        $$
        
        is nonempty, let $$\Omega$$ its smallest element.
    -   Then $$S_{\Omega}$$ is the required set.

## A corollary

1.  Corolario

    If $$A\subseteq S_{\Omega}$$ is countable, then $$A$$ has an upper
    bound in $$S_{\Omega}$$.

2.  Proof
    -   Since for each $$a\in A$$, we have that $$S_{a}$$ is countable,
        then $$B=\cup_{a\in A}S_{a}$$ is also countable.
    -   Since $$B\subseteq S_{\Omega}$$, and $$S_{\Omega}$$ is
        uncountable, we can choose $$x\in S_{\Omega}-B$$.
    -   If there was $$a\in A$$ with $$x<a$$, then $$x$$ would be in
        $$B$$, which is a contradiction.
    -   Hence $$x$$ is an upper bound of $$A$$.\qed



1.  A nonmetrizable ordered space

    The set $$S_{\Omega}\cup\{\Omega\}$$ is not metrizable

2.  Proof
    -   We have that $$\Omega$$ is a limit point of $$S_{\Omega}$$,
        since any basic element containing $$\Omega$$ has the form
        $$(a,\Omega]$$ and must intersect $$S_{\Omega}$$. Otherwise we
        would have $$S_{\Omega}=S_{a}\cup\{a\}$$, but $$S_{a}\cup\{a\}$$
        is countable.
    -   However, there is no sequence in $$S_{\Omega}$$ that converges
        to $$\Omega$$, since if $$(x_{n})$$ is a sequence in
        $$S_{\Omega}$$, there is an upper bound $$b\in S_{\Omega}$$ for
        all the terms in the sequence. Then $$(b,\Omega]$$ contains no
        point of the sequence.\qed

3.  

    We will denote with $$\overline{S_{\Omega}}$$ the set
    $$S_{\Omega}\cup\{\Omega\}$$.
