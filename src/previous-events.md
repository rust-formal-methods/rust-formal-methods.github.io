## Previous Meetings

### June Meeting (June 27th, 2022)

#### Abstract
Statically analyzing information flow, or how data influences other data within a program, is a challenging task in languages with mutation and pointers. Prior work addressed these challenges with bespoke type systems to encode information flow, such as in JFlow (for Java) and FlowCaml (for OCaml). We demonstrate that Rust's existing system of ownership types can repurposed for modular information flow analysis. We describe our analysis using Oxide, a formal model of safe Rust, and prove its soundness as noninterference. We implement the analysis as Flowistry, a tool that analyzes information flow within Rust's MIR CFG. And we show that Flowistry is reasonably precise versus a whole-program analysis via an evaluation on a dataset of large Rust codebases.

#### About the Speaker
Will Crichton is a 6th year CS Ph.D. student at Stanford University advised by Profs. Pat Hanrahan and Maneesh Agrawala. His research combines programming language theory and cognitive psychology to build better tools for programmers. Will just defended his thesis, "Revisiting Program Slicing with Ownership-based Information Flow", and will soon be starting a postdoc with Shriram Krishnamurthi at Brown to study the learnability of Rust.

Video: Coming Soon!

### May Meeting (May 30th, 2022)

#### Abstract
crux-mir is a symbolic testing tool for Rust.  The user writes test cases using symbolic variables as inputs; crux-mir uses symbolic execution to check that the tests pass for all possible values of the symbolic variables.  crux-mir checks for absence of panics, overflows, and some forms of undefined behavior, and it supports user-defined assertions.  Recently, crux-mir gained support for calling Cryptol specifications directly from Rust code and for compositional reasoning, which allows efficiently verifying more complex functions, such as Rust implementations of cryptographic primitives.
In this talk, I'll describe the design of crux-mir and show some examples of its use, with particular focus on the newer Cryptol and compositional reasoning features.

[Video](https://www.youtube.com/watch?v=f3b5V3B4Q8c)

### April Meeting (April 25th, 2022)

#### Abstract

Ferrocene is an effort to bring Rust into the realm of safety-critical software while also bringing tangible benefits to so called mission-critical efforts. The project has been ongoing for about a year now. This talk will give an overview of current findings and particularly an observation of the current state of the safety-critical ecosystem.

Particularly, it will share observations on the application of formal methods in the realm right now.

#### Speaker

Florian Gilcher is a co-founder of Ferrous Systems and a Rust teacher since 2015. Previously a member of the Rust Community and Core team and a co-founder of the Rust Foundation, Florian is currently focusing to bringing Rust to safety critical systems, such as cars.

[Video](https://www.youtube.com/watch?v=eaObPhTnoGo)

### March Meeting (March 28th, 2022)

Celina Val and Daniel Schwartz-Narbonne will present their work on [Kani](https://github.com/model-checking/kani), a Rust model-checker they are developing at Amazon.

Kani is a Rust verification tool based on model checking. With Kani, you can ensure that broad classes of problems are absent from your Rust code by writing proof harnesses, which are broadly similar to tests (especially property tests). Kani is especially useful for verifying unsafe code in Rust, where many of the language's usual guarantees can no longer be checked by the compiler. But Kani is also useful for finding panics in safe Rust, and it can check user-defined assertions.

Kani is currently in the initial development phase, and has not yet made an official release. It is under active development, but it does not yet support all Rust language features."

https://model-checking.github.io/kani/getting-started.html

### February Meeting (February 28th, 2022)

Xavier Denis will discuss [Creusot](https://github.com/xldenis/creusot), his deductive verifier for Rust. Creusot aims to provide efficient verification of complex *safe* Rust code, and is backed by the Why3 verification platform. In this talk we'll briefly cover the high-level architecture of Creusot and some of the unique features in the tool.

https://www.eventbrite.com/e/creusot-tickets-260072873967

### January Meeting (January 31st, 2022)

Herman Venter gave a retrospective view of his work on [MIRAI](https://github.com/facebookexperimental/mirai), an abstract interpreter for MIR code. We went over key design choices for abstract interpreters and the tradeoffs they imply. 

Find the YouTube video [here](https://www.youtube.com/watch?v=Slf1QWaRe2c).

### November Meeting (November 29th, 2021)

[Bas Spitters](twitter.com/basspittersbs) [EventBrite](https://www.eventbrite.com/e/november-meeting-rust-verification-with-bas-spitters-tickets-198474531667).

**Formal Verification of Subsets of Rust**

Rust is a big and complex language. Fortunately, it contains a number of interesting sublanguages for which formal verification is more manageable.
I will give an overview of three projects that we are working on in my group.
 
[ConCert](https://github.com/AU-COBRA/ConCert) is a Coq framework for reasoning about functional programs, in particular focussing on smart contracts. 
As part of this we have developed a general backend to the Coq proof assistant which allows one to generate provably correct functional *rust* programs.
One main use case is to generate rust smart contracts which can be used on the [concordium](https://concordium.com) blockchain.

[HACSPEC](https://github.com/HACS-workshop/hacspec) is a subset of rust for the specification of high assurance cryptography. We have used it to specify the BLS elliptic curve. This sepcification can be translated to Coq from where we use [fiat-cryptography](https://github.com/mit-plv/fiat-crypto) and [BedRock](https://github.com/mit-plv/bedrock) to generate a correct by construction, efficient, platform independent implementation.

Find the YouTube video [here](https://www.youtube.com/watch?v=OCehhVDMXKQ).


### October Meeting (October 25th, 2021)

Unfortunately this meeting was not record (my bad).

We discussed the specifications for a few simple functions in [Prusti](https://github.com/viperproject/prusti-dev) and [Creusot](github.com/xldenis/creusot). 
There were quite a few things to say on how we handle borrows and the differences between the two tools.

A summary will be posted soon. 

The slides are [here](./previous-events/october.pdf)

### Inaugural Meeting (September 20th, 2021)

During this meeting, we will introduced the RFMIG, and had a presentation from Vytautas Astraukas of Prusti, showing a little glimpse of verification for Rust software.

[Youtube recording](https://www.youtube.com/watch?v=ACqgutP0jXs)

## Previous events

* [RustVerify2021](https://sites.google.com/view/rustverify2021)
* [RustVerify2020](https://sites.google.com/view/rustverify2020)
