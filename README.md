# ChimeraV1-public

### Chimera V1 is a Java obfuscator designed to be resistant to AI-assisted deobfuscation.

## The Problem

Recent advances in AI have made it possible to deobfuscate even some of the strongest commercial Java protection systems, including techniques such as virtualization and native transpilation.

Chimera aims to make this significantly more difficult by implementing protection techniques that AI models struggle to reason about statically, encouraging or requiring runtime analysis instead. While this is unlikely to make deobfuscation impossible, it can substantially increase the time and effort required.

## Design Goals

Chimera is designed as an **anti-deobfuscation** obfuscator, **not** an anti-cracking solution. It is intended to make understanding and recovering code substantially more difficult, but it does not directly attempt to prevent modification, patching, or other forms of cracking.

Additionally, Chimera does **not** include conventional obfuscation techniques such as identifier renaming, string encryption, or control-flow obfuscation. It is intended to complement a traditional Java obfuscator rather than replace one, and using both together is strongly recommended.

The primary goal of Chimera V1 is effectiveness above all else. Performance, code size, and usability are considered secondary concerns. If a protected program takes 15 seconds to print `"Hello, World!"`, but significantly increases the difficulty of AI-assisted deobfuscation, then V1 has achieved its objective.

Future versions will refine this approach:

* **Chimera V2** will focus on improving performance, architecture, and maintainability while preserving the core protection techniques.
* **Chimera V3** will aim to combine the strongest security properties of V1 with the performance and engineering improvements introduced in V2.

> **Note:** Chimera V1 is not yet publicly released. Once development is complete, it will be superseded by Chimera V2, which is intended to address the architectural limitations and shortcomings identified in V1.
