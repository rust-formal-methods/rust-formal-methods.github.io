+++
title = "Tree Borrows, a pointer aliasing model for Rust"
date = 2023-05-29
+++

The strong guarantees of unique ownership and immutability provided by reference types
in Rust should in principle allow compilers to apply more powerful optimizations that rely
on uniqueness. However `unsafe` code can easily break these assumptions by allowing
shared mutability, which makes many optimizations seemingly incompatible with the use
of `unsafe`. Since optimizations are necessary for Rust to achieve its promised performance,
and because `unsafe` is rooted in the low level manipulations of nearly every major library,
these two aspects need to be reconciled somehow.
Much like its predecessor Stacked Borrows which it improves upon, Tree Borrows defines an
alternative operational semantics of memory accesses by enforcing a pointer aliasing discipline.
Programs that violate this discipline are declared to have undefined behavior (UB) and are ruled
out from the verification of compiler optimizations. This introduces a tradeoff in which the stricter
the aliasing discipline is, the stronger optimizations can be performed, but also the more
programmers need to be careful not to accidentally write code that exhibits UB.
Common patterns that Stacked Borrows is known for rejecting too aggressively or being inconsistent
with have in part guided the design and evaluation of Tree Borrows, in order to ensure that the
balance between enabling optimizations and being able to write `unsafe` code is suited to real-life
codebases.
The rules of Tree Borrows are thus,
- consistent, with as few exceptions as possible (notably two-phase borrows and `extern`
types of unknown size do not require special handling);
- permissive enough to allow most common patterns that would break backwards compatibility
if forbidden, even at the cost of some optimizations;
- configurable in their details in case a version with stronger guarantees is desired.