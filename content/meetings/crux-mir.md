+++
title = "CRUX MIR"
date = 2022-05-30
+++


crux-mir is a symbolic testing tool for Rust.  The user writes test cases using symbolic variables as inputs; crux-mir uses symbolic execution to check that the tests pass for all possible values of the symbolic variables.  crux-mir checks for absence of panics, overflows, and some forms of undefined behavior, and it supports user-defined assertions.  Recently, crux-mir gained support for calling Cryptol specifications directly from Rust code and for compositional reasoning, which allows efficiently verifying more complex functions, such as Rust implementations of cryptographic primitives.
In this talk, I'll describe the design of crux-mir and show some examples of its use, with particular focus on the newer Cryptol and compositional reasoning features.

[Video](https://www.youtube.com/watch?v=f3b5V3B4Q8c)