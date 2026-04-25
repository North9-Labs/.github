<div align="center">

# North9

**A venture studio building the infrastructure for a more private, more verifiable, post-classical internet.**

[north9.org](https://north9.org)

</div>

---

## What we do

We build companies. The hard kind — products that require new cryptography, new transport stacks, new operating systems, or new ways to simulate physics. We start with a problem that the existing toolchain can't solve, build the toolchain, ship the product, and spin it out.

Our work spans four threads: **post-quantum infrastructure**, **provable media authenticity**, **frontier quantum simulation**, and **privacy-first consumer software**. AI shows up across all of them — as a tool, as a threat model, and as a target.

---

## Active projects

| Project | What it is |
|---|---|
| **[Signet](https://github.com/North9LLC/Signet)** | Cryptographic watermarking SDK that camera apps embed to certify photos are real. Stamps happen at the shutter, before encoding. Verification is a binary BLS check against the [drand](https://drand.love/) public randomness beacon — no model, no score. |
| **[qRoute](https://github.com/North9LLC/qRoute)** | Hybrid quantum circuit simulator. Auto-routes to the cheapest correct backend (light-cone, Heisenberg, stabilizer, dense). Exact expectation values on **200–1000+ qubit** circuits — on a laptop CPU. |
| **[Apex Protocol](https://github.com/North9LLC/apex)** | Post-quantum encrypted UDP transport in Rust. Noise_XX + ML-KEM768 handshake in **247 µs**, ChaCha20-Poly1305 packet protection, GF(2⁸) FEC, multi-stream priority scheduling. ~568 MiB/s per core. |
| **[NorthOS](https://github.com/North9LLC/NorthOS)** | A GrapheneOS fork built for people under real threat. Three switchable security tiers, 27 purpose-built defensive apps, IMSI-catcher detection, duress PIN, ultrasonic-beacon notch filtering, no Google endpoints anywhere. |
| **[Relay](https://github.com/North9LLC/Relay)** | End-to-end encrypted messenger for high-trust networks. Per-message X25519 key rotation, ChaCha20-Poly1305 AEAD, 20-minute relay TTL, encrypted-at-rest local store. No social graph, no logs. |
| **[North9 Search](https://github.com/North9LLC/north9-search)** | Privacy-first metasearch. Aggregates and re-ranks Brave, Mojeek, DuckDuckGo, and Wikipedia. No cookies, no tracking, no logs — upstream engines see the server, not the user. |

---

## How we work

- **Build the hard part first.** If a product needs new crypto, a new transport, or a new kernel patch series, we build that — not a wrapper around an API.
- **Open source by default.** Most of our work ships under MIT. Trust comes from auditable code, not marketing copy.
- **Cross-validated, not just tested.** Quantum backends are checked against Qiskit Aer to 1e-10. Crypto is built on `@noble/*`, `ring`, drand, and standards-track primitives — never homegrown.
- **No nonsense in READMEs.** Our docs say what something is, what it isn't, and what its limits are. The same applies to how we talk about the company.

---

## Get in touch

- Web — [north9.org](https://north9.org)
- Building at the frontier — privacy infrastructure, post-quantum systems, applied quantum, AI-native products? We'd like to talk.

<div align="center">

Built with care · North9

</div>

<!--
This file lives at `profile/README.md` in the `North9LLC/.github` repo
and renders as the public landing page at github.com/North9LLC.
-->
