+++
title = "Type Invariants in Creusot"
date = 2023-09-25
+++

Type invariants are a common mechanism in program verification, that allows attaching logical predicates to data types. They typically capture properties of a data type that are preserved by operations on its values. Creusot is a tool for automated deductive verification of (safe) Rust programs. Leveraging the non-aliasing guarantees of Rust's type system, it translates annotated Rust to a functional language. The challenge of supporting type invariants in Creusot is preserving its strong composability without introducing unsoundness in the interaction with Creusot's encoding of mutable borrows. We present a novel translation of invariants for mutable borrows, that overcomes these challenges. Type invariants in Creusot proved useful for the verification of Rust's iterator combinators, reducing the required amount of manual specifications.