---
draft: 
date: ""
---
I followed this course by, Prof. Dekker during my [[5th Semester]] at the [[University of Amsterdam]] for my [[M.Sc. Logic (UvA)]]. 

Relevant courses in [[Index of Bachelor Works#Philosophy of Language]] I took are just the one on Kripke (see: [[The Frequency of Telling Stories]], on Kripkean reference of the indexical "I") and in Philosophy of Logic (see: [[The Silent Assumption in Tarskian Semantics]]).
#### Take-Home Exams
- [Overleaf: MRM, 1](https://www.overleaf.com/read/vjmbbgpmktnw#9851a5)
- [Overleaf: MRM, 2](https://www.overleaf.com/read/vpsffhvnmnhg#8adcdc)
- [Overleaf: MRM, 3](https://www.overleaf.com/read/fvzshcmnnfck#558c90)
## Lecture Notes
#### 10.09, I. Introduction
[[MRM Slides A.pdf]]
- **Formal Semantics**
	- In order to do any formal semantics, one should assume:
		1. There is structure in the world
		2. There is meaning in the world
		3. There is structure in meaning
			- doubtable. Compositionality, entailment, aprioricity
- _Extensional Semantics_: meaning is reference
	- _einen Satz verstehen, heißt, wissen was der Fall ist, wenn er wahr ist._ (L. Wittgenstein)
	- $M, g \models \phi$; $M \models \phi$; $\models \phi$; $\Gamma \models \phi$
		- (satisfaction, truth, validity, entailment)
	- "Fido"$\mapsto Fido$
		- "Fido is a boy"$\mapsto 0$ iff $Fido \not \in Boys$ 
		- "All boys swim"$\mapsto 1$ iff $Boys \subseteq Swimmers$ 
	- _Extensionality Principles_:
		- $t = t' \models \varphi \leftrightarrow [t'/t]\varphi$
		- $\forall_{x}(A(x) \leftrightarrow A'(x)) \models \varphi \leftrightarrow [A'/A]\varphi$
		- $\psi = \psi' \models \varphi \leftrightarrow [\psi'/\psi]\varphi$
		- same reference $\leftrightarrow$ same meaning
	- Problems:
		- _Identity_: Lois doesn't know that Leningrad is Saint Petersburg
			- equivalent to: Lois doesn't know that SP is itself
		- _Existence_: Rumpelstiltskin does not exist
			- you cannot use the word without reference
		- _Substitution_: it is necessary that 9 is 9, planets are 9, hence nec. there are 9 planets
	- possibility of a sentence is given by:
		1. the atomic propositions that are true there
			- determined by the valuation function $V_w(p) \in \{0, 1\}$
		2. what is its space of possibilities
			- determined by $R$
- _intensional semantics_: meaning is determination of reference
	- _meaning as information_ (J. Hintikka)
	- $M, w , g \models \phi$; $M, w \models \phi$; $(F) \models \phi$; $\Gamma \models \phi$
- _dynamic semantics_: meaning is potential to update information
	- $M, \langle g , h \rangle \models \phi$; $M, g \models \phi$; $\models \phi$; $\vec{\gamma} \models \phi$ 
#### 13.09, II. Frege & Basics in Modal Logic
- Basic Modal Logic: already seen material
	- [[Modal Logic (Lecture)]]
		- [[Modal Logic (Lecture)#13. Epistemic Logic]]
	- [[Introduction to Modal Logic (Lecture)]]
- **Frege**: _Gedanke are neither things from the external world, not Vorstellungen. A third realm has to be acknowledged._
- Each word (Syntax) is mapped to a Bedeutung (World) and a Sinn (3rd Realm)
- If $a = b$ then $S(a) = S(b)$ (Compositionality)
	- Clar Kent works for the Local Herald $\not =$ Superman works for te Daily Planet
		- Same Bedeutung (compositionality on Bedeutung applied)
		- Different Sinn, no compositionality on Sinn has been applied
			- Hence _Gedanke_ is not Bedeutung.
- _Sinn as Mode of Presentation_
- a thought (G.) is _what is true or false_
	- Examples
		- $a^2 + b^2 = c^2$
		- Venus follows an elliptic orbit around the sun
		- Circe has drugged Odysseus' men
	- not a picture, not a sentence, that thing that is true or false
		- Thought and truth cannot be better defined.
	- _unchangeable_, not psychological but "metaphysical"
		- very close to _modern Platonism_
			- thoughts are metaphysical and hyperuranical entities
				- real, with determinate truth values and consequences relations, timeless and without location.
		- everything that is content dependent must be encoded in the thought so that the thought iscontext-indipendent.
		- (this can, for instance, not happen with the representation of yourself, see [[The Frequency of Telling Stories]])
	- Leibniz: _Eadum sunt, quae sibi mutuo substitui posunt, salva veritate._
		- Quotations:
			- _direct_: expressions refer to themselves
			- _indirect_: expressions refer to their ordinary sense
				- the _Sinn_ is the _Bedeutung_ of that sentence in indirect use.
#### 17.09, III. Worlds
- _Quine_: $\square \varphi \equiv$ "$\varphi$" is analythic
- Extremes:
	- _Leibniz_: all worlds certainly exist
	- _Quine_: nihilist, there are none.
- _Lewis_: Modal Realism
	- "_things could have been different_" $\Rightarrow$ "there are _ways things could have been_"
	- _Stalnaker_: modal realism is just "_some ordinary beliefs by another name_"
	- Actuality is Indexical: our world is one among others.
		1. Not a particular property of our world.
		2. We just believe to more things just like the actual world, nothing more.
		3. Only a systematic thinking about the possibilities we already know.
	- _Stalnaker_: possible worlds are "_some ordinary beliefs by another name_".
	- _Lewis on Ordinary Beliefs_:
		1. Belief in possible worlds is a natural belief
		2. There is no sensible alternative to this belief
		3. There is nothing wrong with the belief
	- _Stalnaker_ answers Lewis as:
		1. Possible worlds exist.
		2. They are of the same sort of the actual world.
			- Against:  $b \rightsquigarrow \bigwedge \{P : P(b)\}(b)$ is ok, not $b = \bigwedge \{P : P(b)\}$
				- the way the world is, is not the same thing as the world that is that way.
		3. Actuality is an indexical.
			- Against: but real
				- _The objective, absolute point of view is the view from within the actual world, and it is part of the concept of actuality that this should be so._
				- _Solopsism_: deny most things, _presentist_ the future and past, _actualist_ is inclusive
		4. Possible worlds are irreducible.
- Instrumentalist: "_Possible worlds are convenient fictions which help to make a workable and perspicuous theory_"
- **Frames**: as done in [[Introduction to Modal Logic (Lecture)]] &
	- From: [[Modal Logic (Lecture)]]
		- $\square \varphi \to \varphi$ corr. to refl.
		- $\varphi \to \square \lozenge \varphi$ corr. to sym.
		- $\square \varphi \to \square \square \varphi$ corr. to trans.
		- $\square \varphi \to \lozenge \varphi$ corr. to seriality
		- $\lozenge \varphi \to \square \lozenge \varphi$ corr. to euclideaness ($\forall_{u, v, w \in M}u R v \land u R w \to w R v)$
	- in S5: $\Diamond \square \phi \Leftrightarrow \square \phi \Leftrightarrow \square \square \phi$ and $\Diamond \Diamond \phi \Leftrightarrow \Diamond \phi \Leftrightarrow \square \Diamond \phi$, R is refl., trans., eucl.
#### 20.09, IV. A. Prior
- He gave foundations of temporal logic as a modal logic
- Prior: _Wheresoever then is whatsoever is, it is only as present_ (mentioning S. Augustine)
- Some Rules
	1. $S \Leftrightarrow S$ present
	2. $S$ future $\Leftrightarrow (S$ present$)$ future
	3. $S$ future $\Leftrightarrow (S$ future$)$ present
- Tenses as Temporal Operators:
	- $F$ ex. in fut., $G$ alw. in the fut.
	- $P$ ex. in past, $H$ alw. in the past.
- Temporal Logic (as in [[Modal Logic (Lecture)#9. Temporal Logic]])
	- $\models G \phi \leftrightarrow \lnot F \lnot \phi$ and $\models H \phi \leftrightarrow \lnot P \lnot \phi$ (Dualities)
	- $\models (p \to GPp)$, in the fut., pres. is past, $\models (p \to HFp)$, pres. is fut. of past. (Interaction Principles)
	- Limits: irrefl. and univ. cannot be characterised. That is though intuitive.
		- Time is possibly circular, and this is not here. Can we exclude parallel times?
#### 24.09, V. Kripke & Modal Predicate Logic
[[MRM Slides B.pdf]]
- Lecture based on _Naming and Necessity_, seen mostly in [[The Frequency of Telling Stories]].
- _a priori_ $\not \Leftrightarrow$ _necessary_
	- Goldenbach conjecture is nec. true or nec. false, it does not imply anything epistemic
- After Frege:
	- _Russel_: _Sinn_ can be captured in a _Description_
	- _Searl_: we need to have a _cluster_ of description of the same designator in different modalities
	- _Kripke_: names are rigid designators, definite descriptions must not be
		- _rigid designator_: "_if in every possible world it designates the same object_" (NN, p.48)
			- we need to make sense of "_criteria of transworld identity_"
			- Possible Worlds themselves are _stipulated_ because we can rigidly refer to objects
				- "if Biden didn't win elections", such a description of a possible world is possible _because_ we can _rigidly refer_ to Biden. (NN, p.49)
				- Q: if Biden rigidly refers to Biden, then Biden is necessarily named "Biden"
					- A: Biden is nec. Biden, but Biden is not nec. named "Biden". Two different languages, we can use our-own for practical purposes, must not be the same used in other worlds. "The person called Biden" is not a rigid designator.
					- {Q: should we develop a meta-language or just use the one true in @?}
				- Q: Sinn and Bedeutung of rigid names?
					- A: Bedeutung makes no sense, different domains, Sinn is not the proper way to think about it, (against Lewis) possible worlds are not already there, they are stipulated after we use names rigidly, that is what refers necessarily to objects in other worlds.
- **Predicate Modal Logic**\[I use here $\Vdash$ for `\backmodels` or `sledom` which are not in Markdown.\]
	- $D: W \to  \{D_{w_0}, D_{w_1}, ...\}, w \mapsto D_w$, $D_w$ is the _domain of individuals_ (Domain Function)
		- hence _existence is contigent_
	- $I$ interpretations are _rigid_, same in every world.
	- Valuations are _partial_, i.e. $\mathcal{M}, w, V \models \varphi$ or $\mathcal{M}, w, V \Vdash \varphi$ or neither
		- see [[Meaning, Reference and Modality (Lecture)#Alternative Semantics to Modal Predicate Logic]]
	- We use Weak Kleene Truth tables
		- if there is an undefined, then undefined.
	- **Semantics**
		- $\mathcal{M}, w \models R(t_1, ..., t_n)$ iff $[t_1]_{M, g} \in D_w$ and $\langle [t_1]_{M, g}, ..., [t_n]_{M, g} \rangle \in I_w(R)$
		- "same as above" $\Vdash$ "same as above" $\not \in$ "same as above"
		- $\mathcal{M}, w \models t_i = t_j$ iff $[t_i]_{M, g} \in D_w$ and $[t_i]_{M, g} = [t_j]_{M, g}$, similarly for $\not =$
		- $\mathcal{M}, w \models (\phi \land \psi)$ - classical and defined \[only?\]
		- $\mathcal{M},w \models \forall_x \phi$ iff $\forall_{d \in D_w} \mathcal{M}, w, V[x/ d] \models \phi$ 
		- "same" $\Vdash$ "same" $\Vdash \phi$, and for $\exists$ 
		- $\square$ as usual.
	- **Hard and Friendly Modality**
		- Hard Modality: $\mathcal{M}, w \models \square_h \varphi \Leftrightarrow \forall_{w' \in W} w R w' \to \mathcal{M}, w' \models \varphi$
			- $\mathcal{M}, w \Vdash \square_h \varphi \Leftrightarrow \forall_{w' \in W} w R w' \to \mathcal{M}, w' \Vdash \varphi$
			- $\not \models_h \square (a = a)$
			- $\not \models \square_h (Fa \to Fa)$ 
		- Friendly Modality: $\mathcal{M}, w \models \square_f \varphi \Leftrightarrow \forall_{w' \in W} (w R w' \land def.(\varphi)) \to \mathcal{M}, w' \models \varphi$
			- Distribution of $\square_f$ is not valid.
			- we could have $\square F(a)$ but $\Diamond \lnot \exists_x F(x)$ 
	- **String & Tolerant Modality**
		- $\Gamma \models_s \psi$ iff in all models $\forall_{w \in W}\forall_{\gamma \in \Gamma} (\mathcal{M}, w \models \gamma )\Rightarrow \mathcal{M}, w \models \phi$
			- formulae with individual terms are never valid
			- $F(a) \models_s F(a)$ but $\not \models_s (F(a)\to F(a))$ 
		- $\Gamma \models_p \psi$ iff $\psi$ is defined and in all models $\lnot \exists_{w \in W}\forall_{\gamma \in \Gamma} (\mathcal{M}, w \models \gamma )\Rightarrow \mathcal{M}, w \Vdash \phi$ 
		- Some Results: [[Some_Results_MPL.jpeg]]
	- **Barcan Formulae** &co
		- $\forall_x \Diamond F(x) \to \Diamond \forall_xF(x)$, no.
		- $\square \exists_x F(x) \to \exists_x \square F(x)$, no.
		- $\Diamond \forall_x F(x) \\to \forall_x \Diamond F(x)$, increasing domains
			- inc.dom., i.e. $\forall_{w, w'} w R w' \to D_w \subseteq D_{w'}$
			- alw. valid with "$\square_h$" and "$\models_t$"
		- $\exists_x \square F(x) \to \square \exists_x F(x)$
			- alw. valid with "$\square_h$" and "$\models_t$"
			- only of objects with necessary existence.
		- $\square \forall_x F(x) \to \forall_x \square F(x)$
			- valid with "$\square_h$" and inc.dom.
			- alw. valid with "$\square_f$"
		- $\exists_x \Diamond F(x) \to \Diamond \exists_x F(x)$
			- not valid with "$\models_s$" and "$\square_h$"
		- $\exists_x \Diamond_h F(x) \models_s \Diamond_h \exists_xF(x)$
		- $\square_h \forall_x F(x) \not \models_s \forall_x \square_h F(x)$ 
		- $\forall_x \square F(x) \to \square \forall_x F(x)$ decreasing domains (Barcan Formula)
			- dec.dom., i.e. $\forall_{w, w'} w R w' \to D_w \supseteq D_{w'}$
			- not valid with str.inc.dom.
		- $\Diamond \exists F(x) \to \exists_x \Diamond F(x)$ 
			- Quine: nonsense
			- others: if we can refer to smth, it must be there
#### 01.10, VI. Real, Possible and Impossible Objects
...

## Questions
### Alternative Semantics to Modal Predicate Logic
We have defined in [[Meaning, Reference and Modality (Lecture)#24.09, V. Kripke & Modal Predicate Logic]] the semantic that answers to the very natural question of how one can introduce first order logic in modal logic. Here I present a semantics that I claim to be equivalent to the presented one but that is simpler in two ways: (i) it does not require the introduction of three valued Weak Kleene Logic and (ii) it does not require the introduction of the reversed semantic consequence symbol.

**Idea**: To see the intuition, recall that for theories, instead of models, we already have an integrated way of having three truth values: that is (i) $T \models \varphi$, or (ii) $T \models \lnot \varphi$ or (iii) $T \not \models \varphi$ and $T \not \models \lnot \varphi$. This though cannot be directly applied to pointed modal models. That is, because models are complete and therefore the case (iii) is excluded.^[1] 

Consider this slight edit (that is sometimes already implicitly used in mathematical praxis) where for a sequence of symbols that are not in the language, call it $\delta$, we have $T \not \models \delta$. (alternatively, one may say that the whole formula $T \models \delta$ is not defined, I want it now to be defined and false).

Now, for each world construct a first order language whose terms are variables and the associated domain $D_w$ (the same defined in class), call such a language $\mathcal{L}^w$ (in the construction I currently give, these languages solely differ in the constants accepted in the domain, one might consider other differences though) . That is when we write "$\mathcal{M}, w \models_w \varphi$" we use "$\models_w$" which is the consequence relation^[2] of the language $\mathcal{L}^w$.

To see that Week Kleene Logic is applied, is fairly easy: for $\delta \notin \mathcal{L}^w$ and $\varphi \in \mathcal{L}^w$, we derive $\delta \circ \varphi \notin \mathcal{L}^w$ for any connective $\circ$, similarly for negation. For instance, $\mathcal{M}, w \not \models \varphi \land \delta$. Examples of such $\delta$ would be those formula that would be well formed but contain names of objects that are not in the domain of the world. In general we can state $\forall_{d \in \bigcup_{v \in W} D_v}(d \not \in D_w \land d \in \delta )\to \mathcal{M}, w \not \models \delta$.^[3]

Also note that, for $a \not \in \bigcap_{w \in W}D_w$, I have $\not \models (a = a)$ since for $a \not \in D_w$, then $\mathcal{M}, w \not \models a = a$. Though I always have $\models \forall_{x} x = x$ (since it is equivalent to $\forall_{w \in W} \models_w \forall_{x \in D_w} x = x$) and hence also $\models \square \forall_{x = x}$ since $D_w \not = \emptyset$.

**Questions**
1. Do you agree that this semantics is completely equivalent with the one seen in class?
2. Do you agree on the better simplicity in defining the semantics in this way?
3. Do you see any philosophical / foundational concern that one should take care of and which may make this semantics differ to the one presented in class?

[1]: this point already may not be 100% coherent with the way Kripke sees possible worlds, but that is another matter <br>
[2]: it may now be better to consider the syntactic relation rather than the semantic one, since it is essentially language-dependent and generally would _feel more appropriate_.<br>
[3]: here I write $d \in \delta$ because I consider $\delta$ to be an ordered set of symbols, hence I mean $d$ to be a symbol within the sentence $\delta$.

**Re:** by [Soeren Knudstorp](https://knudstorp.github.io/).<br>
If I’ve understood your suggestion correctly, your proposed semantics wouldn’t be equivalent. For instance, since you have only one constant for each element of a given domain, you wouldn’t be able to express statements like $h=p$ (‘Hesperus is Phosphorus’), but only express $v=v$ ('Venus is Venus’). 

**My Reply**:<br>
I first try to make to make clear to myself how statements like $h = p$ are possible in the predicate modal logic seen in class, and then note that, to my understanding, there is no difference in forming such statements in "_mine_" or in the _given_ semantics. <br>
To begin, in order to construct the statement ‘Hesperus is Phosphorus’ we wish to have variables $h, p$ that _denote_ the same object. Since we have taken names to refer rigidly, we have the general principle that each name, that is a constant $d \in \bigcup_{w \in W}D_w$, always refers to the _same object_ when interpreted in the different worlds. More precisely, that is for constants $h, p \in \bigcup_{w \in W} D_w$ we have that for every Kripke model $\mathcal{M}$,  $\forall_{w \in W} h, p \in D_w \to (\mathcal{M}, w \models h = p)$. Now, such a construction is similarly valid in the semantics I have given without any difference that I can see. 

A crucial difference is that the semantic I described gives the hard modality since $\varphi \not \in \mathcal{L}^w \to \square \varphi \not \in \mathcal{L}^w$ and also strict validity since for every Kripke model $\mathcal{M}$ I have $\forall_{\varphi \in \bigcup_{w \in W}\mathcal{L}^w} \forall_{w \in W} \varphi \not \in \mathcal{L}^w \to (\mathcal{M}, w \not \models \varphi)$. In fact, I do not prove results like "$\models a = a$", since for $a \not \in D_w$ it would not hold.

Defining tolerant modality is easily doable by changing again the semantics of "$\models$", one can in fact set it so that when the consequent is not defined the whole formula containing "$\models$" is true.

Defining friendly modality is though way less natural, since for any formula $\varphi \not \in \mathcal{L}^w \to \square \varphi \not \in \mathcal{L}^w$ and this can only be avoided by changing again the semantics of "$\models$" but buy setting more intricate syntactic rules.