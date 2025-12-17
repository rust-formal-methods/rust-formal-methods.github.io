+++
title = "Soteria Rust"
date = 2025-12-15T19:00:00+01:00 # (Paris/Zurich)
+++


In this talk, we present work in progress on Soteria Rust, the first symbolic execution engine for Rust that fully supports reasoning about the language's complex aliasing model, Tree Borrows, while delivering performance competitive with Kani, the state-of-the-art bounded model checker for Rust. 

We describe the architecture of the engine, from its value language, inspired from MiniRust, to its state representation, optimised for symbolic execution (unlike a more naive byte-array approach). Soteria Rust natively supports Tree Borrows, Rust's newest aliasing model, out of the box. We show how the engine's design simplifies the implementation of Rust's evolving internals, and catches some errors at the compilation stage, rather than at runtime. Because the underlying library, Soteria, is proven sound, we can trust the engine's results and can focus on the minute details of Rust's semantics, rather than building a symbolic execution engine from the ground up. 

Finally, we compare Soteria Rust with Kani and Miri across a suite of benchmarks, showing strong performance, a more complete analysis than Kani, all while doing a symbolic analysis, unlike Miri. We conclude by outlining directions for future work, including support for compositional analysis and bi-abduction.

**Speaker:** [Opale](https://portfolio.n1ark.com) is a PhD student at imperial College London, under the supervision of Azalea Raad. She works on the [Soteria](https://github.com/soteria-tools/soteria) library with Sacha-Élie Ayoun. Her research interests include under-approximate bug finding, bi-abduction, and language semantics for Rust.

**Meeting Link**: [Zoom](https://ethz.zoom.us/j/64354800595)

**Recording Link**: [YouTube](https://www.youtube.com/watch?v=Q7sOHhbL0N8)
