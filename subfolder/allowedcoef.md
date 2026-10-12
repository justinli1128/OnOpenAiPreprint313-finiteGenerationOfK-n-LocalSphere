---
layout: default1
title: Allowed Coefficients
---
Recall the definition of allowed coefficients.

#### Definition
[\[OAI26\], Definition 3.1](bibligraphy.md/) _The **basic coefficients** are_ 
\\[
\mathcal{L}\_m^{\otimes t}\otimes\_{A\_m}\bigotimes\_{i=1}^s D\_m(\ell\_i, b\_i)
\\]
_for $s\geq 0$, $\ell\_i\geq 0$ and $0\leq b\_i\leq m\ell\_i$, and $t\in \mathbb{Z}$._

_The **allowed coefficient** is the smallest class of $A\_m$-modules $\mathcal{C}\_m$ containing the basic coefficients closed under finite direct sum, tensor product, taking equivariant direct summand, and finite equivariant filtrations whose successive quotients belong to the class_

#### Lemma 3.1 (Weierstrass Preparation Theorem)

_Let $R$ be a complete local ring, with maximal ideal $\mathfrak{m}$. Suppose $f$ is a formal power series over $R$, such that $f\not \equiv 0 \mod \mathfrak{m}$, then there is $v\in R\[\[t\]\]^\times$ and monic polynomial $W(t)=t^{s}+\sum\_{i=0}^{s-1} b\_i t^i$ for $b\_i \in \mathfrak{m}$._

#### Lemma 3.2
[\[OAI26\], Lemma 3.2](bibligraphy.md/)

_The algebra $D\_m(\ell, b)$ are free of rank $p^{n\ell-b}$ over $A\_m$. Moreover, the construction of this subalgebra is independent of the choice of coordinate, i.e. suppose we have a change of coordinate $\alpha: A\_m\[\[T\]\]\to A\_m\[\[\alpha(T)\]\]$, the Frobenius and hence $D\_m(\ell, b)$ are unchanged, with $D\_m(\ell, b)/(x)=D\_{m+1}(\ell, b)$. Lastly, every module in $\mathcal{C}\_m$ are finite free over $A\_m$, and modulo $x$ takes $\mathcal{C}\_m$ to $\mathcal{C}\_{m+1}$._

_proof:_

Since $\[p^\ell\]\_F T=K(T^{p^{m\ell})$ for some power series $K$, there is power series $f$ such that $f(T^{p^b})=\[p^\ell\]\_F T$, and $f(t)=x^\ell t^{p^{m\ell-b}}+...$.

Note that $F$ is a deformation of $\Gamma\_n$, hence modulo the maximal ideal recovers the $n$-series. In other word, $\[p^\ell\]\_F T\equiv T^{n\ell}\mod \mathfrak{m}$. Therefore, $f(t)\equiv t^{p^{n\ell-b}}\mod \mathfrak{m}$. 

By Weierstrass Preparation Theorem, $f(t)=v(t)W(t)$, with $W(t)=t^{p^{n\ell-b}}+...$. Since $W$ is monic, $A\_m\[t\]/(W)$ is finite free over $A\_m$, with rank $p^{n\ell-b}$.

Define map $A\_m\[t\]/(W)\to A\_m\[\[T\]\]/(\[p^\ell\]\_F T)$ via $t\mapsto T^{p^b}$, this is injective and has image $D\_m(\ell, b)$, which shows the first statement.

For a coordinate change, we have $\alpha(T^{p^b})=\alpha(T)^{p^b}$, so the subalgebra is preserved. 

We see that $\[p^\ell\]\_F T$ over $A\_m$ modulo $x$ is precisely $\[p^\ell\]\_FT$ over $A\_{m+1}$, so the subalgebra is preserved under restriction to higher height locus. Similarly, $\mathcal{L}\_m/ (x)=\mathcal{L}\_{m+1}$ as well.

Lastly, finite tensor product and finite direct sums preserves finite freeness. Since $A\_m$ is local, by Kaplansky's Theorem of Projective Modules, direct summand of finite free modules are finite free. 

Now its left with the filtration condition. Given a finite filtration $F^t M\subseteq F^{t-1}\subseteq F^0M$, where $F^iM/F^{i+1}M\in \mathcal{C}\_m$. There are exact sequences
\\[
0\to F^{i+1}M\to F^iM\to F^iM/F^{i+1}M\to 0
\\] The right term is by assumption finite free, hence $F^iM$ splits. Inducting on $i$, we are then left to show that $F^tM$ is finite free, which is the assumption.

Q.E.D.

We denote $F\[p^\ell\]:=\mathrm{spf} A\_m\[\[T\]\]/(\[p^\ell\]\_F T)$ the formal scheme of $p^\ell$-torsions of $F$. There is inclusion $F\[p^\ell\]\to F\[p^{\ell+1}\]$, and we denote $F\[p^\infty\]:=\colim\_\ell F\[p^\ell\]$, the $p$-divisible group of $F$.

