+++
title = "Kani"
date = 2022-03-28
+++



Kani is a Rust verification tool based on model checking. With Kani, you can ensure that broad classes of problems are absent from your Rust code by writing proof harnesses, which are broadly similar to tests (especially property tests). Kani is especially useful for verifying unsafe code in Rust, where many of the language's usual guarantees can no longer be checked by the compiler. But Kani is also useful for finding panics in safe Rust, and it can check user-defined assertions.

Kani is currently in the initial development phase, and has not yet made an official release. It is under active development, but it does not yet support all Rust language features."

https://model-checking.github.io/kani/getting-started.html

Celina Val and Daniel Schwartz-Narbonne will present their work on [Kani](https://github.com/model-checking/kani), a Rust model-checker they are developing at Amazon.