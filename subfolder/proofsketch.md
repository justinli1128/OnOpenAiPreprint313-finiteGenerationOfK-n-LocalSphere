---
layout: default1
title: Proof Sketch
---

The proof of [\[OAI26\]](bibliography.md/) regarding Conjecture A follows from the following observation.

### Algebraic Topology 

#### Lemma 2.1
[\[OAI26, Lemma 12.2.2\]](bibliography.md/)

Let $X$ be a derived $p$-complete spectrum, that is $X\simeq \holim\_n (X/p^n)$, where $X/p^n:=\mathrm{hocofib}(p^n:X\to X)$. Then $\pi\_m X$ is $\Z\_p$-finitely generated for every $m\in \Z$ if and only if $\pi\_m (X/p)$ is finite.

_proof:_

The exact sequence $X\xrightarrow{p} X\to X/p\xrightarrow{\delta} \Sigma X$ determines an exact sequence for every $m$

\\[
0\to (\pi\_m X)/ (p \pi\_m X)\to \pi\_m X/p\to \pi\_{m-1} X\[p\]\to 0
\\]Where $M\[p\]$ denoted the $p$-torsion in the abelian group $M$.

($\implies$) For every finitely generated $\Z\_p$-module $M$ and $N$, $M/pM$ and $N\[p\]=\mathrm{span}(u\_i)$ such that $pu\_i=0$ are both finite. Hence, the middle term must be finite.

($\impliedby$) We have exact sequences $X/p^n\xrightarrow{p} X/p^{n+1}\to X/p$. Induction on $n$ shows that if $\pi\_mX/p$ is finite, then $\pi\_m X/p^n$ must all be finite.

We have Milnor's $\lim^1$ sequence and derived $p$-completeness of $X$ determines exact sequence
\\[
0\to \lim^1\pi\_{m-1}(X/p^n) \to \pi\_m(X)\to \lim \pi\_m(X/p^n)\to 0
\\]
Since $\pi\_{m-1}(X/p^n)$ are finite, and since inverse system of finite abelian groups satisfies Mittag-Leffler condition, $\lim^1$ term vanishes, and $\pi\_m(X)\cong \lim \pi\_m(X/p^n)$.

Looking at the exact sequence deduced from $X\to X\to X/p$, the left term is a $p$-torsion finite group, the right term is a $p$-torsion finite group. Hence the middle term must be a finite $p$-group (not necessarily a $p$-torsion, as it might not split, but it is ok). Therefore, $\pi\_m(X)$ has the $\Z\_p$-module structure induced from the inverse limit.

Since $\pi\_m(X/p^n)$ are finite, $\pi\_m(X)$ is compact with the profinite topology. Moreover, since $\pi\_m(X)/p\pi\_m(X)$ and $\Z\_p$ is a local ring with maximal ideal $p\Z\_p$, then by topological Nakayama's lemma, $\pi\_m(X)$ is finitely generated [\[NSW08, Lemma 5.2.18\]](bibliography.md/).

QED.

We have that $K(n)$-local spectrum are derived $p$-complete. Hence, from Lemma 2.1, if we want to show that $\pi\_\*\LKn\S$ is $\Z\_p$-finitely generated, then we just need to show that $(\LKn \S)/p\simeq \LKn (\S/p)$ has finite homotopy group. 

### Continuous Cohomology

We have 
\\[
0\to (E\_n)\_\*\S\xrightarrow{(E\_n)\_\*(p)=\times p}(E\_n)\_\*\S\to (E\_n)\_\*\S/p\to 0
\\] exact, and therefore, $(E\_n)\_\*\S/p\cong (E\_n)\_\*/p$.

By DHSS, we have 
\\[
E\_2^{s,t}=\Hcts^s(\Gn, (E\_n)\_t/p)\implies \pi\_{t-s}\LKn \S/p
\\]

Since $\Gn=Gal(\Fpn/\Fp)\ltimes P\_n$, for every $\Gn$-module $M$. There is the continuous Lyndon-Hochschild-Serre spectral sequence
\\[
E\_2^{p,q}=\Hcts^p(Gal(\Fpn/\Fp), \Hcts^q(P\_n, M))\implies \Hcts^{p+q}(\Gn, M)
\\]

We have $Gal(\Fpn/\Fp)\cong C\_{n}$. If a $C\_{n}$-module $N$ is finite, then $H^p(C\_{n}, N)$ are all finite. Then the god-given vertical and horizontal vanishing line implies that if $\Hcts^q(P\_n, M)$ are finite, $\Hcts^{p+q}(\Gn, M)$ are finite.

