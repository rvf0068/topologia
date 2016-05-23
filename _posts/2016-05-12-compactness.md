---
layout: post
title: Compact spaces
date: 2016-05-12 10:00 
comments: true
published: true
categories: 
---

# Definition

## Cover and compact

1.  Cover

    A collection $$\mathcal{O}$$ of open subsets of the topological
    space $$X$$ is called an **open cover** if $$\cup \mathcal{O}=X$$.

2.  Compact space

    A topological space $$X$$ is called **compact** if every open cover of
    $$X$$ has a finite subcollection that is also an open cover of
    $$X$$.

## Examples

1.  Examples
    -   The space $$\mathbb{R}$$ is not compact
    -   The subspace $$A=\{0\}\cup\{\frac{1}{n}\mid n\in \mathbb{N}\}$$
        of $$\mathbb{R}$$ is compact.
    -   Any finite topological space is compact.
    -   The subspace $$(0,1]\subseteq \mathbb{R}$$ is not compact.

# Compact subspaces

## Cover of subspace

1.  Cover of subspace

    Let $$Y\subseteq X$$. A collection $$\mathcal{O}$$
    of subsets of $$X$$ is said to **cover** $$Y$$ if $$Y\subseteq \cup \mathcal{O}$$.

2.  :B<sub>lemma</sub>:

    Let $$Y\subseteq X$$ be a subspace. Then $$Y$$ is compact if an
    only if every covering of $$Y$$ by open sets (in $$X$$) contains a
    finite subcollection covering $$Y$$.

## Proof

-   Assume that $$Y$$ is compact. Let $$\mathcal{O}=\{U_{\alpha}\}$$
    be a covering of $$Y$$, where each $$U_{\alpha}$$ is open in
    $$X$$.
-   Then $$\{U_{\alpha}\cap Y\}$$ is a cover of $$Y$$ by
    open sets in $$Y$$. By compactness of $$Y$$, we have that there
    is a finite subset $$\{U_{1},U_{2},\ldots,U_{r}\}\subseteq
         \mathcal{O}$$ such that
    
    $$
    Y= (U_{1}\cap Y)\cup\cdots\cup (U_{r}\cap Y).
    $$
-   It follows then that $$\{U_{i}\}\subseteq \mathcal{O}$$ is a
    finite open cover of $$Y$$.
-   Now, let $$\mathcal{O}'$$ be a cover of $$Y$$ by open sets in
    $$Y$$. For each $$U_{\alpha}'\in \mathcal{O}'$$, let
    $$U_{\alpha}$$ open in $$X$$ such that
    $$U_{\alpha}'=U_{\alpha}\cap Y$$. Then $$\{U_{\alpha}\}$$ covers $$Y$$.
