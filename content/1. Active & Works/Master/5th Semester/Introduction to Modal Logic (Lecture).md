---
draft: 
date: 2024-09-30
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
#### From the Book
- $\tau = (O, \rho)$ is a _modal similarity type_ for $O \not = \emptyset$, $\rho: O \to \mathbb{N}$, 1.11
	- elements of $O$ are _modal operators_
		- use $\triangle_0, \triangle_1, ...$ to denote its elements.
			- for $i \in \mathbb{N}$, $\triangledown_i(\varphi_1, ..., \varphi_n) := \lnot \triangle_i (\lnot \varphi_1, ..., \lnot \varphi_n)$ 
	- $\rho$ assigns to each operator $\triangle$ a finite arity.
- $ML(\tau, \Phi)$ is a _modal language_ for $\tau = (O, \rho)$ and a set of prop.lett $\Phi$, 1.12
	- $Form(\tau, \Phi)$ is given by $\langle p | \bot | \lnot \varphi | \varphi_1 \land \varphi_2 | \triangle (\varphi_1, ..., \varphi_{\rho(\triangle)}) \rangle$ 
- $\tau$-type at $w$ is $\{\varphi : \mathcal{M}, w \models\varphi\}$, 2.1
	- two $\tau$-types at $w$ and $w'$, for $w \in M, w' \in M'$, s.t. $\mathcal{M}, \mathcal{M}'$ have same mod.sim.type $\tau$, write $w \leftrightsquigarrow w'$ if $\tau$-type.$w$ is $\tau$-type.$w'$.
	- $\mathcal{M} \leftrightsquigarrow \mathcal{M}'$ iff $\bigcap_{w \in M} \{\varphi : \mathcal{M}, w \models\varphi\} = \bigcap_{w' \in M'} \{\varphi : \mathcal{M}', w' \models\varphi\}$
	- $\mathcal{M} \bigsqcup \mathcal{N}$ preserves all information.
- for $\tau$ mod.sim.type, $\mathcal{M}_i$ $\tau$-models, then $\forall_{\varphi \in \mathcal{L}_{\tau-ML}}\forall_{i \in I} \forall_{w \in M_i} \mathcal{M}_i, w \models \varphi \Leftrightarrow \bigcup_{i \in I}\mathcal{M}_i, w \models \varphi$, 2.3
#### 17.09, Filtrations
- A (generated) submodel $\mathcal{M}'$ of $\mathcal{M}$ is a model s.t.
	1. $W' \subseteq W$ 
	2. $R' = R \cap (W' \times W')$
	3. $V'(p) = V(p) \cap W'$ 
	(4.) $(w \in W' \land wRv) \to v \in W'$ 
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
#### 24.09, IV.
- a tree $(T,S)$ is a frame s.t. 
	1. $T$ is _rooted_ (i.e. $\forall_{t \in T}\exists!_{r \in T} rS^*t$)
		1. for $S^*$ the refl.trans.cl. of $S$
	2. $\forall_{t \in T} t \not = r \to \exists!_{t' \in T} t' S t$
	3. $\forall_{t \in T} \lnot t S^+ t$
		1. for $S^+$ the trans.cl. of $S$
- for $\mathcal{M} = (W, R, V)$, ex. $\mathcal{T} = (T, S, V)$ s.t. $f: T \to V$ surj. bounded morphism.
- a path in $\mathcal{M}$ is a seq. $(r, u_1, ..., u_n)$ s.t. $u_i R u_{i + 1}$ 