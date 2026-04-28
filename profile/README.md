<div align="center">

# North9

**A venture studio building the infrastructure for a more private, more verifiable, post-classical internet.**

[north9.org](https://north9.org) · [Become a member](https://north9.org/become-member)

</div>

---

## What we do

We build companies. The hard kind — products that require new cryptography, new transport stacks, new operating systems, or new ways to simulate physics. We start with a problem that the existing toolchain can't solve, build the toolchain, ship the product, and spin it out.

Our work spans four threads: **post-quantum infrastructure**, **provable media authenticity**, **frontier quantum simulation**, and **privacy-first consumer software**. AI shows up across all of them — as a tool, as a threat model, and as a target.

---

## Active projects

### 🔐 Post-Quantum Infrastructure

Build cryptography and transport for the quantum-era Internet.

| Project | Status | Stack | What it does |
|---|---|---|---|
| **[Apex Protocol](https://github.com/North9LLC/Apex)** | ✅ Production | Rust, UDP, ML-KEM768 | High-performance post-quantum encrypted transport. 247 µs handshake, 568 MiB/s throughput, multi-stream priority scheduling, built-in FEC for lossy networks. |
| **[Ape](https://github.com/North9LLC/Ape)** | ✅ Production | Rust, UDP, ML-KEM768 | Post-quantum encrypted reverse tunnels. Connect any device to the public Internet through hybrid X25519 + ML-KEM-768 handshake with adaptive congestion control. |

### 📸 Media Authenticity & Verification

Cryptographic proof that digital media is real.

| Project | Status | Stack | What it does |
|---|---|---|---|
| **[Signet](https://github.com/North9LLC/Signet)** | ✅ Released | iOS/Kotlin + C/C++ | Photo watermarking SDK. Camera apps embed unforgeable proof from the drand public randomness beacon at capture time. Verification is binary, public, non-interactive. |

### 🌐 Privacy-First Software

Consumer products with zero tracking, zero logs, zero central authority.

| Project | Status | Stack | What it does |
|---|---|---|---|
| **[Relay](https://github.com/North9LLC/Relay)** | ✅ Production | Next.js, TypeScript, X25519+ML-KEM768 | End-to-end encrypted messenger for high-trust networks. Per-message ephemeral keys, 20-minute message TTL, encrypted local-only persistence. No social graph, no cloud history. |
| **[North9 Search](https://github.com/North9LLC/Search)** | ✅ Production | Next.js 16, React 19 | Privacy-first metasearch with zero tracking, cookies, or logs. Aggregates Brave, Mojeek, DuckDuckGo, Wikipedia with instant answers (calculator, unit conversion, IP lookup, hashing). |
| **[NorthUSB](https://github.com/North9LLC/NorthUSB)** | ✅ Production | Browser + Rust CLI | Encrypted vault on any USB drive. Passwords, TOTP, SSH keys, secure notes — all client-side with AES-256-GCM, no network, no server. Single-command install. |
| **[North9 Black](https://github.com/North9LLC/North9Black)** | ✅ Production | Next.js 14, TypeScript | Premium security membership site. Post-quantum communications infrastructure, member provisioning, threat intelligence dashboard for founders and operators under real threat. |
| **[NorthOS](https://github.com/North9LLC/NorthOS)** | 🚀 Alpha | Android 16, Kotlin | GrapheneOS fork for high-threat environments. Three security tiers (no factory reset needed), 27+ defensive apps, IMSI-catcher detection, duress PIN, zero Google endpoints. Pre-alpha (v0.1). |

### 🧮 Frontier Quantum

Quantum simulation and quantum-native applications.

| Project | Status | Stack | What it does |
|---|---|---|---|
| **[qRoute](https://github.com/North9LLC/qRoute)** | ✅ v0.1.0 | Python 3.11+, NumPy | Hybrid quantum circuit simulator. Exact expectation values on 200–1000+ qubit circuits without approximation, GPU, or exponential memory. Auto-routes to optimal backend (light-cone, Heisenberg, stabilizer). On PyPI. |

### 🤖 AI Infrastructure

AI agents and intelligence platforms.

| Project | Status | Stack | What it does |
|---|---|---|---|
| **[Agent](https://github.com/North9LLC/Agent)** (Loop) | 🚀 Phase 2 | Next.js 15, Fastify, Redis | Self-hosted, token-efficient AI agent with chat UI, streaming responses, and shell tool execution. WebSocket streaming, tool visualization, Redis-backed session history. Phase 1 complete; Phase 2 adds Docker sandboxing. |
| **[Lantern](https://github.com/North9LLC/lantern)** | ✅ Production | Next.js 15, PostgreSQL, Claude API | Ad intelligence platform. Monthly reports analyzing competitor ads with four ready-to-launch creative recommendations for invite-only brands. Runs ports 7770 (app) + 7771 (WebSocket). |

---

## How we work

- **Build the hard part first.** If a product needs new crypto, a new transport, or a new kernel patch series, we build that — not a wrapper around an API.
- **Open source by default.** Most of our work ships under MIT. Trust comes from auditable code, not marketing copy.
- **Cross-validated, not just tested.** Quantum backends are checked against Qiskit Aer to 1e-10. Crypto is built on `@noble/*`, `ring`, drand, and standards-track primitives — never homegrown.
- **No nonsense in READMEs.** Our docs say what something is, what it isn't, and what its limits are. The same applies to how we talk about the company.

---

## Stack overview

| Thread | Primary Languages |
|---|---|
| **Post-quantum infrastructure** | Rust (Apex, Ape), Kotlin + C/C++ (Signet) |
| **Privacy-first consumer** | Next.js + TypeScript (Relay, Search, NorthUSB web, North9Black), Kotlin + Android (NorthOS) |
| **Quantum simulation** | Python 3.11+ (qRoute) |
| **AI infrastructure** | Next.js + TypeScript + Fastify (Agent, Lantern) |

---

## Contributing

All repositories are open source under MIT license. Issues and PRs welcome across all projects.

**Before contributing:**
1. Check the project's README for contribution guidelines
2. Review existing issues to avoid duplicate work
3. For crypto/security code, audit-first approach — discuss large changes in issues first

---

## Get in touch

- **Web** — [north9.org](https://north9.org)
- **Building at the frontier?** Privacy infrastructure, post-quantum systems, applied quantum, or AI-native products? [Let's talk.](https://north9.org/contact)

---

<div align="center">

Built with care · North9 LLC

**All projects are MIT licensed. Code audits and security reports welcome.**

</div>

<!--
This file lives at `profile/README.md` in the `North9LLC/.github` repo
and renders as the public landing page at github.com/North9LLC.
-->
