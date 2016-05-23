---
layout: post
title: Connectedness
date: 2015-04-26 11:00 
comments: true
published: true
categories: 
---

# Connected spaces

## Separations

1.  Separation

    Let $$X$$ be a topological space. A **separation** of $$X$$ is a pair
    of open sets $$U,V$$ such that:
    
    -   $$U\cap V=\emptyset$$,
    -   $$U\cup V=X$$,
    -   $$U\ne\emptyset$$, $$V\ne\emptyset$$

2.  Connected space

    A topological space is **connected** if it has no separation.

## Remark

1.  

    A space is connected if an only if the only subsets that are both
    open and closed are $$\emptyset$$ and $$X$$.

2.  

    This is because if $$U,V$$ form a separation, then both are open
    and closed. Conversely, if $$A\subseteq X$$ is not the empty set
    and not $$X$$, and is open and closed, then $$A,X-A$$ form a
    separation.

## Lemmas

1.  :B<sub>lemma</sub>:

    Let $$X$$ be a space and $$Y$$ a subspace of $$X$$. Then a
    separation of $$Y$$ is a pair of disjoint nonempty sets $$A,B$$ with
    union $$Y$$, and none containing a limit point of the other.

2.  
    -   Let $$A,B$$ be a separation of $$Y$$. Then both $$A,B$$ are open
        and closed in $$Y$$. We have that the closure of $$A$$ in $$Y$$
        is $$\overline{A}\cap Y$$, and since $$A$$ is closed, we have
        $$A=\overline{A}\cap Y$$. Since $$A,B$$ are disjoint, we have
        $$\overline{A}\cap B=\emptyset$$.
    -   Now, suppose $$A,B\subseteq Y$$ are disjoint, nonempty, and none
        containing a limit point of the other. Then $$\overline{A}\cap
              B=\emptyset$$, hence $$\overline{A}\cap Y=A$$. It follows that
        $$A$$ is closed in $$Y$$, hence $$B$$ is open in $$Y$$.

## Examples

-   If $$X$$ has the indiscrete topology, then $$X$$ is connected.
-   If $$X$$ is a space with only one point, then it is connected.
-   The subspace $$Y=[-1,0)\cup (0,1]$$ of $$\mathbb{R}$$ is not
    connected.
-   $$\mathbb{Q}$$ as a subspace of $$\mathbb{R}$$ is not connected.

## Properties of connected spaces

1.  :B<sub>lemma</sub>:

    If $$A,B$$ form a separation of $$X$$, and $$Y\subseteq X$$ is
    connected, then either $$Y\subseteq A$$ or $$Y\subseteq B$$.

2.  

    We have that $$Y\cap A,Y\cap B$$ are both open in $$Y$$, they
    are disjoint and its union is $$Y$$. Since $$Y$$ is connected they
    cannot be both nonempty, and if $$Y\cap A=\emptyset$$, then
    $$Y\subseteq B$$.

3.  :B<sub>lemma</sub>:

    The union of connected subspaces with a point in common is
    connected.

4.  

    Let $$X=\cup_{\alpha\in I}A_{\alpha}$$ with $$A_{\alpha}$$
    connected, and $$x_{0}\in\cap A_{\alpha}$$. Let $$U,V$$ be a
    separation of $$X$$. Suppose $$x_{0}\in U$$. By the previous
    lemma, we must have $$A_{\alpha}\subseteq U$$ for all $$\alpha\in
        I$$. But then $$V=\emptyset$$, which is a contradiction.

## More theorems

1.  Teorema

    Let $$A\subseteq X$$ be connected. Then if $$B\subseteq X$$ is
    such that $$A\subseteq B\subseteq\overline{A}$$, then $$B$$ is
    also connected.

2.  Proof

    Suppose that $$C,D$$ is a separation of $$B$$. By a previous
    lemma, we may assume without loss that $$A\subseteq C$$. But then
    $$\overline{A}\subseteq \overline{C}$$, and, since
    $$\overline{C}$$ and $$D$$ are disjoint and $$B\subseteq
        \overline{A}$$, we must have $$B\cap D=\emptyset$$, which is a
    contradiction. $$\square{}$$



1.  Teorema

    Let $$f\colon X\to Y$$ be a continuous map, with $$X$$
    connected. Then $$f(X)$$ is connected.

2.  Proof

    Let $$Z=f(X)$$, and consider the surjective map $$f\colon X\to
        Z$$, which is also continuous. Let $$A,B$$ be a separation of
    $$Z$$. Then $$f^{-1}(A),f^{-1}(B)$$ would form a separation of
    $$X$$, which is impossible. Therefore, there is no separation of
    $$Z$$, hence $$f(X)$$ is connected. $$\square{}$$



1.  Teorema

    The arbitrary product of connected spaces is connected.

2.  
    -   For the proof, we first prove that if $$X,Y$$ are connected,
        then $$X\times Y$$ is connected.
    -   Let $$(a,b)\in X\times Y$$. Then $$X\times\{b\}$$ and
        $$\{x\}\times Y$$ are connected, for all $$y\in Y$$.
    -   Hence $$T_{x}=(X\times\{b\})\cup (\{x\}\times Y)$$ is connected,
        since it is the union of two connected spaces with a point in
        common.
    -   Then, $$X\times Y=\cup_{x\in X}T_{x}$$ is the union of connected
        spaces with the point $$(a,b)$$ in common.
    -   By induction, we obtain that the product of any finite number of
        connected spaces is connected.



-   Now, let $$X_{\alpha}$$ be a connected space, for $$\alpha\in
          I$$. We want to prove that $$\prod_{\alpha}X_{\alpha}$$ is
    connected. Choose $$b=(b_{\alpha})\in X$$.
