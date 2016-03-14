---
layout: post
title: Arbitrary products
date: 2016-03-06 09:00 -0500 
comments: true
published: true
categories: 
---

# Topologies on the product

## Products

1.  Arbitrary Cartesian product as set

    Let $$X_{\alpha}$$ be a topological space for each $$\alpha\in
        I$$. The *Cartesian product* of the sets $$X_{\alpha}$$ is denoted as:
    \[
        \prod_{\alpha\in I}X_{\alpha}
        \]
    and consists of all maps $$f\colon I\to \cup_{\alpha}X_{\alpha}$$
    such that $$f(\alpha)\in X_{\alpha}$$. If
    $$f(\alpha)=x_{\alpha}$$, we denote $$f$$ as $$(x_{\alpha})_{\alpha}$$.



1.  Projections

    For each $$\alpha_{0}\in I$$, there is a *projection map* 
    \[
        p_{\alpha_{0}}\colon\prod_{\alpha\in I}X_{\alpha}\to X_{\alpha_{0}},
        \]
    given by $$p_{\alpha_{0}}((x_{\alpha})_{\alpha})=x_{\alpha_{0}}$$.

## Box topology

1.  

    Let $$X_{\alpha}$$ a topological space for each $$\alpha\in
        I$$, and $$X$$ the product $$\prod X_{\alpha}$$.

2.  Box topology

    The collection of all subsets of $$X$$ of the form
    \[
        \prod_{\alpha\in I} U_{\alpha},
        \]
    where $$U_{\alpha}$$ is open in $$X_{\alpha}$$ for all $$\alpha\in
        I$$, is a basis for a topology on $$X$$, called the *box topology*.

## Product topology

1.  Product topology

    The collection
    \[
        \mathcal{S}=\cup_{\alpha\in I}\{p^{-1}_{\alpha}(U_{\alpha})\mid
        U_{\alpha}\text{ open in } X_{\alpha}\}
        \]
    is a subbasis for a topology on $$X$$, called the *product topology*.



1.  Remark

    The product topology has as basis the subsets of $$X=\prod
        X_{\alpha}$$ of the form 
    \[
        \prod_{\alpha\in I} U_{\alpha},
        \]
    where $$U_{\alpha}$$ is open in $$X_{\alpha}$$ for all $$\alpha\in
        I$$, and $$U_{\alpha}=X_{\alpha}$$ for all but finitely many
    values of $$\alpha\in I$$

## Continuous functions into the product

1.  Teorema

    Let $$f\colon A\to\prod_{\alpha\in I}X_{\alpha} $$ be given by:
    \[
        f(a)=(f_{\alpha}(a))_{\alpha\in I},
        \]
    where $$f_{\alpha}\colon A\to X_{\alpha}$$ for each
    $$\alpha$$. Suppose that $$\prod X_{\alpha}$$ has the product
    topology. Then $$f$$ is continuous if and only if each
    $$f_{\alpha}$$ is continuous.

2.  Remark

    The last theorem is not true if we use the box topology on the
    Cartesian product

# Exercises

## Exercises

1.  Let $$X_{\alpha}$$ be a topological space for each $$\alpha\in
          I$$, and $$A_{\alpha}\subseteq X_{\alpha}$$.
    -   Show that if $$A_{\alpha}\subseteq X_{\alpha}$$ is closed,
        then $$\prod A_{\alpha}$$ is closed in $$\prod X_{\alpha}$$.
    -   Show that
        
        $$
        \overline{\prod A_{\alpha}}=\prod \overline{A_{\alpha}}.
        $$
    -   Which of the last two are true if we use the box topology?
2.  We say that the sequence $$x_{n}$$ of points in $$X$$ **converges**
    to $$x\in X$$ if for any neighborhood $$U$$ of $$x$$ there is
    $$N$$ such that $$n\geq N$$ implies $$x_{n}\in U$$. Show that a
    sequence $$x_{n}$$ in $$\prod_{\alpha\in I} X_{\alpha}$$
    converges to $$(x_{\alpha})$$ if and only if
    $$\pi_{\alpha}(x_{n})$$ converges to $$x_{\alpha}$$ for each
    $$\alpha\in I$$.
