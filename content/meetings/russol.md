+++
title = "Leveraging Rust Types for Program Synthesis"
date = 2023-01-30
+++
This talk will explore how one can apply ideas from verification to synthesize Rust function bodies given a signature and possibly some functional annotation, which has been implemented in a tool called RusSOL. Due to Rust's strong type system, RusSOL can get away with significantly simpler specifications (counting the function signature + annotation) while also reducing the search space to improve performance when compared to similar tools for imperative languages. The key ingredient of RusSOL's synthesis procedure is Synthetic Ownership Logic, a new program logic for deriving programs that are guaranteed to satisfy both a user-provided functional specification and, importantly, Rust's intricate type system.