# Syndicate Labs

Independent systems research. Solo builder. 1.5 years in.

I design and build novel infrastructure primitives — storage engines, attestation protocols, archival formats, and programming languages — from first principles, on a phone, in Termux.

No institutional affiliation. No degree. Just working systems.



## Active Public Projects

### 🔒 RLC — Rhizome Lattice Core
**Physics-gated storage that makes data exfiltration physically difficult.**

RLC turns passive file storage into an active, policy-governed system. Files exist in one of three viscosity states — FLOW, AUDIT, or FROZEN — determined by access behavior in real time. High-velocity extraction patterns (bulk reads, rapid sequential access) trigger progressive resistance without requiring agent installation on endpoints.

- Merkle + Lattice structure with signed policy epochs
- HMAC-authenticated daemon with HTTP interface
- Portable demo mode: runs without FUSE or admin rights
- v9.18.2 — production-ready demo bundle with full threat model, SBOM, and enterprise intake docs

> *"Normal work feels normal. High-velocity extraction becomes physically difficult."*



### ⚡ CSA — Chaotic System Attestation
**Post-quantum device identity rooted in hardware physics, not static keys.**

CSA binds device identity to how a specific piece of silicon behaves when driven through a chaotic dynamical system — not just what secrets it stores. An attacker who steals your firmware still cannot impersonate your device, because they cannot reproduce your hardware's drift profile in real time.

- Chaos-Amplified Physical Unclonable Function (CA-PUF) architecture
- Fixed-point Lorenz attractor engine (CSA-Storm) in C
- Time-bounded challenge–response protocol
- Designed for air-gapped, edge, and autonomous systems where heavyweight crypto stacks are impractical

→ [Public demo and architectural overview](https://github.com/RobertP-SyndicateLabs/chaotic-system-attestation-demo)



### 🗄️ LARC — Lattice Archival Resilience Container
**An archival format that degrades gracefully instead of dying catastrophically.**

Standard archives (ZIP, tar) fail completely when their directory is corrupted. LARC treats catastrophic failure as a design constraint to engineer around. Its distributed directory is Reed-Solomon encoded, replicated 7×, and scattered through the lattice. If the directory is destroyed, the system reconstructs it mathematically. If that fails, it falls back to blind payload extraction of surviving cells.

- Custom GF(2^8) Reed-Solomon engine with convolutional interleaving
- Adaptive entropy compression per chunk (MSHT pipeline)
- Cryptographic ROOTCELL witness for tamper detection
- Proven "Impossible Demo": recovers files from archives with 20–30% random internal byte destruction



### 🔤 SIC — Sacred Index Code *(active development)*
**A programming language and meta-unification substrate.**

SIC is a novel language designed around sovereign execution semantics — code that knows where it runs, enforces its own identity boundaries, and bridges naturally into orchestrated multi-agent environments. Early stage but architecturally intentional.



## Philosophy

These systems share a common thread: they treat the physics of computation — timing, drift, entropy, state — as a first-class design resource rather than implementation noise to be abstracted away.

Security that lives in math can be broken by better math.  
Security that lives in physics requires you to replicate physics.



## Contact

Building in public. Open to technical discussion, licensing inquiries, and pilot engagements.

📧 wespaoletti@gmail.com

🔗LinkedIn: https://www.linkedin.com/in/robert-p-145437a1?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app
