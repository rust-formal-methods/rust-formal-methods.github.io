+++
title = "CreuSAT"
date = 2022-09-26
+++

This talk describes CreuSAT, a formally verified SAT solver written in Rust. In addition to implementing the core conflict-driven clause learning (CDCL) algorithm, CreuSAT also implements a series of crucial optimizations.
The most important of these is the two watched literals scheme with blocking literals and circular search, the variable move-to-front (VMTF) decision heuristic, clause deletion, phase saving, and moving average based restarts.

The resulting solver is the first deductively verified solver which is able to consistently solve problems from the SAT competition.
This is done while maintaining a relatively small code base, amounting to around 4 thousand lines of proof code and program code combined, with a low proof overhead of around three lines of proof code per line of program code.

[Video]( https://youtu.be/MkhjDpai8fM )