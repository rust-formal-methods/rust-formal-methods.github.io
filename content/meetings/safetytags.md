+++
title = "Taming Unsafe Code with Safety Tags"
date = 2025-10-27T19:00:00+01:00 # (Paris/Zurich)
+++


This talk introduces a tag-based approach for modeling and reasoning about the propagation of unsafe code in Rust crates. By representing the safety requirements of each unsafe function as safety tags, the approach tracks how these tags flow and transform across function calls and data structures, enabling the formulation of formal constraints to verify the soundness of both safe and unsafe functions.

This talk will also showcase two ongoing projects: tag-std and RAPx. tag-std provides a tag-based domain-specific language and tooling to document unsafe APIs, ensuring every unsafe function is annotated and checked at each call site via a linter. These tags can also be compiled into formal contracts for downstream verification. RAPx is a static analysis tool based on abstract interpretation, which we use to verify the soundness of the Rust standard library.

**Speaker:** [Hui Xu](https://hxuhack.github.io/) is an Associate Professor at the College of Computer Science and Artificial Intelligence, Fudan University. His research focuses on program analysis and software reliability, with an emphasis on Rust code analysis.

**Meeting Link**: [Zoom Link](https://ethz.zoom.us/j/67398986159)

**Recording Link**: [YouTube](https://youtu.be/g6o-TtvCFv8)
