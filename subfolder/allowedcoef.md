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

Since $\[p^\ell\]\_F T=K(T^{p^{m\ell}})$ for some power series $K$, there is power series $f$ such that $f(T^{p^b})=\[p^\ell\]\_F T$, and $f(t)=x^\ell t^{p^{m\ell-b}}+...$.

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

We denote $F\[p^\ell\]:=\spec A\_m\[\[T\]\]/(\[p^\ell\]\_F T)$ the scheme of $p^\ell$-torsions of $F$. There is inclusion $F\[p^\ell\]\to F\[p^{\ell+1}\]$, and we denote $F\[p^\infty\]$ the $p$-divisible group of $F$.

Now over, $B\_m=A\_m\[1/x\]$, $x$ is invertible, so $F$ has height exactly $m$. Hence the formal group of connected component of $F\[p^\infty\]$, $F\[p^\infty\]^0$ has height exactly $m$. 

#### Theorem 3.2
[\[Lur10\], Theorem 1, Lecture 14](bibliography.md/)
_For $F$ and $F'$ two formal group law over a ring $R$ of height exactly $h>0$, let $Iso(F,F')$ denote the ring classifying isomorphisms from $F$ to $F'$, there is then a directed system of injective finite étale map 
\\[
R=R(1)\to R(2)\to ... 
\\]such that $Iso(F,F')=\colim \_n R(n)$._

#### Definition 3.3
(I am not sure if this definition is found elsewhere, but the preprint did not give a definition, forcing me to guess what it means)

_Given two formal groups of height $h$ over $R$, we know that $Iso(F,F')$ is pro-finite-étale, a **marking** is then a $T$-point of $Iso(F,F')$ for some cover $T$ over $R$, that is an isomorphism $f: F\_T\to F\_T'$._

There is an action of $P\_n$ on $Q:=Iso(F\[p^\infty\]^0,\Gamma\_m \otimes\_k B\_m)$ determined by precomposition. There is also an action of $P\_m$ on $Q$ determined by postcomposition, which is transitive, determining a pro-finite-étale $P\_m$-torsor over $B\_m$, as $Q=\lim\_h Q\_h$ is pro-finite-étale, for each $Q\_h:=Iso(F\[p^\infty\]^0,\Gamma\_m \otimes\_k B\_m)/ U\_h$ a $P\_m/ U\_h$-finite-étale torsor (so $Q\_h$ is represented by some finite étale $B\_m$-algebra. Recall that $U\_h$ is the normal subgroup of $P\_m$ such that $U\_h$ are equivalent to the identity modulo $T^{p^{h+1}}$.

#### Proposition 3.3

_For every $h\geq 0$, the $P\_m/U\_h$-torsor $Q\_h$ is represented by a finite free algebra $H\_{m,h}$ over $A\_m$ spanned by variables $a\_0,...,a\_h$ such that
\\[
a\_0^{p^m-1}=x, a\_i^{p^m}-x^{p^i}a\_i=P\_i(a\_0,...,a\_{i−1})
\\]for some polynomials $P\_i$. That is over $B\_m$, $Q\_h=\spec(H\_{m,h}\[1/x\])$. $H\_{m,h}$ are freely generated by $a\_0^{e\_0}a\_1^{e\_1}...a\_{h}^{e\_h}$ for $0\leq e\_0 <p^m-1$ and $0\leq e\_i<p^m$_

_Moreover, the $P\_n$ action on $H\_{m,h}$ induced by the identification above preserves $H\_{m.h}\[1/x\]$, and there exists a finite filtration on $F^t\subseteq F^{t-1}\subseteq ...\subseteq F^0=H\_{m,h}$ such that $F^{i}/F^{i+1}\cong \mathcal{L}\_m^{\otimes d\_i}$ for some $d\_i \in \Z$. The identification and the filtration is preserved under restriction to higher height._


_proof:_

Let $f:F\[p^\infty\]^0\to \Gamma\_m$ be an isomorphism over some $B\_m$-algebra, which is an ordinary power series $f(T)=\sum\_{j\geq 1}c\_j T^j, and denote $a\_i=c\_{p^i}$. 

We have the equality,
\\[
f(F\[p^\infty\]^0(X,Y))=\Gamma\_m(f(X),f(Y))
\\]
Comparing coefficients and using the fact $p=0$ over $B\_m$, we have that $c\_i$ are determined by $a\_i$, where $a\_i$ are freely determined. Comparing $p$-series
\\[
f(\[p\]\_F T)=f(T)^{p^m}
\\]gives us the identity in the statement. Then we see that the generation is trivial.

Therefore, there exists a morphism $Q\_h\to \spec(H\_{m,h}\[1/x\])$ sending an isomorphism modulo $U\_h$ over a $B\_m$ algebra $R$ to the $R$ point corresponding to the formal power series modulo $T^{p^{h+1}}$ determined by the corresponding $R$-point of $ \spec(H\_{m,h}\[1/x\])$.

Over separable closed fields, every height $m$ formal group law $F$ is isomorphic to $\Gamma\_m$, and we have $P\_m/U\_h$ has rank $(p^m-1)p^{mh}$. The map $Q\_h\to \spec(H\_{m,h}\[1/x\])$ is surjective on the separable closed field(?). Therefore, surjectivity and same rank over separable closed field implies isomorphism between finite étale algebra.

The action of $G$ on $Q\_h$ is determined by precomposition, that is for $g\in G$ and $f\in Q\_h$, $g\cdot f\equiv f\circ \alpha\_g \mod T^{p^{h+1}}$. We have that $\alpha\_g(T)=\chi\_g T+\sum\_{l\geq 2}\beta\_l T^l$, and 
\\[
f(\alpha\_g(T))=a\_0\alpha\_g(T)+a\_1\alpha\_g(T)^p+a\_2\alpha\_g(T)^{p^2}+...+ \text{other terms}
\\= g\cdot a\_0 T+g\cdot a\_1 T^{p}+...+ g\cdot \text{other terms}
\\]
The only degree $1$ term in this equation is $\chi\_g a\_0$ hence $g(a\_0)=\chi\_g a\_0$. Similarly, for the degree $p^i$ term, there is a coefficient of $\chi\_g^{p^i} a\_i$ with addition of some polynomial of coefficient $Q$, which depends on the term $a\_0,...,a\_{i-1}$ because all the term containing $a\_{j> i}$ contribute to the term of higher degree. The coefficient of $Q$ does not contain any inverses of $x$, and $H\_{m,h}$ is $x$-torsion-free, so the action of $G$ on $Q\_h=\spec H\_{m,h}\[1/x\]$ extend to an action on $H\_{m,h}$.

Lastly, we impose the inverse lex ordering on $a\_0^{e\_0}...a\_h^{e\_h}$, that is comparing power $e\_h$ first then break tie with $e\_{h-1}$ and so on. 









