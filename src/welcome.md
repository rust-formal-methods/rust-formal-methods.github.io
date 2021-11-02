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

## November Meeting (November 29th, 2021)

[Bas Spitters](twitter.com/basspittersbs) [EventBrite](https://www.eventbrite.com/e/november-meeting-rust-verification-with-bas-spitters-tickets-198474531667).

**Formal Verification of Subsets of Rust**

Rust is a big and complex language. Fortunately, it contains a number of interesting sublanguages for which formal verification is more manageable.
I will give an overview of three projects that we are working on in my group.
 
[ConCert](https://github.com/AU-COBRA/ConCert) is a Coq framework for reasoning about functional programs, in particular focussing on smart contracts. 
As part of this we have developed a general backend to the Coq proof assistant which allows one to generate provably correct functional *rust* programs.
One main use case is to generate rust smart contracts which can be used on the [concordium](https://concordium.com) blockchain.

[HACSPEC](https://github.com/HACS-workshop/hacspec) is a subset of rust for the specification of high assurance cryptography. We have used it to specify the BLS elliptic curve. This sepcification can be translated to Coq from where we use [fiat-cryptography](https://github.com/mit-plv/fiat-crypto) and [BedRock](https://github.com/mit-plv/bedrock) to generate a correct by construction, efficient, platform independent implementation.


## December -- Cancelled

Though we love talking rust verification, its important to take breaks too. Enjoy the end of your year and we'll see you back in 2022!

## January Meeting (January 31st, 2022)

Herman Venter will present to us his work on [MIRAI](https://github.com/facebookexperimental/MIRAI), an abstract interpreter for MIR.

Details coming soon!

## February Meeting (February 28th, 2022)

We will hear an update on Ferrocene, a project to develop a specification for MIR itself, given by Sabree Blackmon and Florian Gilcher.

Details forthcoming! 

## March Meeting (March 28th, 2022)

Celina Val and Daniel Schwartz-Narbonne will present their work on [RMC](https://github.com/model-checking/rmc) (Rust Model Checker), a tool they have been developing at Amazon.

Details forthcoming!
