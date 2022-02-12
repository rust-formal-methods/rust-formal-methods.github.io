# Rust Formal Methods Interest Group

[WG repo](https://github.com/rust-formal-methods/wg) | [Zulip Channel](https://rust-lang.zulipchat.com/#narrow/stream/183875-wg-formal-methods)

The RFMIG provides a forum for academics, industry users and any other interested party discuss and collaborate on the challenges of Rust program verification.

Our objectives are to:

*Improve communication between formal tool developers and the Rust core teams*
- Hold 'office hours' with Rust team members to answer questions about the `rustc` API or the direction of the language.
- Identify weak points in Rust's current tool interfaces, help shepherd the improvements the formal methods community needs.

*Foster a community of formal methods tools and users*
- Provide a platform for tool developers to share their work and encourage collaboration.
- Gather feedback and input from industrial and hobbyist users of formal method tooling.
- Work towards improving tool inter-compatibility, in particular of specifications.

# Upcoming Meetings

We hold our meetings on the last monday of every month. Currently, we base ourselve off of European time, with meetings at 7PM. If this causes an issue for you, please leave a message on zulip.

## February Meeting (February 28th, 2022)

Xavier Denis will discuss [Creusot](https://github.com/xldenis/creusot), his deductive verifier for Rust. Creusot aims to provide efficient verification of complex *safe* Rust code, and is backed by the Why3 verification platform. In this talk we'll briefly cover the high-level architecture of Creusot and some of the unique features in the tool.

https://www.eventbrite.com/e/creusot-tickets-260072873967

## March Meeting (March 28th, 2022)

Celina Val and Daniel Schwartz-Narbonne will present their work on [Kani](https://github.com/model-checking/kani), a Rust model-checker they are developing at Amazon.

Kani is a Rust verification tool based on model checking. With Kani, you can ensure that broad classes of problems are absent from your Rust code by writing proof harnesses, which are broadly similar to tests (especially property tests). Kani is especially useful for verifying unsafe code in Rust, where many of the language's usual guarantees can no longer be checked by the compiler. But Kani is also useful for finding panics in safe Rust, and it can check user-defined assertions.

Kani is currently in the initial development phase, and has not yet made an official release. It is under active development, but it does not yet support all Rust language features."

https://model-checking.github.io/rmc/getting-started.html

## April Meeting (February 28th, 2022)

We will hear an update on Ferrocene, a project to develop a specification for MIR itself, given by Sabree Blackmon and Florian Gilcher.

Details forthcoming! 

## 2nd Rust Verification Workshop [RustVerify](https://sites.google.com/view/rustverify2022/home)
Co-located with ETAPS 2022, Munich, Sunday, April 03, 2022

Deadline for talk/demo proposals: January 14, 2022 (Friday)


