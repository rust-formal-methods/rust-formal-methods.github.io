+++
date = 2023-03-27
title = "Flux: Ergonomic Verification of Rust Programs with Liquid Types"
+++

Low-level, pointer-manipulating programs are tricky to write and devilishly hard to verify, requiring complex spatial program logics to reason about heap updates. Recent systems like Prusti and Creusot take advantage of Rust ownership mechanisms to shield the programmer from some spatial assertions, allowing them to only write pure, first-order logic specifications which can be automatically verified by a solver. Even with these advances, verification remains unpleasant. For instance, when working over collections, program-logic based methods require the use of loop invariants that are universally quantified to account for the potentially unbounded contents of the collection. Such invariants often require a sophisticated understanding of the underlying spatial program logic, and worse, the quantification makes them difficult to synthesize.

This talk presents Flux, a refinement type checker for Rust that shows how logical refinements can work in tandem with Rust’s ownership mechanisms to yield ergonomic type-based verification. First, we describe how Flux extends Rust’s type system with logical refinements that can be used to specify properties about data. Next, we demonstrate how the combination of refinements and Rust’s ownership mechanisms allows the specification and verification of imperative code. Finally, by looking at some examples, we show how the combination of refinements, ownership, and Rust polymorphic constructors, enables ergonomic verification of lightweight properties.

**Recording Link**: [YouTube](https://www.youtube.com/watch?v=2PEjvhkknzw)
