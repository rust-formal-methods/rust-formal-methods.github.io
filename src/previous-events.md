## Previous Meetings

### November Meeting (November 29th, 2021)

[Bas Spitters](twitter.com/basspittersbs) [EventBrite](https://www.eventbrite.com/e/november-meeting-rust-verification-with-bas-spitters-tickets-198474531667).

**Formal Verification of Subsets of Rust**

Rust is a big and complex language. Fortunately, it contains a number of interesting sublanguages for which formal verification is more manageable.
I will give an overview of three projects that we are working on in my group.
 
[ConCert](https://github.com/AU-COBRA/ConCert) is a Coq framework for reasoning about functional programs, in particular focussing on smart contracts. 
As part of this we have developed a general backend to the Coq proof assistant which allows one to generate provably correct functional *rust* programs.
One main use case is to generate rust smart contracts which can be used on the [concordium](https://concordium.com) blockchain.

[HACSPEC](https://github.com/HACS-workshop/hacspec) is a subset of rust for the specification of high assurance cryptography. We have used it to specify the BLS elliptic curve. This sepcification can be translated to Coq from where we use [fiat-cryptography](https://github.com/mit-plv/fiat-crypto) and [BedRock](https://github.com/mit-plv/bedrock) to generate a correct by construction, efficient, platform independent implementation.

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
