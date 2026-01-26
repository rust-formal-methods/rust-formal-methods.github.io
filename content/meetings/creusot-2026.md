+++
title = "Verifying Rust programs with Creusot"
date = 2026-01-26
+++

[Creusot](https://github.com/creusot-rs/creusot) is a deductive verifier for Rust. In this talk, I will
present Creusot's newest features and case studies. One notable addition is the support for linear ghost
resources (inspired by [Verus](https://dl.acm.org/doi/10.1145/3586037)), which enables the verification of unsafe Rust code involving raw pointers.
Applications include verified implementations of union-find and persistent arrays ([CPP 2026](https://hal.science/hal-05396946)),
as well as the verification of slice functions in the Rust standard library (ongoing work towards [the verify-rust-std challenge](https://model-checking.github.io/verify-rust-std/challenges/0017-slice.html)).

**Speaker:** [Li-yao Xia](https://poisson.chat/), research engineer at Laboratoire Méthodes Formelles.

**Zoom Link:** [https://ethz.zoom.us/j/66163706963](https://ethz.zoom.us/j/66163706963)

[**Slides**](https://docs.google.com/presentation/d/e/2PACX-1vTEJL5lYZLX-M-dF0udV0X7l_ElUEpa3yGW24VdWBka6QRvtGk-HekGQe3iFR_57s2ad--zGuAVoQxx/pub#slide=id.p)
