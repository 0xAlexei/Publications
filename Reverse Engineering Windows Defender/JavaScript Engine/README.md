
# Reverse Engineering Windows Defender's JavaScript Engine

*As presented at REcon Brussels and Jailbreak Security Summit*

Windows Defender’s `MpEngine.dll` implements the core of Defender’s functionality in an enormous ~11 MB, 30,000+ function DLL. In this presentation, we’ll look at the ~1,200 functions that comprise Defender’s proprietary JavaScript engine, which is used for analyzing potentially malicious JS code. Defender implements a full JS engine, though it is significantly simpler than the engines found in modern web browsers, so it is a tractable target for reverse engineering from binary.

We’ll cover reverse engineering the JS engine, including how it works (types, memory management, JS/ECMAScript features, integration with Defender’s antivirus system, etc.), building tooling to interact with it, non-security JS runtime bugs, anti-analysis tricks for malicious scripts, and a bit on the engine’s attack surface for exploitation.

We’ll conclude by considering other attack surface within the remaining 98% of this enormous binary.
