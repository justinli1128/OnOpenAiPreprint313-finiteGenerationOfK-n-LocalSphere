---
layout: default1
title: p-adic Geometry and p Analytic Group
---

#### Definition 3.1

[\[Sch11, Definition, Chapter 1\]](bibliography.md/)

_An **ultrametric** space $(X,d)$ is a metric space such that for any $x,z\in X$_
\\[ d(x,z)\leq \max(d(x,y), d(y,z))
\\]_for any $y \in X$_

#### Lemma 3.1

[\[Sch11, Lemma 1.2\]](bibliography.md/)

_Let $(X,d)$ be an ultrametric space,_
_1) Every ball is both open and closed._

_2) For every $b\in B\_r(a)$, $B\_r(b)=B\_r(a)$, and for every $b\in \overline{ B\_r(a)}$, $\overline{ B\_r(b)}=\overline{ B\_r(a)}$_

#### Definition 3.1

[\[Sch11, Definition, Chapter 1\]](bibliography.md/)

_Let $K$ be a field. A **nonarchimedean absolute value** on $K$ is a multiplicative function_
\\[
|-|: K\to \mathbb{R}\_{\geq 0}
\\]
_such that $|a|=0$ if and only if $a=0$, and $|a+b|\leq \max(|a|,|b|)$._

The metric space induced by a nonarchimedean absolute value on $K$ is then an ultrametric space. We say $K$ is a **nonarchimedean field** if there is $a\in K$ such that $|a|\neq 0,1$ and $K$ is complete under the metric induced.

#### Definition 3.2

_Let $K$ be a field, a **valuation** on $K$ is a function $v: K\to \mathbb{R}\cup \infty$ such that_
_1) $v(ab)=v(a)+v(b)$_

_2) $v(a+b)\geq \min(v(a),v(b))$_

_3) $v(a)=\infty$ if and only if $a=0$_

For every nonarchimedean absolute value $|-|$ on $K$ determines a valuation on $K$ via formula
\\[
v(a)=-\log\_{r}(|a|)
\\]for some $r>1$ (for instance, we may let $r$ be a prime $p$).

A valuation $v$ on a field $K$ determines a ring $R:=v^{-1}(\[0,\infty\])$ (the **valuation ring**), which is closed in $K$ by definition, and has unique maximal ideal $\mathfrak{m}:=v^{-1}((0,\infty\])$.

#### Example

_Let $\mathbb{Q}\_p$ denote the fraction field of $\Z\_p$, so every element $a\in \mathbb{Q}\_p$ can be expressed as a power series with terms $p^{n}$ for $n\in \Z$ such that $a\_n=0$ for $n$ sufficiently small (might be negative). There is a valuation $v\_p(a):= k$ for smallest $k$ such that $a\_k\neq 0$._

_Obviously, $\Z\_p$ is the valuation ring of $v\_p$, with maximal ideal $p\Z\_p$. There is then an absolute value, such that $|a|=p^{-k}$._

_Notice $|-|$ values in $\Z$, hence $\Z\_p$ is also an open set of $\mathbb{Q}\_p$._

#### Definition 3.3

[\[Sch11, Definition, Chapter 2\]](bibliography.md/)

_Fix a nonarchimedean field $K$, a $K$-manifold $M$ of dimension $n$ is a Hausdorff topological space with a set of tuple $(U\_i, \varphi\_i)$, where $U\_i$ determines an open cover of $M$ and $\varphi\_i: U\_i\to K^n$ such that_

_1) $\varphi\_i(U\_i)$ is open_

_2) $\varphi\_i: U\_i \to K^n$ is an homeomorphism onto the image_

(This is just the definition of a typical manifold with $\mathbb{R}$ replaced with $K$)

Let $U \subseteq K^n$ be an open set, and let $V$ be a $K$-Banach space. A **locally analytic** function $U\to V$ is a function $f$ such that for every $X\_0 \in U$, there is an open neighbourhood $N$ of $X\_0$ such that 
\\[
f(x)=\sum\_{\alpha\in \mathbb{N}^{n}}(X-X\_0)^\alpha v\_\alpha
\\]for $v\_\alpha \in V$ (of course, the right hand side must be convergent first, but for nonarchimedean $K$, this is equivalent to $\|v\_\alpha\|\to 0$ as $|\alpha|\to \infty$, which is much easier than $\mathbb{R}$ or $\C$).

We say a map $f: M\to V$ is locally analytic if restricting to the open chart, the function is locally analytic, and $f:M\to N$ is locally analytic if over the overlapped, the function is locally analytic. 

#### Definition 3.4

[\[Sch11, Definition, Chapter 3\]](bibliography.md/)

A **$p$-adic analytiv group** is a group $\varphi: G\times G\to G$ such that $G$ is a $\mathbb{Q}\_p$ manifold, and $\varphi$ is locally analytic.

#### Examples

Equip $\mathbb{Q}\_p$ with the addition group structure, then this is obviously a $p$-adic analytic group. Moreover, $\mathbb{Z}\_p$ is open and a group under the addition group structure, so it is also a $p$-adic analytic group. 

#### Definition 3.5


