---
layout: post
title: Topological spaces
date: 2016-01-25 9:00 -0500 
comments: true
published: true
categories: 
---

<div id="table-of-contents">
<h2>Table of Contents</h2>
<div id="text-table-of-contents">
<ul>
<li><a href="#orgheadline2">1. Notation</a>
<ul>
<li><a href="#orgheadline1">1.1. </a></li>
</ul>
</li>
<li><a href="#orgheadline11">2. Topological spaces</a>
<ul>
<li><a href="#orgheadline5">2.1. Definitions</a></li>
<li><a href="#orgheadline6">2.2. Examples</a></li>
<li><a href="#orgheadline7">2.3. More examples</a></li>
<li><a href="#orgheadline10">2.4. Cofinite topology</a></li>
</ul>
</li>
<li><a href="#orgheadline13">3. Exercises</a>
<ul>
<li><a href="#orgheadline12">3.1. Exercises</a></li>
</ul>
</li>
<li><a href="#orgheadline15">4. Links</a>
<ul>
<li><a href="#orgheadline14">4.1. Links</a></li>
</ul>
</li>
</ul>
</div>
</div>


# Notation<a id="orgheadline2"></a>

## <a id="orgheadline1"></a>

-   **$$X$$:** a set
-   **$$P(X)$$:** the **power set** of $$X$$, that is, the set of all
    subsets of $$X$$.
-   **$$\mathbb{R}$$:** the set of real numbers.

# Topological spaces<a id="orgheadline11"></a>

## Definitions<a id="orgheadline5"></a>

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

## Examples<a id="orgheadline6"></a>

-   Let $$X$$ be any set. Then $$\tau_{d}=P(X)$$ is a topology,
    called the *discrete topology*.

-   Let $$X$$ be any set. Then $$\tau_{i}=\{\emptyset,X\}$$ is a
    topology, called the *indiscrete topology*.

-   Let $$X=\{1,2\}$$. Then $$\tau=\{\emptyset,X,\{1\}\}$$ is a
    topology, and $$(X,\tau)$$ is called the *Sierpiński space*.

## More examples<a id="orgheadline7"></a>

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

## Cofinite topology<a id="orgheadline10"></a>

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
        $$U_{1}\cap U_{2}$$ is empty or $$X-U_{1}\cap U_{2}$$ is finite.

# Exercises<a id="orgheadline13"></a>

## Exercises<a id="orgheadline12"></a>

1.  Show that if $$X$$ is any set, there is a metric on $$X$$ such
    that the metric topology is the same as the discrete topology.
2.  Show that in general there is no metric on $$X$$ such that the
    metric topology is the same as the indiscrete topology.
3.  Show that if $$\tau_{\alpha}$$ is a topology on $$X$$ for each
    $$\alpha\in I$$, then $$\tau=\cap\tau_{\alpha}$$ is a topology
    on $$X$$.

# Links<a id="orgheadline15"></a>

## Links<a id="orgheadline14"></a>

-   [Topological space - Wikipedia, the free encyclopedia](http://en.wikipedia.org/wiki/Topological_space)
-   [How to get intuition in topology concerning the definitions? - Mathematics Stack Exchange](http://math.stackexchange.com/questions/1598409/)
-   [Why is a topology made up of 'open' sets? - MathOverflow](http://mathoverflow.net/questions/19152/why-is-a-topology-made-up-of-open-sets)
-   [Why does topology rarely come up outside of topology? - Mathematics Stack Exchange](http://math.stackexchange.com/questions/1592421/why-does-topology-rarely-come-up-outside-of-topology)