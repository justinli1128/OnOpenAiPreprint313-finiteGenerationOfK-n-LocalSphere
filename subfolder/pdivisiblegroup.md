---
layout: default1
title: p-divisible Group
---

#### Definition A.1
[\[Tat67\], 1.1](\bibliography.md/)
_A **finite group scheme** of rank $m$ over a base scheme $S$ is a finite morphism $G\to S$ such that $G$ is locally free of rank $m$ such that there is multiplication $m: G\times\_S G\to G$, inverse $i:G\to G$, and $e: S\to G$ over $S$ determining a group structure._

#### Definition A.1
[\[Tat67\], 1.3](\bibliography.md/)
_Assume everything to be commutative, a **short exact sequence** of finite group schemes is a sequence of group scheme morphism
\\[
0\to G'\xrightarrow{i} G\xrightarrow{p} G"\to 0
\\]
such that this is exact in the category of fppf sheaves of abelian group over schemes over $S$._

This is equivalent to closed immersion $i:G'\to G$ such that $G'=G\times\_{G"}S$, and $p: G\to G"$ is faithfully flat.   

#### Definition A.1
[\[Tat67\], 2.1](\bibliography.md/)

_A **$p$-divisible group of height $h$** over $S$ is a inductive system $(G\_n, i\_n)\_{n\in \mathbb{N}}$ such that $G\_n$ is a finite group of rank $p^{nh}$ over $S$, and closed immersions $i\_n: G\_n\to G\_{n+1}$ such that 
\\[
0\to G\_n \xrightarrow{i\_n} G\_{n+1}\xrightarrow{p^n}G\_{n+1}\to 0
\\]
are exact._

_A homomorphism of $p$-divisible group is a morphism of inductive system._

#### Examples

Let $G_n$ be ordinary abelian groups, then we have $G\_1=(\Z/p\Z)^h$, and by induction, 
\\[
G\_n=(\Z/p^n\Z)^h, G=\colim\_n G\_n =(\mathbb{Q}\_{p}/\Z\_p)^h
\\]

Let $F$ be a formal group of height $h$, $F\[p^n\]$ of $p^n$-torsion are finite group schemes, and determines a $p$-divisible group $F\[p^\infty\]$. If $F$ has height $\geq h$, then $F\[p^\infty\]$ woud have at least height $h$.

For every finite group scheme $G$ over $S$, there is an short exact sequence [\[Tat67\], 1.4](bibliography.md/)
\\[
0\to G^0\to G\to G^{ét}\to 0
\\]
Where $G^0$ is connected, and $G^{ét}$ is étale over $S$. If $G$ is $p$-divisible, then $i\_n:G\_n^0\to G\_{n+1}^0$, then there is an exact sequence of $p$-divisible group.


