---
draft: 
date: 2024-09-03
---
I followed this course by, Prof. [Nick Bezhanishvili]() during my [[5th Semester]] at the [[University of Amsterdam]] for my [[M.Sc. Logic (UvA)]]. I covered most of the material already in [[Modal Logic (Lecture)]]. I paired for exercises with Josje van der Laan.
#### Assignments
1. [Overleaf: IML, 1](https://www.overleaf.com/read/qdtknhmjymqt#0a2005)
2. [Overleaf: IML, 2](https://www.overleaf.com/read/cpcbpxgshgwx#9933a8)
3. [Overleaf: IML, 3](https://www.overleaf.com/read/fhfgdcfdxfks#e50bb8)
4. [Overleaf: IML, 4](https://www.overleaf.com/read/nqzhrtkqwbjy#cd734e)
5. [Overleaf: IML, 5](https://www.overleaf.com/read/bnbpqggkwwdm#e2f4f5)

## Lecture Notes
- Bisimilarity & Invariance Lemma, as in: [[Modal Logic (Lecture)#3. Expressive Power and Invariance]].
	- converse of invariance lemma holds with $n$-bisimilarity for $n \in \mathbb{N}$.
	- $\mathcal{M} = (M, R, V)$ is _image finite_ if $\forall_{x \in M} |R[x]| < \aleph_0$
		- $R[x] := \{y \in M : x R y\}$
	- for $\mathcal{M}$, $\mathcal{M}'$ image finite, $\forall_{x \in M}\forall_{x' \in M'} \mathcal{M}, x \equiv \mathcal{M}', x' \Rightarrow \mathcal{M}, x \underline{\leftrightarrow}\mathcal{M}', x'$ (Hennessy - Milner)
		- $\equiv$ often written as $\leftrightsquigarrow$
		- $\mathcal{M}, x \equiv \mathcal{M}', x' \Rightarrow \mathcal{M}, x \underline{\leftrightarrow}\mathcal{M}', x'$ often written as $x \equiv x' \Rightarrow x \underline{\leftrightarrow} x'$.
	- \[for $k \in ON$ the maximal complexity of a formula in $\mathcal{L}^k_{ML}$, a $k$-inductively defined modal logic, then $\forall_{x \in M}\forall_{x' \in M'} \mathcal{M}, x \equiv \mathcal{M}', x' \Rightarrow \mathcal{M}, x \underline{\leftrightarrow}^k \mathcal{M}', x'$ for $\underline{\leftrightarrow}^k$ the $k$-bisimulation, as defined in: [Overleaf: IML, 1](https://www.overleaf.com/read/qdtknhmjymqt#0a2005)\]
#### 17.09, Filtrations
- A (generated) submodel $\mathcal{M}'$ of $\mathcal{M}$ is a model s.t.
	1. ==?==
	2. $R' = R \cap (W' \times W')$
	3. $V'(p) = V(p) \cap W'$ 
	(4.) $(x \in W' \to ...) ==?==
	- $\mathcal{M'}$ is gen.sub, of $\mathcal{M}$, $x \in W'$, then $\mathcal{M}, x \underline{\leftrightarrow} \mathcal{M}', x$
	- for $\mathcal{M}$, $\mathcal{M}'$ models, $f: W \to W'$ is a bounded morphism if:
		1. $\forall_{p \in Prop}\mathcal{M}, x \models p \Leftrightarrow \mathcal{M'}, f(x) \models p$
		2. $x R y \Rightarrow f(x) R' f(y)$
		3. $f(x) R' x' \Rightarrow \exists_{y \in W} x R y \land f(y) = x$
	- for $\mathcal{M}, \mathcal{M}'$ models, $f: W \to W'$ a bound.morph., then $\mathcal{M}, x \underline{\leftrightarrow} \mathcal{M}', f(x)$
	- for $\{\mathcal{M}_i\}_{i \in I}$ for $\mathcal{M}_i$ model, the disj.union is a model $\mathcal{M}$ s.t.
		1. $W := \bigsqcup_{i \in I} W_i$, $R = \bigcup_{i \in I} R_i$, $V(p) = \bigcup_{i \in I} V_i(p)$ 
- [[Modal Logic (Lecture)#5. Finite Model Property]]:
	- let $\Sigma$ be a fin.set, cl.under subformulae
	- $W/\Sigma = \{[x]: x \in W\}$
		- $[x] =\{y \in W : x \leftrightsquigarrow y\}$
			- $x \leftrightsquigarrow y := \forall_{\varphi\in \Sigma}(\mathcal{M}, x \models \varphi \Leftrightarrow \mathcal{M}, y \models \varphi$
	- $g: W / \Sigma \to \mathcal{P}(\Sigma)$, $[x] \mapsto \{\varphi \in \Sigma : \mathcal{M},x \models \varphi\}$
	- the filtration model $\mathcal{M}^f$
		1. $W^f = W_\Sigma$
		2. $V^f(p) = \{[x]: \mathcal{M}, x \models p\}$
		3. $xRy \Rightarrow [x] R^f [y]$ 
		4. $[x]R^f[y] \Rightarrow \forall_{\lozenge \varphi \in \Sigma}(\mathcal{M}, y \models \varphi \Rightarrow \mathcal{M}, x \models \lozenge \varphi)$
	- $\forall_{\varphi \in Sigma} \forall_{x \in W} \mathcal{M}, x \models \varphi \Leftrightarrow \mathcal{M}^f, [x] \models \varphi$