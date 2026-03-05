---
layout: post
title:  "When Agda Met Vampire"
speaker: "Dr. Artjoms Šinkarovs and Dr. Michael Rawson"
location: "Building 32, Room 3079"
time: "13:00 - 14:00"
---

A talk given by Artoms Šinkarovs and Michael Rawson on their work integrating Vampire with Agda.

# Abstract
Dependently-typed proof assistants furnish expressive foundations for mechanised mathematics
and verified software. However, automation for these systems has been either modest in scope or
complex in implementation. We aim to improve the situation by integrating proof assistants with
automated theorem provers (ATPs) in a simple way, while preserving the correctness guarantees of
the former. A central difficulty arises from the fact that most ATPs operate in classical first - order
logic, whereas these proof assistants are grounded in constructive dependent type theory. We
identify an expressive fragment of both languages—essentially equational Horn—that admits sound,
straightforward translations in both directions. The approach produces a prototype system for Agda
forwarding proof obligations to the ATP Vampire, then transforming the resulting classical proof
into a constructive proof term that Agda can type- check. The prototype automatically derives proofs
concerning the properties of a complex field equipped with roots of unity, which took professional
Agda developers two full days to complete. The required engineering effort is modest, and we
anticipate that the methodology will extend readily to other ATPs and proof assistants.
