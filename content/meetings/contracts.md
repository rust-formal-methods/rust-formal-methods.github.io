+++
title = "Contracts in Rust"
date = 2024-09-24
+++
**Title**: 

**Abstract**:

As the growing number of verification tools (Aeneas, Creusot, Kani, Prusti, Verus, ...) has shown, there is a growing community for formal verification of Rust code. 
Each of these tools needs to re-invent a specification language, leading to a rapidly fragmenting ecosystem of incompatible languages and tools.
To address this and related challenges, a Major Change Proposal was proposed to integrate support for contracts and invariants into Rust.
But what does this mean? 

Today, current tools must either embed a whole additional specification language via macros, or attemt to parse contracts from `assert!` and related features.
Both solutions leave a lot to be desired, as this makes it difficult for users to use these tools, while also hindering the development of said tools.
It also means that each tool has its own language, making interoperability hard.

The shiny future we are aiming for is one in which ordinary Rust programmers are writing contracts as part of every day Rust to be verified with dynamic (and static) tools.	
Rather than building their codebase around a single verifier, they can just "plug in" different verifiers, reusing the majority of their contracts. 

In this talk we present a vision for how we might get to this future, and some of the steps we can take on the way there.

**Presenter**:

Felix has been working on the Rust compiler since before Rust 1.0; he was co-lead of the Rust compiler team from 2019 until 2023. Felix has taken on this work as part of a broader interest in enforcing safety and correctness properties for Rust code.

**Meeting Link**:

**Recording Link**: