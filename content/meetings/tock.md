+++
title = "Tock"
date = 2025-02-24T19:00:00+01:00 # (Paris/Zurich)
+++

Tock is a modern operating system designed to safely run multiple distrustful applications on millions of embedded devices. While Tock is written in Rust, a type and memory safe language, low-level hardware abstractions remain fundamentally unsafe. Relying solely on language and hardware safety features is not enough to prevent bugs that compromise one of Tock's core guarantees: process isolation. In particular, isolation has been violated by bugs in interrupt handling, context switching, and hardware configuration code.

To address these challenges, we are building VTock, a formally verified fork of Tock that uses Flux, an automatic Rust verifier, to prove the correctness of security-critical properties.

In this talk, I will give an overview of our verification efforts along with some of the challenges we have faced verifying production Rust code.

**Presenter**: Vivien Rindisbacher

Hi! I'm a PhD Student in the Programming Systems Group at the University of California San Diego (UCSD).
My research focuses on lightweight verification of Rust code using tools like Flux.
Before joining UCSD, I worked as a Software Engineer at Dimensional Fund Advisors and completed my undergraduate 
degree at Boston University. Feel free to check out my website for more details: https://www.vivienrindisbacher.com/

**Meeting Link**: [Zoom Link](https://ethz.zoom.us/j/67876362770)

**Recording Link**: TBD
