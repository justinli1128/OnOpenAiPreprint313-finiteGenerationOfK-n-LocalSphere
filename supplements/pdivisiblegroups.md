---
meta-viewport: width=device-width, initial-scale=1
title: p-divisible Groups (continued)
---

# $p$-divisible Groups (continued)

[Home](https://justinli1128.github.io/OnOpenAiPreprint313-finiteGenerationOfK-n-LocalSphere/) · [Background](https://justinli1128.github.io/OnOpenAiPreprint313-finiteGenerationOfK-n-LocalSphere/subfolder/background/) · [p-divisible Group](https://justinli1128.github.io/OnOpenAiPreprint313-finiteGenerationOfK-n-LocalSphere/subfolder/pdivisiblegroup/)

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

Picks up after Definition A.1 and the connected–étale sequence on the earlier page.

#### Definition D.1 (Frobenius and relative Frobenius)

*TODO: $F$, $V$, $\mathrm{Frob}^b$ on a finite group scheme over $\mathbb F_p$-algebras; the relative Frobenius image.*

#### Proposition D.2 (connected–étale sequence over $x\ne0$)

*TODO: for $F[p^\ell]$ over $B_m$, orders $p^{m\ell}$ (connected) and $p^{r\ell}$ (étale), $r=n-m$. Why the sequence exists only over $x\ne0$.*

#### Definition D.3 (Cartier duality)

*TODO: $G^D=\underline{\mathrm{Hom}}(G,\mathbb G_m)$ for finite flat commutative $G$.*

#### Proposition D.4 (duality arithmetic on $\Gamma_m$)

*TODO: $F^m=[p]$ and $FV=[p]$ on $\Gamma_m$; hence $V^m=[p]$ on the dual, $\dim\Gamma_m^D=m-1$, and for $m>1$ the dual has no étale part. Consequence: $d=(m-1)r$.*

Used in: §7 (Cartier transfer), §10.5 (the algebra $\Lambda=k[[D_1,\dots,D_d]]$).

#### Definition D.5 (universal cover)

*TODO: $\widetilde G(S)=\varprojlim_{p:G\to G}G(S)$.*

#### Theorem D.6 (Scholze–Weinstein, Prop 3.1.3)

*TODO: over a perfect base $R$ of characteristic $p$, for $G$ connected with $\mathrm{Lie}\,G$ free of rank $d$, $\widetilde G$ is represented by $\mathrm{Spf}\,R[[X_1^{1/p^\infty},\dots,X_d^{1/p^\infty}]]$.*

Used in: Lemma 4.1.

#### Examples

*TODO: $F[p^\infty]$ for a formal group $F$ of height $h$; $\mu_{p^\infty}$ and $\mathbb Q_p/\mathbb Z_p$.*

#### Where the preprint uses this

*TODO: locators for §3.3–3.4, §4 (Lemma 4.1), §7.*

© 2026
