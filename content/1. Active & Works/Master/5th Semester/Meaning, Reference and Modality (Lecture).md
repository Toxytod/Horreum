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
- **Extensional Semantics**: meaning is reference
	- $M, g \models \phi$; $M \models \phi$; $\models \phi$; $\Gamma \models \phi$
		- (satisfaction, truth, validity, entailment)
	- "Fido"$\mapsto Fido$
		- "Fido is a boy"$\mapsto 0$ iff $Fido \not \in Boys$ 
		- "All boys swim"$\mapsto 1$ iff $Boys \subseteq Swimmers$ 
	- Principles:
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
- _intensional semantics_: meaning is determination of reference
	- $M, w , g \models \phi$; $M, w \models \phi$; $(F) \models \phi$; $\Gamma \models \phi$
- _dynamic semantics_: meaning is potential to update information
	- $M, \langle g , h \rangle \models \phi$; $M, g \models \phi$; $\models \phi$; $\vec{\gamma} \models \phi$ 
- *Frege*: Sinn und Bedeutung
	- Morning/Evening star
#### 13.09, II. Basics in Modal Logic
- Already seen material
	- [[Modal Logic (Lecture)]]
		- [[Modal Logic (Lecture)#13. Epistemic Logic]]
	- [[Introduction to Modal Logic (Lecture)]]
- **Frege**: every word has a reference (B.) and a meaning (S.)
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
		- everything that is content dependent must be encoded in the thought so that the thought is context-indipendent.
			- (this can, for instance, not happen with the representation of yourself, see [[The Frequency of Telling Stories]])
#### 17.09, III. Worlds
- _Quine_: $\square \varphi \equiv$ "$\varphi$" is analythic
- _Lewis_: Modal Realism
	- "_things could have been different_" $\Rightarrow$ "there are _ways things could have been_"
	- _Stalnaker_: modal realism is just "_some ordinary beliefs by another name_"
	- It is a natural belief and there is no problem with it.
	- Actuality is Indexical: our world is one among others.
	- _Stalnaker_: 
		1. Possible worlds exist
		2. they are of the same sort of the actual world
		3. actuality is an indexical notion
		4. possible worlds are irreducible 
			- but can be given a naturalistic explanation
	- In some sense $b \rightsquigarrow \bigwedge \{P : P(b)\}$ 
		- cannot be "$=$"
	- _Solopsism_: deny most things, _presentist_ the future and past, _actualist_ is inclusive
#### 20.09, IV A. Prior
- He gave foundations of temporal logic as a modal logic
- Prior: _Wheresoever then is whatsoever is, it is only as present_ (mentioning S. Augustine)
- 