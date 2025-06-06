+++
title = "RefinedRust"
date = 2025-04-28T19:00:00+02:00 # (Paris/Zurich)
+++

RefinedRust is a verification tool for Rust with the goal of establishing foundational semi-automated functional correctness verification of both safe and unsafe Rust code.
It is based on a refinement type system proven sound in the Rocq prover against a RustBelt-based model.
RefinedRust translates Rust code (with user annotations) into a formal model of Rust's execution embedded in Rocq, and then checks its adherence to the RefinedRust type system using separation logic automation in Rocq.
All proofs generated by RefinedRust are checked by the Rocq proof assistant (i.e., foundational), and consequently the automation and type system do not have to be trusted.

In ongoing work, we use RefinedRust to verify core components of the ACE security monitor of IBM Research which provides a  trusted execution environment (TEE).
Low-level systems code like the ACE security monitor (which includes unsafe code in its core) are particularly interesting targets for foundational verification with RefinedRust: The properties we aim to verify are rich and security-critical, and the program code relies on low-level details of the Rust semantics and hardware.
As part of this work, we are equipping RefinedRust to model and handle larger parts of the Rust language, like traits and closures.

**Speaker:** [Lennard Gäher](https://people.mpi-sws.org/~gaeher/) is a PhD student at MPI-SWS and Saarland University in Germany since 2021, under the supervision of Derek Dreyer. His research focuses on separation logic verification, in particular for verifying properties about programs written in the Rust programming language.

**Meeting Link**: [Zoom Link](https://ethz.zoom.us/j/64556412079)

**Recording Link**: [YouTube](https://www.youtube.com/watch?v=XR8p9R1cPC4)