-   Now, if $$\{U_{\alpha_{i}}\}_{i=1}^{r}$$ covers $$Y$$, we have
    that $$\{U'_{\alpha_{i}}\}_{i=1}^{r}\subseteq \mathcal{O}'$$
    covers $$Y$$ as well.

# Theorems



1.  Closed in compact

    Every closed subset of a compact space is compact.

2.  Proof
    -   Let $$Y\subseteq X$$ with $$Y$$ closed and $$X$$ compact. Let
        $$\mathcal{O}$$ be a cover of $$Y$$ by open sets in $$X$$.
    -   Then $$\mathcal{O}'=\mathcal{O}\cup\{X-Y\}$$ is an open cover of
        $$X$$. Since $$X$$ is compact, a finite subcollection
        $$\mathcal{F}\subseteq \mathcal{O}'$$ covers $$X$$.
    -   Then $$\mathcal{F}-\{X-Y\}$$ is a subcollection of
        $$\mathcal{O}$$ and is a finite subcover of $$Y$$. \qed



1.  Compact in Hausdorff

    Every compact subset of a Hausdorff space is closed.

2.  Proof
    -   Let $$Y\subseteq X$$ with $$Y$$ compact and $$X$$ Hausdorff. We
        will prove that $$X-Y$$ is open.
    -   Let $$x_{0}\in X-Y$$. For each $$y\in Y$$, let $$U_{y},V_{y}$$
        be disjoint neighborhoods of $$x_{0},y$$ respectively.
    -   Then $$\{V_{y}\}_{y\in Y}$$ is an open cover of $$Y$$. Choose
        $$y_{1},y_{2},\ldots,y_{r}\in Y$$ such that $$Y\subseteq
              V_{y_{1}}\cup\cdots\cup V_{y_{r}}$$.
    -   It follows that $$U_{y_{1}}\cap\cdots\cap U_{y_{r}}$$ is a
        neigborhood of $$x_{0}$$ that is disjoint from
        $$V_{y_{1}}\cup\cdots\cup V_{y_{r}}$$ and so is contained in
        $$X-Y$$. \qed

## A corollary

This statement follows from the proof of the previous theorem:

1.  Corollary

    If $$Y\subseteq X$$ is compact, where $$X$$ is Hausdorff, and
    $$x\not\in Y$$, there are disjoint open sets $$U,V$$ such that
    $$x\in U$$ and $$Y\subseteq V$$.

## Image of compact

1.  Teorema

    Let $$f\colon X\to Y$$ be continuous, with $$X$$ compact. Then
    $$f(X)$$ is compact.

2.  :B<sub>ignoreheading</sub>:
    -   Let $$\{V_{\alpha}\}$$ be an open cover of $$f(X)$$.
    -   Then $$\{f^{-1}(V_{\alpha})\}$$ is an open cover of $$X$$. Since
        $$X$$ is compact, there are $$\alpha_{1},\ldots,\alpha_{n}$$
        such that $$X\subseteq f^{-1}(V_{\alpha_{1}})\cup\cdots\cup
              f^{-1}(V_{\alpha_{n}})$$.
    -   It follows that $$f(X)\subseteq V_{\alpha_{1}}\cup\cdots\cup
              V_{\alpha_{n}}$$. $$\square$$



1.  Teorema

    Let $$f\colon X\to Y$$ be a continuous and biyective function,
    where $$X$$ is compact and $$Y$$ is Hausdorff. Then $$f$$ is a
    homeomorphism.

2.  :B<sub>ignoreheading</sub>:
    -   Since $$f$$ is continuous and biyective, in order to show that
        $$f$$ is a homeomorphism it is enough to show it is closed.
    -   Let $$C\subseteq X$$ be closed. Since $$X$$ is compact, we have
        that $$C$$ is compact.
    -   Since $$f$$ is continuous, we have that $$f(C)$$ is compact.
    -   Finally, since $$Y$$ is Hausdorff, we have that $$f(C)$$ is
        closed. $$\square$$



1.  Teorema

    If $$X$$ and $$Y$$ are compact spaces, then $$X\times Y$$ is
    compact.

2.  :B<sub>ignoreheading</sub>:
    -   First, we assume that we have spaces $$X,Y$$, with $$Y$$
        compact. Let $$x_{0}\in X$$ and $$N\subseteq X\times Y$$ open
        such that $$\{x_{0}\}\times Y\subseteq N$$. We will prove then
        that there is a neighborhood $$W$$ of $$x_{0}$$ such that
        $$W\times Y\subseteq N$$.
    -   For each $$y\in Y$$, since $$(x_{0},y)\in N$$, which is open in
        $$X\times Y$$, there is a basis element $$U_{y}\times
              V_{y}\subseteq N$$ containing $$(x_{0},y)$$. The collection
        $$\{U_{y}\times V_{y}\}$$ covers the compact set
        $$\{x_{0}\}\times Y$$, and so we can cover it with finitely many
        such basis elements: $$U_{1}\times V_{1},\ldots,U_{n}\times V_{n}$$.
    -   Let $$W=U_{1}\cap\cdots\cap U_{n}$$. Then $$W$$ is a
        neighborhood of $$x_{0}$$. We prove the finite subcover also
        cover the *tube* $$W\times Y$$.
    -   Let $$(x,y)\in W\times Y$$. Then $$(x_{0},y)\in U_{j}\times
              V_{j}$$ for some $$j$$. Since $$x\in W$$ implies $$x\in U_{j}$$,
        it follows that $$(x,y)\in U_{j}\times V_{j}$$, and so $$W\times
              Y\subseteq N$$.



-   We now assume $$X,Y$$ are compact spaces, and let $$\mathcal{O}$$
    be an open cover of $$X\times Y$$.
-   Given $$x\in X$$, since $$\{x\}\times Y$$ is compact and is
    covered by $$\mathcal{O}$$, it can also be covered by finitely
    many $$U_{1},\ldots, U_{n}$$ elements of $$\mathcal{O}$$. Let
    $$N=U_{1}\cup\cdots\cup U_{n}$$.
-   By the *tube lemma*, there is a neighborhood $$W_{x}$$ of $$x$$
    such that $$W\times Y\subseteq N$$. Then the collection
    $$\{W_{x}\}$$ covers $$X$$. Since $$X$$ is compact, there is a
    finite subcollection $$W_{1},\ldots,W_{m}$$ covering $$X$$.
-   Finally, since the finite collection of tubes $$W_{1}\times
         Y,\ldots,W_{m}\times Y$$ covers $$X\times Y$$, and each tube can
    be covered by a finite subcollection of $$\mathcal{O}$$, we are
    done. $$\square$$

## Property of finite intersection

1.  Finite intersection property

    Let $$\mathcal{C}$$ be a collection of subsets of $$X$$. We say
    that $$\mathcal{C}$$ has the **finite intersection property** if for
    every finite subcolection $$\{F_{1},\ldots,F_{r}\}\subseteq
        \mathcal{C}$$ we have that $$F_{1}\cap\cdots\cap F_{r}\ne\emptyset$$.

2.  Teorema

    A topological space $$X$$ is compact if an only if for every
    collection of closed sets $$\mathcal{C}$$ that has the finite
    intersection property, we have that $$\cap\mathcal{C}\ne\emptyset$$.

3.  :B<sub>ignoreheading</sub>:
    -   Given a collection $$\mathcal{O}$$ of subsets of $$X$$, define
        the collection $$\mathcal{C}=\{X-U\mid U\in
              \mathcal{O}\}$$. Then we have:
        -   $$\mathcal{O}$$ is a collection of open sets if and only if
            $$\mathcal{C}$$ is a collection of closed sets.
        -   $$\mathcal{O}$$ is a cover of $$X$$ if and only if $$\cap
                    \mathcal{C}=\emptyset$$.
        -   The finite subcolection $$\{U_{1},\ldots,U_{n}\}\subseteq
                    \mathcal{O}$$ covers $$X$$ if and only if the intersection of
            the corresponding $$X-U_{i}$$ is empty.

# Compact ordered sets

## Closed intervals on ordered sets

1.  Teorema

    Let $$X$$ be a totally ordered set with the least upper bound
    property (every non-empty subset that has an upper bound has a
    least upper bound). Then, in the ordered topology, every closed
    interval in $$X$$ is compact.

2.  :B<sub>ignoreheading</sub>:
    -   Let $$a,b\in X$$, $$a<b$$, and let $$\mathcal{O}$$ be a covering
        of $$[a,b]$$ by sets open in $$[a,b]$$ with respect to the
        subspace topology (which is the same as the order topology on
        $$[a,b]$$). We wish to prove there is a finite subcover of
        $$\mathcal{O}$$.
    -   We prove first that if $$x\in [a,b]$$, $$x\ne b$$, then there is
        a point $$y\in [a,b]$$, $$y>x$$, such that the inverval
        $$[x,y]$$ can be covered by at most two elements of
        $$\mathcal{O}$$.
    -   If $$x$$ has an immediate successor $$y\in X$$, then $$y\in
              [a,b]$$ and $$[x,y]=\{x,y\}$$



1.  Corollary

    Every closed interval in $$\mathbb{R}$$ is compact.

2.  Teorema

    A subset $$A\subseteq \mathbb{R}^{n}$$ is compact if and only if
    is closed and bounded in the euclidian metric $$d$$, or in the
    metric $$\rho$$. ($$\rho(x,y)=\max \vert x_{i}-y_{i}\vert $$)

## Maximum value theorem

1.  Maximum value theorem

    Let $$f\colon X\to Y$$ be continuous, where $$Y$$ is a totally
    ordered set with the order topology. If $$X$$ is compact, there
    are points $$c,d\in X$$ such that $$f(c)\leq f(x)\leq f(d)$$ for
    every $$x\in X$$.

## The reals are uncountable

1.  Teorema

    Let $$X$$ be a non-empty compact Hausdorff space. If every point
    of $$X$$ is a limit point of $$X$$, then $$X$$ is uncountable.

2.  Corollary

    Every closed interval in $$\mathbb{R}$$ is uncountable.
