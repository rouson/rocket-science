---
title: 'Rocket Science: An Exercise in Refactoring Legacy Fortran'
tags:
  - Fortran
  - refactoring
  - rocket
authors:
  - name: Damian Rouson
    orcid: 0000-0002-2344-868X
    affiliation: 1
  - name: Brad Richardson
    orcid: 0000-0002-3205-2169
    affiliation: 1
  - name: Brian Laubacher
    affiliation: 2
affiliations:
 - name: Sourcery Institute
   index: 1
 - name: Autoliv
   index: 2
date: 2 December 2020
bibliography: paper.bib
---

# Summary

The near ubiquity of object-oriented programming support in modern programming languages
and the continued utility of legacy, procedural Fortran in important application domains
combine to make object-oriented design a common destination of code modernization efforts.
As Fortran has evolved into a multi-paradigm language, however, the peer-reviewed literature
contains far fewer detailed considerations of Fortran's support for functional programming.
This paper explores the symbiotic relationship between the two by demonstrating a legacy
code refactoring strategy in which the aim of writing pure functions motivates the choice
of abstractions and the ability to encapsulate function results facilitates the writing
of pure functions.  We show how a Fortran feature typically used for aliasing can be
applied to ensure the immutability of state.  We apply the resulting code refactoring
strategy to the modernization of an open-source pedagogical tool: a rocket motor
simulation mini-application.  We describe (1) the original, procedural Fortran 90 program
that uses global data, (2) a ground-up reimplementation of the same algorithms using
object-oriented design patterns in Fortran 2018, and (3) an evolutionary refactoring
that uses a consistent methodology for deriving purely functional abstractions from the
Fortran 90 code.  We contrast the two modern designs and demonstrate an evolutionary
path that could naturally lead the same resulting design for the ground-up reimplementation
and the evolutionary refactoring.

# Statement of need

The most highly cited article on refactoring Fortran is "Refactorings
for Fortran and high-performance computing" [@overbey2005refactorings].

# Acknowledgements

# References
