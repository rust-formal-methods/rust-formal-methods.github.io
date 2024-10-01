+++
title = "Towards Sound `unsafe` Rust"
date = 2024-10-28T19:00:00+02:00
+++

Rust guarantees memory safety and data race freedom through its type checker, which enforces *ownership* and *borrowing* rules. However, adhering strictly to these rules can limit expressiveness and restrict certain high-performance implementations. To address this limitation, Rust allows programmers to relax some type system checks within `unsafe` blocks. The challenge, however, is that maintaining type system invariants within these relaxed blocks becomes the programmer's responsibility.

Although the use of `unsafe` blocks is not uncommon in Rust crates, writing sound `unsafe` code remains difficult. There are numerous obligations that programmers must fulfill, many of which are easy to overlook, leading to bugs that are difficult to detect. We have extended *VeriFast*, a verification tool based on *modular symbolic execution*, to verify that Rust's safety guarantees hold in programs containing `unsafe` blocks. Using this tool, we have successfully verified approximations of several well-known, fundamental components from Rust's standard library, along with other examples, all of which make use of `unsafe` code.

**Presenter**:

Felix has been working on the Rust compiler since before Rust 1.0; he was co-lead of the Rust compiler team from 2019 until 2023. Felix has taken on this work as part of a broader interest in enforcing safety and correctness properties for Rust code.

**Meeting Link**: TBA

**Recording Link**: TBA