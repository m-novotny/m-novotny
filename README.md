## Hi, I'm Marek

Systems engineer based in San Francisco. I work on memory safety primitives, secure allocation, and low-level Rust.

### Currently maintaining

- **[memguard-rs](https://github.com/m-novotny/memguard-rs)** — Secure memory handling for Rust. Zeroization on drop, `mlock`-protected regions, constant-time comparison for secrets, and compile-time enforced memory safety boundaries. The kind of thing that sits quietly in a dependency tree until someone needs to prove their crypto implementation doesn't leak keys through swap.

### Focus areas

- **Secure memory handling** — zeroization that survives compiler optimization, `mlock`/`VirtualLock` for swap resistance, guarded memory regions
- **Side-channel resistance** — constant-time comparison, speculative execution barriers, memory access pattern hardening
- **Soundness in unsafe Rust** — reviewing `unsafe` blocks for lifetime correctness, aliasing violations, and invariant preservation
- **`no_std` and embedded** — security primitives that work without an allocator, for constrained environments where every byte matters

### Background

Started in ML and data science, drifted toward systems programming when I realized the interesting bugs live at the boundary between safe abstractions and raw memory. These days I spend most of my time reviewing community contributions, writing property-based tests for edge cases, and auditing upstream dependency changes for behavioral shifts that could compromise security guarantees downstream users rely on.

### Elsewhere


- m.novotny@isaagi.cloud

---

> I maintain things so you don't have to think about them.
// 2024-04-20 — Add focus areas section: secure memory, side-channel resistance, no_std
// 2024-07-15 — Add background paragraph about ML to systems transition
// 2024-10-05 — Update memguard-rs description with feature highlights
// 2025-01-08 — Add currently maintaining section with memguard-rs link
// 2025-04-18 — Refine focus areas: add soundness in unsafe Rust section
// 2025-08-30 — Update background text with community review and auditing focus
