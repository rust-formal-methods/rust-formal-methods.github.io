+++
title = "MiniRust with Ralf Jung"
date = 2022-11-28
+++

As Rust grows in popularity and usage, it is becoming more and more important to clearly define its operational semantics.
Despite plenty of work on Rust verification, so far no semantics exist that can capture all the aspects of the 'real thing'.
MiniRust is a new project I started to define a normative specification of a Rust 'core language', which is versatile enough to be used as a cornerstone for a full Rust specification.
Rather than use the traditional mathematical jargon, MiniRust is written as an interpreter using Rust syntax (with a few extensions).

In this talk I will introduce MiniRust, what has been specified so far, and the road left to go.
We'll also see how to use MiniRust to explain the behavior of several intricate snippets of unsafe Rust code.