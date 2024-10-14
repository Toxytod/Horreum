Here is the code I usually add to all documents created after October 2024 which makes typing in $\LaTeX$ easier and quicker. I also implemented the _gaming cards symbols_ which I find funny to use.

``` LaTeX
\documentclass[12pt]{article}
\usepackage{amsmath, amssymb, amsfonts, amsthm, mathtools}
\usepackage{geometry}
\geometry{margin=1in}
\usepackage{graphicx}
\usepackage{tikz}
\usepackage{xcolor}
\usepackage{csquotes}
\usepackage{enumerate}
%\usepackage{stix2}
\usepackage{hyperref}
\usepackage{wasysym}

\newcommand{\fbS}{\textcolor{black}{\spadesuit}} 
\newcommand{\ebS}{\textcolor{black}{\varspadesuit}} 
\newcommand{\frS}{\textcolor{red}{\spadesuit}} 
\newcommand{\erS}{\textcolor{red}{\varspadesuit}} 

\newcommand{\fbH}{\textcolor{black}{\heartsuit}} 
\newcommand{\ebH}{\textcolor{black}{\varheartsuit}} 
\newcommand{\frH}{\textcolor{red}{\heartsuit}} 
\newcommand{\erH}{\textcolor{red}{\varheartsuit}} 

\newcommand{\fbD}{\textcolor{black}{\diamondsuit}} 
\newcommand{\ebD}{\textcolor{black}{\vardiamondsuit}} 
\newcommand{\frD}{\textcolor{red}{\diamondsuit}} 
\newcommand{\erD}{\textcolor{red}{\vardiamondsuit}} 

\newcommand{\fbC}{\textcolor{black}{\clubsuit}} 
\newcommand{\ebC}{\textcolor{black}{\varclubsuit}} 
\newcommand{\frC}{\textcolor{red}{\clubsuit}} 
\newcommand{\erC}{\textcolor{red}{\varclubsuit}} 

\renewcommand{\b}[1]{\mathbb{#1}}
\renewcommand{\c}[1]{\mathcal{#1}}
\newcommand{\f}[1]{\mathfrak{#1}}
\newcommand{\vf}{\varphi}
\newcommand{\p}{\psi}
\newcommand{\fa}[1]{\forall_{#1}}
\newcommand{\ex}[1]{\exists_{#1}}
\renewcommand{\a}{\land}
\renewcommand{\o}{\lor}
\newcommand{\n}{\lnot}
\newcommand{\Cat}{\textbf{Cat}}
\newcommand{\Set}{\textbf{Set}}
\newcommand{\subs}{\subseteq}
\newcommand{\sups}{\supseteq}
\newcommand{\sq}{\Box}
\newcommand{\dm}{\lozenge}
\newcommand{\q}[1]{\enquote{#1}}
\newcommand{\txr}[1]{\textcolor{red}{#1}}
\newcommand{\txb}[1]{\textcolor{blue}{#1}}
\newcommand{\md}{\models}
\newcommand{\vd}{\vdash}
\newcommand{\forces}{\vDash}
\newcommand{\az}{\aleph_0}
\newcommand{\fca}{for contradiction assume }
\newcommand{\Fca}{For contradiction assume }
\newcommand{\fn}[1]{\footnote{#1}}
\newcommand{\To}{\Rightarrow}
\newcommand{\oT}{\Leftarrow}
\newcommand{\ToT}{\Leftrightarrow}
\newcommand{\ot}{\leftarrow}
\newcommand{\tot}{\leftrightarrow}
\newcommand{\Prop}{\text{Prop}}
\newcommand{\Atom}{\text{Atom}}
\newcommand{\FV}{\text{FV}}
\newcommand{\FOL}{\mathcal{L}_{FOL}}
\newcommand{\PL}{\mathcal{L}_{PL}}
\newcommand{\Le}{\mathcal{L}_{\epsilon}}

\theoremstyle{definition}
\newtheorem{Definition}{Definition}[section]
\newtheorem*{definition}{Definition}
\newtheorem{Exercise}[Definition]{Exercise}
\newtheorem*{exercise}{Exercise}


\theoremstyle{plain}
\newtheorem{Theorem}[Definition]{Theorem}
\newtheorem{Lemma}[Definition]{Lemma}
\newtheorem{Corollary}[Definition]{Corollary}
\newtheorem*{corollary}{Corollary}
\newtheorem*{theorem}{Theorem}
\newtheorem*{lemma}{Lemma}

\theoremstyle{remark}
\newtheorem{Remark}[Definition]{Remark}
\newtheorem*{remark}{Remark}
\newtheorem{Quest}[Definition]{Question}
\newtheorem*{quest}{Question}
\newtheorem{Hypothesis}[Definition]{Hypothesis}
\newtheorem*{hypothesis}{Hypothesis}

\newenvironment{happyproof}[1][\proofname]
{\renewcommand\qedsymbol{\smiley{}}\proof[#1]}
{\endproof}

\newenvironment{argument}[1][\proofname]
{\renewcommand\qedsymbol{}\proof[#1]}
{\endproof}

\newenvironment{proof sketch}[1][\proofname]
{\renewcommand\qedsymbol{}\proof[#1]}
{\endproof}

\hypersetup{
    colorlinks=true,
    linkcolor=blue,
    urlcolor=blue,
    citecolor=blue,
    pdfborder={0 0 0}
}

\author{Simone Testino}
\date{\today}
```