-   Given $$\{\alpha_{1},\ldots,\alpha_{n}\}\subseteq I$$, we define
    $$X(\alpha_{1},\ldots,\alpha_{n})$$ as the subspace of $$X$$
    with points such that $$x_{\alpha}=b_{\alpha}$$ for
    $$\alpha\not\in\{\alpha_{1},\ldots,\alpha_{n}\}$$.
-   We have that $$X(\alpha_{1},\ldots,\alpha_{n})$$ is homeomorphic
    to $$X_{\alpha_{1}}\times\cdots\times X_{\alpha_{n}}$$, and so
    it is connected.
-   Let $$Y$$ be the subspace of $$X$$ that is the union of all
    $$X(\alpha_{1},\ldots,\alpha_{n})$$, for
    $$\{\alpha_{1},\ldots,\alpha_{n}\}\subseteq I$$ finite. Then
    $$Y$$ is connected, as is the union of connected spaces with the
    point $$b$$ in common.
-   We finally prove that $$\overline{Y}=X$$. Let
    $$x=(x_{\alpha})\in X$$, and $$U=\prod U_{\alpha}$$ be a basis
    element of the product topology. We have that $$U=X_{\alpha}$$
    for all $$\alpha\in I-\{\alpha_{1},\ldots,\alpha_{n}\}$$.
-   Let $$y=(y_{\alpha})$$ defined as $$y_{\alpha}=x_{\alpha}$$ for
    $$\alpha\in\{\alpha_{1},\ldots,\alpha_{n}\}$$, and
    $$y_{\alpha}=b_{\alpha}$$ otherwise. Then $$y\in
          X(\alpha_{1},\ldots,\alpha_{n})$$, so $$Y\cap
          U\neq\emptyset$$. $$\square{}$$

# Connected subsets of $$\mathbb{R}$$

## Linear continuum

1.  :B<sub>definition</sub>:

    A totally ordered set $$L$$ is called a **linear continuum** if it
    satisfies the following:
    
    -   $$L$$ has the least upper bound property.
    -   If $$x<y$$, there is $$z$$ such that $$x<z<y$$.

2.  Teorema

    If $$L$$ is a linear continuum, then $$L$$ is connected in the
    order topology. (Hence, every interval and every ray in $$L$$ is
    connected.)

## Proof

-   We say that a subset $$Y\subseteq L$$ is **convex** if $$a,b\in Y$$
    with $$a<b$$ implies $$[a,b]\subseteq Y$$. We will prove that any
    convex subset $$Y$$ of $$L$$ is connected.
-   Suppose that $$Y=A\cup B$$, with $$A,B$$ open in $$Y$$, disjoint
    and nonempty. Let $$a\in A$$, $$b\in B$$, and assume that
    $$a<b$$.
-   Since $$Y$$ is convex, we have $$[a,b]\subseteq Y$$. Then
    $$[a,b]$$ is the union of the disjoint nonempty sets
    $$A_{0},B_{0}$$ given by:
    
    $$
    A_{0}=A\cap [a,b]\qquad B_{0}=B\cap [a,b]
    $$
-   Note that $$A_{0}$$, $$B_{0}$$ are open in $$[a,b]$$, and thus
    form a separation of $$[a,b]$$.
-   The interval $$[a,b]$$ is a subspace of $$L$$. Therefore the
    topology on $$[a,b]$$ is the order topology.
-   Let $$c=\sup A_{0}$$. Then $$c\in [a,b]$$.

## Proof (continuation)

-   Suppose $$c\in B_{0}$$. Given that $$c\ne a$$, we have that
    either $$c=b$$ or $$c\in (a,b)$$.
-   In any case, we have that there is $$d\in [a,b]$$ such that
    $$(d,c]\subseteq B_{0}$$.
-   Hence $$d$$ is an upper bound of $$A_{0}$$, which contradicts the
    choice of $$c$$.
-   Then $$c\in A_{0}$$. Given that $$c\ne b$$, we have that either
    $$c=a$$ or $$c\in (a,b)$$.
-   In any case, we have that there is $$d$$ such that
    $$[c,d)\subseteq A_{0}$$.
-   By Property 2 of linear continuum, there is $$z$$ such that
    $$c<z<d$$. But this contradicts that $$c$$ is upper bound of
    $$A_{0}$$. \qed

## Connected subsets of $$\mathbb{R}$$

1.  Corolario

    $$\mathbb{R}$$ is connected, and so is every interval and ray in
    $$\mathbb{R}$$. 

2.  Teorema

    If $$X$$ and $$Y$$ are linear continuum, and $$Y$$ is bounded
    above and below, then $$X\times Y$$ is a linear continuum with
    dictionary order. 

## Intermediate value theorem

1.  Teorema

    Let $$f\colon X\to Y$$ be a continuous map, where $$X$$ is
    connected and $$Y$$ is ordered and has the order topology. Suppose
    that $$a,b\in X$$ and $$y\in Y$$ are such that
    $$f(a)<y<f(b)$$. Then there is $$c\in X$$ such that $$f(c)=y$$.

# Path connectedness



1.  :B<sub>definition</sub>:
    -   A **path** on a space $$X$$ from $$x\in X$$ to $$y\in X$$ is a
        continuous function $$f\colon [a,b]\to X$$ from some interval
        $$[a,b]\subseteq \mathbb{R}$$, such that $$f(a)=x, f(b)=y$$.
    -   A space $$X$$ is **path-connected** if for every $$x,y\in X$$ there
        is a path from $$x$$ to $$y$$.

2.  Teorema

    If $$X$$ is path-connected, then it is connected.

3.  Examples

    The converse is not true, see $$[0,1]\times [0,1]$$ with
    dictionary order and the *deleted comb space*.
