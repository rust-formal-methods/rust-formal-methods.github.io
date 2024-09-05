+++
title = "CONCERT and HACSPEC"
date = 2021-11-29
+++

Rust is a big and complex language. Fortunately, it contains a number of interesting sublanguages for which formal verification is more manageable.
I will give an overview of three projects that we are working on in my group.
 
[ConCert](https://github.com/AU-COBRA/ConCert) is a Coq framework for reasoning about functional programs, in particular focussing on smart contracts. 
As part of this we have developed a general backend to the Coq proof assistant which allows one to generate provably correct functional *rust* programs.
One main use case is to generate rust smart contracts which can be used on the [concordium](https://concordium.com) blockchain.

[HACSPEC](https://github.com/HACS-workshop/hacspec) is a subset of rust for the specification of high assurance cryptography. We have used it to specify the BLS elliptic curve. This sepcification can be translated to Coq from where we use [fiat-cryptography](https://github.com/mit-plv/fiat-crypto) and [BedRock](https://github.com/mit-plv/bedrock) to generate a correct by construction, efficient, platform independent implementation.

---


[Bas Spitters](twitter.com/basspittersbs) [EventBrite](https://www.eventbrite.com/e/november-meeting-rust-verification-with-bas-spitters-tickets-198474531667).


Find the YouTube video [here](https://www.youtube.com/watch?v=OCehhVDMXKQ).
