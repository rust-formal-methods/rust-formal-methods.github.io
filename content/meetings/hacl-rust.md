+++
date = 2024-01-22
+++


The program verification community is slowly realizing that life is much better when one verifies Rust programs instead of C or ASM programs. Yet, a large body of verified code has already been written to generate C and/or ASM – I am talking specifically about the HACL* and Vale projects, respectively. What do we do about those, then, in a world where users want pure Rust code? (The answer is NOT "hire 10 more PhD students and have them redo everything". That would not be nice.)

In this talk, I will present two projects that, together, provide a smooth transition path while offering backwards-compatibility.
HACL-rs is a new code-generation path that compiles the HACL* verified cryptographic library from F* to Rust. HACL* is written in a DSL of F*, called "Low*", which models C-like pointer arithmetic and arrays. The research question is: how do we rewire the compilation pipeline to produce safe Rust code instead? This poses an array (pun intended) of interesting challenges, such as how to deal with borrows and pointer arithmetic.
Eurydice (same family as Charon and Aeneas, which were presented here before) is a compiler from Rust to C. While this is possibly one of the least glamorous projects ever, it actually fills a very real use-case: we are now writing new verified crypto in Rust, yet a lot of folks are not ready to take a dependency on Rust in their codebases. These people include flagship customers of HACL*, like Mozilla. I'll talk about the engineering behind the project and how to reconstruct palatable C code out of MIR, relying on Charon for some of the heavy-lifting.