#### Lemma 2.2 
[\[Hea23, Proposition 4.13\]](bibliography.md/)

For spectrum $X$ such that DHSS is strongly convergent, there is a horizontal vanishing line on a finite page of DHSS.

Therefore, if $\Hcts^{s}(\Gn, (E\_n)\_t/p)$ are all finite, the horizontal vanishing line implies the ending filtration has only finitely many elements, so $\pi\_{t-s}\LKn(\S/p)$ is finite for all $m=t-s$.

We have deduced the argument into showing the continuous cohomology $\Hcts^q(P\_n, (E\_n)\_t/p)$ is finite.

### $p$-adic Geometry

The Honda formal group law $\Gamma\_n$ has the property $\[p\]\_{\Gamma\_n} T=T^{p^n}$.

Let $k$ be a perfect field of characteristice $p$ ($\Fpn$ is good enough for our argument), $n \leq m\geq 1$ $A\_m:=k\[\[u\_m, ..., u\_{n-1}\]$, $x=u\_m$, and $r=n-m$. Let $F$ denote the restriction of the universal deformation $\widehat{ \Gamma\_n}$ of $\Gamma\_n$ on $A\_m$, that is the pushforward of $\widehat{ \Gamma\_n}$ along $W(k)\[u\_1,...,u\_{n-1}\]\to A\_m$. So $F$ is the universal deformation of $\Gamma\_n$ on height $\geq m$.

Therefore, we have the following property regarding $F$
\\[
\[p\]\_FT= xT^{p^m}+...=Q(T^{p^m})
\\]
for some power series $Q$.

Let $B\_m:= A\_m\[1/x\]$, this is then the locus of the deformation of $\Gamma\_n$ of height exactly $m$, as $x$ is invertible. 

Let $g\in P\_n$, there is a change of coordinate $\alpha\_g: g^*F\to F$. Let $\chi\_g =\alpha'\_g(0)$, then $g(x)=\chi\_g^{p^m-1}x$. Denote $\mathcal{L}\_m=A\_m \cdot u$ where $g(u)=\chi\_g$, the invariant differential line bundle over $A\_m$, an invertible line bundle. We have $L\_m^{\otimes t}=(E\_n)\_{2t}$ as continuous $P\_n$-module. 

Let $\ell\geq 0$, the $p^\ell$-torsion locus of $F$ is described by 
\\[
A\_m\[\[T\]\]/(\[p^\ell\]\_F T)
\\]

Let $0\leq b\leq m\ell$, denote $D(\ell, b)$ the subalgebra of $A\_m\[\[T\]\]/(\[p^\ell\]\_F T)$ generated by $T^{p^b}$. This describes image of $b$-fold Frobenius map ($a\mapsto a^p$ for $b$-times, which is defined as $k$ is characteristic $p$) of the $p^\ell$-torsion of $F$.

#### Definition 2.3
[\[OAI26\], Definition 3.1](bibligraphy.md/) _The **basic coefficients** are_ 
\\[
\mathcal{L}\_m^{\otimes t}\otimes\_{A\_m}\bigotimes\_{i=1}^s D(\ell\_i, b\_i)
\\]
_for $s\geq 0$, $\ell\_i\geq 0$ and $0\leq b\_i\leq m\ell\_i$, and $t\in \mathbb{Z}$._

_The **allowed coefficient** is the smallest class of $A\_m$-modules $\mathcal{C}\_m$ containing the basic coefficients closed under finite direct sum, tensor product, taking equivariant direct summand, and finite equivariant filtrations whose successive quotients belong to the class_

We can think of $\bigotimes\_{i=1}^s D(\ell\_i, b\_i)$ as the geometric intersections of the $b\_i$-fold Frobenius points of $p^{\ell\_i}$-torsions, and tensoring with $\mathcal{L}\_m^{\otimes t}$ takes the invariant differentials over the geometric intersection.

#### Theorem 2.4 (Theorem I)
[\[OAI26\]](bibliography.md/)

_For every $1\leq m\leq n$, for every $M\in \mathcal{C}\_m$ and every $i\geq 0$,
\\[
\Hcts^i(P\_n, M)
\\]is finite._

_proof:_
This argument follows from reverse induction on $m$, going from $n$ to $1$. However, we need to gather some necessary results to deduce this. We leave the proof of this theorem for later.

Q.E.D

We see that Theorem I implies the finite generatedness of $\pi\_t \LKn \S$.



