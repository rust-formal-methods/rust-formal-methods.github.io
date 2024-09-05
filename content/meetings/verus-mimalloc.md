+++
date = 2023-11-27
title = "Verifying a Concurrent Memory Allocator with Verus"
+++

2023-11-27

mimalloc verus

I will present ongoing work in verifying a concurrent memory allocator using Verus [1], a deductive verification tool for Rust. One of the challenges with a memory allocator is that it has to coarsely acquire memory from the OS, which it then must divide between the its own internal data structures and the memory to be allocated to the user. Verifying this code therefore requires detailed reasoning about memory permissions, which Verus supports with ownership ghost types [2].
In this talk, I'll give an overview of the memory allocator's design, which is based roughly on the design of mimalloc [3]. I'll explain what ownership ghost types are, how Verus uses them, and how they help us reason about the memory permissions in the allocator proof. I'll also show how ownership ghost types help us provide succinct specifications for the allocator's malloc and free functions.
[1] https://github.com/verus-lang/verus
[2] Verus: Verifying Rust Programs using Linear Ghost Types. Andrea Lattuada, Travis Hance, Chanhee Cho, Matthias Brun, Isitha Subasinghe, Yi Zhou, Jon Howell, Bryan Parno, Chris Hawblitzel. (OOPSLA 2023)
[3] Mimalloc: Free List Sharding in Action. Daan Leijen, Ben Zorn, Leonardo de Moura.