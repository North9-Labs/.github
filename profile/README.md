<div align="center">

# North9

**Building infrastructure for a post-quantum internet.**

[north9.org](https://north9.org) &nbsp;·&nbsp; [contact@north9.org](mailto:contact@north9.org)

</div>

---

We build the hard parts — cryptography, transport stacks, and systems that have to work when everything else fails. Everything ships under MIT.

---

## Open Source

### [Seam](https://github.com/North9LLC/Seam) &nbsp;·&nbsp; Post-quantum transport protocol

A user-space UDP transport stack built in Rust. Hybrid Noise\_XX + ML-KEM-768 handshake baked in from the start — not added on top. Multi-stream multiplexing with priority scheduling, forward error correction, token-bucket pacing, and DDoS-resistant stateless cookie handshakes. 247 µs full handshake. 568 MiB/s encrypted throughput per core.

### [Seamless](https://github.com/North9LLC/Seamless) &nbsp;·&nbsp; Post-quantum reverse tunnels

Expose any local service through a relay you control — HTTP by subdomain, raw TCP by port. Built on Seam, so every byte between client and relay is post-quantum encrypted end-to-end. Client dials out through NAT with no port forwarding or firewall rules.

### [Signet](https://github.com/North9LLC/Signet) &nbsp;·&nbsp; Cryptographic photo watermarking SDK

Camera apps embed an unforgeable cryptographic proof at the moment the shutter fires, derived from the [drand](https://drand.love/) public randomness beacon. Verification is binary, non-interactive, and decentralized — the Ed25519 signature and beacon data either check out or they don't. Supports iOS, Android, and C/C++ via FFI.

### [Fob](https://github.com/North9LLC/Fob) &nbsp;·&nbsp; Encrypted vault on any USB drive

Turns a commodity USB stick into a cryptographic security key. Passwords, TOTP codes, SSH keys, and secure notes — all encrypted with Argon2id and XChaCha20-Poly1305, living entirely on the drive. Plausible deniability built in. Nothing installed on your computer.

---

<div align="center">

MIT &nbsp;·&nbsp; [north9.org](https://north9.org)

</div>
