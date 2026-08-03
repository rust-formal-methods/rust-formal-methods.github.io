+++
title = "KMIR: Semantics of Public MIR in K"
date = 2026-08-10T19:00:00+02:00
+++
This talk covers KMIR and the K Framework. KMIR is an executable formal semantics of Rust's Stable (Public) MIR, written in the K Framework. K is a language for defining programming-language semantics, from which its toolchain automatically derives an interpreter that runs the same rules either concretely or symbolically. Therefore, KMIR can be used to verify properties in Rust programs concretely or symbolically at the MIR level.

We present an orientation to the K Framework and Matching Logic (the mathematical foundation of its symbolic execution), together with the current encoding of MIR in K, its capabilities to date, and next steps for the project.

**Presenter**:

Daniel Cumming works as a verification engineer for Runtime Verification Inc., mostly either auditing Rust code or working on KMIR which is an encoding of Rust's MIR in RV's operational semantics framework K.

**Meeting Link**: [https://ethz.zoom.us/j/67132185438](https://ethz.zoom.us/j/67132185438)

**Recording Link**: TBD
