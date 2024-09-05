+++
title = "Aeneas"
date = 2022-10-24
+++

We present Aeneas, a new verification toolchain for Rust programs based on a lightweight functional translation. We leverage Rust's rich region-based type system to eliminate memory reasoning for a large class of Rust programs by translating them to a pure lambda-calculus, as long as they do not rely on interior mutability or unsafe code. Doing so, we relieve the proof engineer of the burden of memory-based reasoning, allowing them to instead focus on *functional* properties of their code.

[Video]( https://youtu.be/9j9EE36lJJI )