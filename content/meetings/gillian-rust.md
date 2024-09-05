+++
title ="Gillian-Rust: A hybrid approach to unsafe Rust verification"
date = 2024-05-25
+++

The Rust Formal Methods Interest group has seen several talks about scalable verification of safe Rust (Prusti, Creusot, Aeneas, Flux…), and other analyses that leverage the guarantees provided by the Rust type and borrow checker (Flowistry, RusSOL…). However, there has been little work on the verification of unsafe Rust, which requires techniques that do not scale as well to large programs. In this talk, we propose a hybrid approach to Rust verification, where safe code is verified by Creusot, and unsafe code is verified by a prototype tool called Gillian-Rust. At the core of this approach is the ability of Gillian-Rust to interpret and verify specifications that Creusot is able to use but not verify.

--- 

About the Speaker

Sacha Ayoun is a PhD student at Imperial College London, under the supervision of Prof. Philippa Gardner. He has been working on the Gillian verification framework, and is now its lead developer. His research covers all aspects of Gillian, from its meta-theory to its most real-world use-cases, with a focus on applications to C and more recently Rust. On his free time, you may find him rollerblading around London or complaining about British food.