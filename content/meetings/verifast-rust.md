+++
title = "Towards Sound `unsafe` Rust"
date = 2024-10-28T19:00:00+02:00
+++

Rust guarantees memory safety and data race freedom through its type checker, which enforces *ownership* and *borrowing* rules. However, adhering strictly to these rules can limit expressiveness and restrict certain high-performance implementations. To address this limitation, Rust allows programmers to relax some type system checks within `unsafe` blocks. The challenge, however, is that maintaining type system invariants within these relaxed blocks becomes the programmer's responsibility.

Although the use of `unsafe` blocks is not uncommon in Rust crates, writing sound `unsafe` code remains difficult. There are numerous obligations that programmers must fulfill, many of which are easy to overlook, leading to bugs that are difficult to detect. We have extended *VeriFast*, a verification tool based on *modular symbolic execution*, to verify that Rust's safety guarantees hold in programs containing `unsafe` blocks. Using this tool, we have successfully verified approximations of several well-known, fundamental components from Rust's standard library, along with other examples, all of which make use of `unsafe` code.

**Presenter**: Nima Rahimi Foroushaani is a PhD student affiliated with the DistriNet research unit within the Department of Computer Science at KU Leuven, under the mentorship of Prof. Dr. Bart Jacobs, since 2022.
He earned his master's degree in Computer Engineering, specializing in Computer Systems Architecture, in 2012.

His research endeavours centre around devising methodologies for verifying the desired properties of programming languages and computer programs. Currently, his concentration lies in verifying the safety properties of programs coded in the Rust programming language.

**Meeting Link**: TBA

**Recording Link**: TBA