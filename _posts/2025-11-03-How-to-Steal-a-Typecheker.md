---
layout: post
title:  "How to Steal a Typecheker" 
speaker: "Dr. Artem Sinkarovs"
location: "Building 59P, Room 1003"
time: "12:00 - 13:00"
---

# Abstract
Conventional definitions of a programming language proceed by first specifying
an untyped syntax and subsequently constructing a type‑checker that eliminates
some of the syntactically admissible but semantically invalid programs. When
dependent types are employed, these two stages can be merged: the language is
defined simultaneously with its typing rules, guaranteeing that ill‑typed terms
cannot even be expressed. This approach is commonly known as an
intrinsically‑typed encoding.

In this talk I will use Agda as the host language and present two
intrinsically‑typed encodings of DSLs:

1.   an encoding based on de Bruijn indices, and
2.   an encoding based on higher‑order abstract syntax.

The session will be a live‑coding demonstration. Prior exposure to Agda may be
helpful, but it is not a prerequisite, as all the techniques are transferable
to other dependently‑typed systems.
