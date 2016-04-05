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
        X\to Y$$ is **continuous** if for any open set $$V$$ in $$Y$$, we have
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

2.  
    -   Let $$f\colon \mathbb{R}\to \mathbb{R}$$ be continuous,
        $$x_{0}\in \mathbb{R}$$ and $$\epsilon>0$$.
    -   We have that $$f^{-1}((f(x_{0})-\epsilon,f(x_{0})+\epsilon))$$ is
        open in $$\mathbb{R}$$ and contains $$x_{0}$$. Hence there is
        $$\delta>0$$ such that $$(x_{0}-\delta,x_{0}+\delta)\subseteq
              f^{-1}(f(x_{0})-\epsilon,f(x_{0})+\epsilon)$$.

## Examples

1.  Continuous functions
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

2.  

    When the last condition is satisfied at $$x_{0}\in X$$, we say
    that $$f$$ is **continuous at $$x_{0}$$**.



## Exercises

1.  Let $$f\colon X\to Y$$ continuous. If $$A\subseteq X$$ and $$x$$
    is a limit point of $$A$$, is $$f(x)$$ a limit point of $$f(A)$$?
2.  If the singleton $$\{x_{0}\}$$ is open in $$X$$, prove that
    every function $$f\colon X\to Y$$ is continuous at $$x_{0}$$. Is
    the converse true?
3.  Prove that $$f\colon X\to Y$$ is continuous if and only if for
    every $$A\subseteq Y$$ we have that $$f^{-1}(A^{\circ})\subseteq
          (f^{-1}(A))^{\circ}$$.
