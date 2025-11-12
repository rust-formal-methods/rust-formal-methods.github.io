+++
title = "Place Capability Graphs"
date = 2025-11-24T19:00:00+01:00 # (Paris/Zurich)
+++

Rust's novel type system has proved an attractive target for verification and
program analysis tools, due to the rich guarantees it provides for controlling
aliasing and mutability. However, fully understanding, extracting, and
exploiting these guarantees is subtle and challenging: existing models for
Rust's type-checking either support a smaller idealised language disconnected
from real-world Rust code, or come with severe limitations in terms of precise
modelling of Rust borrows, composite types storing them, function signatures and
loops.

In this talk, Zack will present *Place Capability Graphs*: a novel model of Rust's
type-checking results, which lifts these limitations, and is directly calculated
from the Rust compiler's own programmatic representations and analyses. The PCG
model supports almost all real-world Rust code (97% of Rust functions in the
most popular public crates), and is suitable as a general-purpose basis for
verification and program analysis tools.

**Presenter**: [Zack Grannan](https://zackg.me) is a PhD student in the [Software
Practices Lab](https://spl.cs.ubc.ca) at the University of British Columbia,
working under the supervision of Alex Summers. His research focuses on Rust
program verification, and he is also involved in the development of the
[Prusti](http://prusti.org/) program verifier.

**Meeting Link**: [Join Zoom meeting here.](https://ethz.zoom.us/j/69305900756)

**Recording Link**: TBD
