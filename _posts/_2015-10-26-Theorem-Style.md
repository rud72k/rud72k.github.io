---
layout: post
title: "Theorem Style Command"
description: "LaTeX setting for theorem style"
tags: 
- latex
- theorem style
- setting
- preamble
---


The amsthm package supports the notion of a current theorem style, which determines what will be produced by a given newtheorem command. The three theorem styles provided, plain, definition, and remark, receive different typographical treatment that gives them visual emphasis corresponding to their relative importance. The details of this typographical treatment may vary depending on the document class, but typically the plain style produces italic body text, while the other two styles produce roman body text.

To create new theorem-like environments in the different styles, divide your newtheorem commands into groups and preface each group with the appropriate theoremstyle. If no theoremstyle command is given, the style used will be plain. Some examples:

~~~

\theoremstyle{plain}% default
\newtheorem{thm}{Theorem}[section]
\newtheorem{lem}[thm]{Lemma}
\newtheorem{prop}[thm]{Proposition}
\newtheorem*{cor}{Corollary}
\newtheorem*{KL}{Klein's Lemma}

\theoremstyle{definition}
\newtheorem{defn}{Definition}[section]
\newtheorem{conj}{Conjecture}[section]
\newtheorem{exmp}{Example}[section]

\theoremstyle{remark}
\newtheorem*{rem}{Remark}
\newtheorem*{note}{Note}
\newtheorem{case}{Case}

~~~

This article originally appear in [here](http://www.nada.kth.se/~carsten/latex/amsldoc/node63.html) 
