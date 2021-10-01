# Rust verification tools (2021)
This is a list of Rust verification tools with a bias towards ‘formal methods’ tools. An update of Alastair Reid's [2020 list](https://alastairreid.github.io/rust-verification-tools/).
Tool types are listed in approximate (and subjective!) increasing order of the level of expertise required and approximate increasing order of the level of assurance that they provide.
## Dynamic checking tools

* [Miri](https://github.com/rust-lang/miri/) for general UB checking (including data race detection, but only on a single execution)
Concurrency checkers
* [Loom](https://github.com/tokio-rs/loom), which focuses on exhaustive checking 
* [Shuttle](https://crates.io/crates/shuttle), which focuses on randomized checking 

## Automatic verification tools
Typically relies on a verification harness to generate symbolic input values for the code under test (although those can sometimes be generated from the function argument types). Typically checks assertions, panics, overflows, etc.

## Bounded model checking / Static Symbolic Execution

* [Rust Model Checker (RMC)](https://github.com/model-checking/rmc)
* [SMACK verifier](https://github.com/smackers/smack)
* [Crux-mir](https://crux.galois.com/  https://github.com/GaloisInc/crucible/tree/master/crux-mir)
* [Crust](https://github.com/uwplse/crust)

## Abstract interpreter ++

* [MIRAI](https://github.com/facebookexperimental/MIRAI)
## Dynamic Symbolic Execution

* [RVT](https://project-oak.github.io/rust-verification-tools/)
Rust → LLVM → {KLEE,SeaHorn} 
Plus a DSL for writing verification harnesses based on the property-based testing library proptest
* [Haybale](https://github.com/PLSysSec/haybale)
symbolic execution engine for LLVM written in Rust
* [Seer](https://github.com/dwrensha/seer)
symbolic execution engine based on Miri (not sure it is active)
* [KLEE-Rust](https://github.com/jawline/klee-rust)
KLEE bindings for Rust (inactive for 6 years)
Unbounded (?)
* [RustHorn](https://github.com/hopv/rust-horn)

## Auto-Active Verification

Midway between automatic and interactive verification. Relies on hints/annotations/etc inserted in source code such as function contracts, loop invariants, data structure invariants, etc.

* [Prusti](https://www.pm.inf.ethz.ch/research/prusti.html) [github link](https://viperproject.github.io/prusti-dev/)
* [Creusot](https://github.com/xldenis/creusot) Rust → whyml verifier

## Interactive verification
Converts Rust to code in an interactive theorem prover which is then verified with human input.
This allows one to treat more complex programs.

#### Coq
* [HacSpec](https://github.com/hacspec/hacspec) A specification language for cryptographic primitives in Rust.
Also has non-cryptographic applications: [riot bootloader](https://github.com/hacspec/hacspec/blob/master/examples/riot-bootloader/src/lib.rs), the part of the bootloader that selects which image to boot :  involves a small hash algorithm and a list traversal. [RIOT link](https://future-proof-iot.github.io/RIOT-fp/events)
* [ConCert](https://github.com/AU-COBRA/ConCert) extracts functional programs in Coq to Rust by using arenas. It originated from smart contract verification.
* [fiat cryptography](https://github.com/mit-plv/fiat-crypto) is a verified compiler for cryptographic primitives in Coq that generates Rust implementations (and other languages). [WIP](https://github.com/AU-COBRA/AUCurves/blob/main/src/Bedrock/ToRustString.v) on extending bedrock2 with a rust printer.
#### Interactive verification of the foundations of Rust
* [RustBelt](https://plv.mpi-sws.org/rustbelt/)
Semantics close to MIR, focuses on verification of unsafe code, 
#### Interactive verification of core subsets of Rust
* [Oxicide](https://github.com/aatxe/oxide), [arxiv link](https://arxiv.org/abs/1903.00982) type systems account of Rust's borrow checker, close to surface rust.
* [WASMCert](https://github.com/WasmCert/WasmCert-Coq) Formalization of the wasm standard
* [VeLLVM](https://github.com/vellvm/vellvm)  Formalization of the LLVM compilation infrastructure

#### LEAN prover

* [Electrolysis](https://github.com/Kha/electrolysis) Rust → LEAN translator (no longer active, MSc thesis)

## Standardization/Specification

* [Ferrocene](https://ferrous-systems.com/blog/sealed-rust-the-pitch/) (previously called Sealed Rust)
