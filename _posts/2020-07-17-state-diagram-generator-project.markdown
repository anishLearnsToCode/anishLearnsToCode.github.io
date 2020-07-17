---
title: "State Diagram Generator"
layout: post
date: 2020-04-23 18:07
tag: theory-of-automata
image: https://github.com/anishLearnsToCode/anishLearnsToCode.github.io/tree/master/assets/images/projects/state-diagram-generator/dfa.png
headerImage: false
projects: true
hidden: true # don't count this post in blog pagination
description: "This is a web application that takes regular expressions as Inputs and creates corresponding Finite Automata - both Deterministic (DFA) and Non-Deterministic (NFA) as an output. Correspondingly also outputs the transition state diagram for the Deterministic Finite State Machine (DFA)."
category: project
author: anish_sachdeva
externalLink: false
---

# State Diagram Generator

See project on [GitHub](https://github.com/anishLearnsToCode/state-diagram-generator) :octocat: and deployed 
[here](state-diagram-generator.web.app/) 🌐. 

This project has been created to display the deterministic finite state automata (DFA) or the Non-Deterministic Finite 
State Automata (NFA) of any given valid regular expression.

A deterministic automata along with it's transmission table will be generated for the given regular expression and the 
user can also check whether any given string is recognized by that particular regular language.

## Motivation 

The first purpose of building this web application was to show to the user the synonymity
of the regular expression, the finite state machine and the transition table and how they
can be used to recognize the same language.

The application aims to provide the user with a visual representation for all valid regular
expressions in the form of deterministic or nondeterministic automata as this helps the
user (even me, the author) - better understand machines and their corresponding regular
languages.

This also helps the user understand how to build finite state machines from regular
expressions better. The instantaneous state transition diagram tool also shows the states
and next states for all possible symbols.
The regular expression parser and string checker tool can then be used to check strings
against the regular expression and the finite state machine and this text box was added to
provide the user with a way to parse and check presence of strings in any given language in
linear time.

Another motivation behind this application was to provide a visual interface that clearly
shows the difference between the deterministic and non-deterministic finite state
automata for the same regular expression (same regular language) and this difference
seen visually can help users learn better how different machines with different number of
states and different transitions can represent the same language.

Another motivation of building this web application was to provide future developers an
interface over the DotScript Language that can be used to create finite state automatas.
This web application is open source and can be viewed and extended by other developers.
Other developers can build on this application and further extend it by adding features
such as support for push-down automata, compiling and lexical parsing directly using the
textbox for string checking to compile entire projects in different languages.

## Finite Automata

A finite automaton is a 5-tuple _(Q, &Sigma;, &delta;, q, F)_ where
- _Q_ is a finite set called the states
- _&Sigma;_ is a finite set called the alphabet.
- _&delta; : Q &times; &Sigma; →  Q_ is the transition function.
- _q ∈  Q_ is the start state.
- _F ⊂  Q_ are the acceptance states. 
