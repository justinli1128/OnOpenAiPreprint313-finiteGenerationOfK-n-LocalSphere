---
layout: default1
title: Proof Sketch
---

The proof of [OAI26](bibliography.md/) regarding Conjecture A follows from the following observation.

#### Lemma 2.1
[OAI26, Lemma ](bibliography.md/)

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

Looking at the exact sequence deduced from $X\to X\to X/p$, the left term is a $p$-torsion finite group, the right term is a $p$-torsion finite group. Hence the middle term must be a finite $p$-group (not necessarily a $p$-torsion, as it might not split, but it is ok). Therefore, $\pi\_m(X)$ is a $\Z\_p$-module. 

Since $\pi\_m(X)/p\pi\_m(X)$ is finite and $\Z\_p$ is a local ring with maximal ideal $p\Z\_p$, then by Nakayama's lemma, $\pi\_m(X)$ is finitely generated.

QED.

We have that $K(n)$-local spectrum are derived $p$-complete. Hence, from Lemma 2.1, if we want to show that $\pi\_\*\LKn\S$ is $\Z\_p$-finitely generated, then we just need to show that $(\LKn \S)/p\simeq \LKn (\S/p)$ has finite homotopy group. 

We have 
\\[
0\to (E\_n)\_\*\S\xrightarrow{(E\_n)\_\*(p)=\times p}(E\_n)\_\*\S\to (E\_n)\_\*\S/p\to 0
\\] exact, and therefore, $(E\_n)\_\*\S/p\cong (E\_n)\_\*/p$.

By DHSS, we have 
\\[
E\_2^{s,t}=\Hcts^s(\Gn, (E\_n)\_\t/p)\implies \pi\_{t-s}\LKn \S/p
\\]

Since $\Gn=Gal(\Fpn/\Fp)\ltimes S\_n$, for every $\Gn$-module $M$. There is the continuous Lyndon-Hochschild-Serre spectral sequence
\\[
E\_2^{p,q}=\Hcts^p(Gal(\Fpn/\Fp), \Hcts^q(S\_n, M))\implies \Hcts^{p+q}(\Gn, M)
\\]

We have $Gal(\Fpn/\Fp)\cong C\_{n-1}$. If a $C\_{n-1}$-module $N$ is finite, then $H^p(C\_{n-1}, N)$ are all finite. Then the god-given vertical and horizontal vanishing line implies that if $\Hcts^q(S\_n, M)$ are finite, $\Hcts^{p+q}(\Gn, M)$ are finite.

#### Lemma 2.2 
[Hea23, Proposition 4.13]

For spectrum $X$ such that DHSS is strongly convergent, there is a horizontal vanishing line on a finite page of DHSS.

Therefore, if $\Hcts^{s}(\Gn, (E\_n)\_\t/p)$ are all finite, the horizontal vanishing line implies the ending filtration has only finitely many elements, so $\pi\_{t-s}\LKn(\S/p)$ is finite for all $m=t-s$.

#### Conclusion

We have deduced the argument into showing the continuous cohomology $\Hcts^q(S\_n, (E\_n)\_\t/p)$ is finite.
