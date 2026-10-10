---
layout: default1
title: Motivations and Related Works
---
v(2.1)
(Some of these definitions are in [my note](https://justinli1128.github.io/jiahaoliAcademicWebsite/Algebraic_Geometry_in_Chromatic_Homotopy_Theory.pdf), or many other texts availables elsewhere)

Let $X$ be a spectrum (in homotopy theory), such as the sphere spectrum $\S=\Sigma^\infty S^0$. We often want to know the stable homotopy groups $\pi_n(X):= \[\Sigma^n\S, X]$.

Given another spectrum $E$, representing some nice cohomology, such as $H\Z$ for integral cohomology, or $M\Z_{(p)}$ for $p$-local Moore spectrum.

[Definition 1.1](https://ncatlab.org/nlab/show/Bousfield+localization+of+spectra#definition)

A **$E$-acyclic spectrum** $X$, is a spectrum such that $E\wedge X\simeq 0$.

A **$E$-equivalence** $f:X\to Y$, is a morphism such that $f:E\wedge X\to E\wedge Y$

A **$E$-local spectrum** $X$, is a spectrum such that the following equivalent conditions are satisfied

1) for any $E$-equivalence $f:Y\to Z$, $\[f,X\]:\[Z, X\]\to\[Y,X\]$ is an isomorphism
2) for any $E$-acyclic spectrum $Y$, $\[Y,X\]\cong 0$.

Some cohomology of interests are

[Definition 1.2](subfolder/bibliography/)\[Lur10\]

A **complex oriented cohomology** is a spectrum $E$, such that $E^2(\CP^\infty)\to E^2(\CP^1)\cong E^0$ is surjective. A **complex orientation** is a lift $t\_E\in E^2(\CP^∞)$ of $1\_E$.

Using Atiyah-Hirzebruch Spectral Sequence to compute $E^*(\CP^n)$, we have $E^*(\CP^n)\cong E^*\[\[t\_E\]\]/(t\_E^{n+1})$, and $\lim^1 E^*(\CP^n)$ vanishes so 

[Theorem 1.3](bibliography.md/)\[Lur10\]

For a complex oriented cohomology $E$, and a complex orientation $t_E\in E^2(\CP^∞)$, then 
\\[
E^*(\CP^∞)\cong E^*\[\[t\_E\]\]
\\]

There is a group structure on $\CP^∞$ induced from the tensor product of complex line bundles (note, $BU(1)\simeq \CP^∞$). Therefore, given a complex oriented cohomology $(E,t\_E)$, there is then a cogroup structure on $E^*\[\[t\_E\]\]$. We refer to a cogroup structure on the formal power series ring over $E^*$ as a **formal group law** over $E^\*$. This is determined by a formal power series $F(x,y)$ determined by the image of $t\_E$.

A formal group law $x+\_F y:=F(x,y)$ over $R$ determines a sequence of power series
\\[
\[n\]\_F t:=t+\_F t+\_F...+\_F t
\\] $n$ times.

For a prime $p$, we let $v\_n\in R$ denote the coefficient in front of $t^{p^n}$ term in $\[p\]\_F t$.

Let $MU$ denote the Thom spectrum of universal complex vector bundle. 

[Theorem 1.4](bibliography.md/)\[Lur10\]

There is a complex orientation $t\_{MU}$ on $MU$, and let $E$ be a commutative ring spectrum, there is bijection
\\[
 \text{Ring maps $MU\to E$}/\sim \cong \text{complex orientation of $E$}
\\]

Therefore, not only $MU$ is complex oriented, it is universal among all the complex orientation over multiplicative cohomology.

A classic theorem of Quillen says.

[Theorem 1.5](bibliography.md/)\[Qui69\]

The ring $MU^\*\cong \Z\[a\_1, a\_2,...\]$ is the Lazard ring, classifying formal group laws and the formal group law $F\_{MU}$ over $MU^*$ is the universal formal group law, such that the ring map determining the complex orientation over $E$ determines the formal group law over $E$.

Therefore, if we have a formal group law $F$ over a graded ring $R\_\*$, there is then an unique graded ring map $MU\_\*\to R\_\*$. We have a functor in graded $R\_\*$-modules
\\[
R\_\*(X):=MU\_\*(X)\otimes \_{MU\_\*} R\_\*
\\]
This is not necessarily a homology. However, under certain circumstances, this determines a homology.

[Theorem 1.6](bibliography.md/)\[Lan76\]

$R\_\*(-)$ is a homology if there is a prime $p$, and associated $v\_n$ in $MU\_\*$ such that $(p, v\_1,v\_2,...)$ is a regular sequence in $R\_{\*}$, i.e. $v\_n$ is not a zero divisor of $R\_\*/(p,v\_1,...,v\_{n-1})R\_\*$.

We refer to this condition as **Landweber flat**

Let $\Mfg$ be the (fpqc) moduli stack of formal groups over $\spec\Z$. As it turns out
[Theorem 1.7](bibliography.md/)\[Nau07\]

A graded ring map $MU\_\*\to R\_\*$ determining a formal group law is Landweber flat iff the classifying map $\spec(R\_\*)\to \Mfg$ is flat.

A multiplicative cohomology $E$ is **even periodic** if there exists $u\in E^2$ such that $\times u:E^\*\to E^{\*+2}$ is an isomorphism, and $E^1\cong 0$. A even periodic cohomology is clearly complex orientable.

Let $MP:=MU\[u^{\pm}\]\cong \bigvee\_{n\in \mathbb{Z}} \Sigma^{2n}MU$, this is even periodic. Then $MP\_0\cong MU\_\*$. Then a Landweber flat $R$ (ungraded) determines an homology $RP\_\*(-):=MP\_\*(-)\otimes\_{MP\_0}R$.

From now we assume everything is $p$-local, then there is a open substack filtration $\Mfg^{\leq n}\subseteq \Mfg$ determining the $p$-local formal groups of height $\leq n$, the complement of $Mfg^{\geq n}$ the formal groups of height $\geq n$ i.e. formal group laws such that and $v\_{m}=0$ for $m\leq n-1$.

The open substack $\Mfg^{\leq n}$ is determined by an affine cover \\[\spec(\Z\_{(p)}\[v\_1,...,v\_n^{\pm}\]\to \Mfg^{\leq n}
\\]

This determines the **Johnson-Wilson** spectrum $E(n)$ such that $E(n)\_\*=\Z\_{(p)}\[v\_1,...,v\_n^{\pm}\]\[u^\pm\]$.

The $E(n)$-localization, denotes $L_n$ determines a tower
\\[
id\to ...\to L\_n\to L\_{n-1}\to ...L\_1\to L\_0 \simeq L\_{H\mathbb{Q}}
\\]

[Theorem 1.8](bibliography.md/)\[Lur10\]
For finite spectrum $X$, $X\simeq \holim\_n L\_n X$.

The closed substack $\Mfg^n$ of formal groups of height exactly $n$, i.e. height $\geq n$ such that $v\_n$ is invertible. There is an affine cover $\spec(\Fp\[v\_n^{\pm}])

This is not flat over $Mfg$, but there is still a spectrum $K(n)$, the **Morava K-theory**, such that \\[K(n)\_*\cong \Fp\[v\_n^{\pm}\][u^\pm]\\]. 

[Theorem 1.9](bibliography.md/)\[Lur10\]

For any spectrum $X$, there is a homotopy pullback diagram 

\begin{array}{ccc}
L\_n X & \longrightarrow & \LKn X
\end{array}
\begin{array}{ccc}
\downarrow && \downarrow
\end{array}
\begin{array}{ccc}
L\_{n-1} X & \longrightarrow & L_{n-1}\LKn X
\end{array}

Therefore, it is important to understand $LKn \S$, as it is the first step to recover $\pi\_* \S$.

Let $\LT\_n$ be the Lubin-Tate space of deformation of a height $n$ formal group law over $\Fpn$. This space lives over $\widehat{\Mfg^{n}}$, the infinitesimal formal neighbourhood of $\Mfg^{n}$. The space $\LT\_n$ is discrete, and it is represented by a profinite ring $W(\Fpn)\[\[v\_1,...,v\_{n-1}\]\]$, and there is a spectrum $E\_n$ such that 
\\[
(E\_n)\_{\*}=W(\Fpn)\[\[v\_1,...,v\_{n-1}\]\]\[u^\pm]
\\] Moreover, let $\Gn$ denote the automorphism group of $\LT\_n$ over $\widehat{\Mfg^{n}}$, then we have $\LT\_n//\Gn\simeq \widehat{\Mfg^{n}}$. The group $\Gn$ is profinite, determined by a chain of closed subgroup $U\_k\subset U\_{k-1}\subset \Gn$, and acts continuously on $(E\_n)\_*$.

[Theorem 1.10](bibliography.md/)\[DH04\]

For a spectrum $X$, there is a spectral sequence
\\[
E^{s,t}\_2=\Hcts^{s}(\Gn, (E\_n)\_t X)\implies \pi\_{t-s}\LKn X
\\]which strongly converges for CW spectra.

We will refer to this spectral sequence DHSS.
