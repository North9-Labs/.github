<div align="center">

# North9 Labs

**AI agent runtimes, post-quantum transports, and cryptographic systems.**

[north9.org](https://north9.org) &nbsp;·&nbsp; [contact@north9.org](mailto:contact@north9.org) &nbsp;·&nbsp; [install.north9.org](https://install.north9.org)

</div>

---

## AI Agents

### [north9](https://github.com/North9-Labs/north9) &nbsp;·&nbsp; Sandboxed runtime + persistent memory

Every command runs inside an isolated Docker container. Structured memory survives every `/compact` and session restart — the agent knows exactly where it left off: files touched, approaches that failed, exact commands to run next. One install wires it into Claude Code.

```sh
curl -fsSL https://install.north9.org/north9.sh | sh
```

Installs 17 MCP tools. For the full 12-server suite (budget, gate, lens, index, vault, grid, scout, forge, sift, chain, autopsy, prism):

```sh
curl -fsSL https://install.north9.org/north9.sh | sh && python3 -m north9 --suite
```

### [Prism](https://github.com/North9-Labs/Prism) &nbsp;·&nbsp; Time-travel debugger for AI agents

Record every LLM call and tool execution into a compact session file. Replay it offline, fork at any frame with a different input, and diff what changed. Git bisect for AI agents.

---

## Post-Quantum Networking

### [Seam](https://github.com/North9-Labs/Seam) &nbsp;·&nbsp; Post-quantum UDP transport

Hybrid Noise_XX + ML-KEM-768 handshake. Multi-stream mux, Reed-Solomon FEC, DDoS-resistant stateless cookies. **247 µs handshake. 568 MiB/s encrypted throughput per core.** Replaces `scp`, `netcat`, and `ssh -L`.

```sh
curl -fsSL https://install.north9.org/seam.sh | sh
```

### [Seamless](https://github.com/North9-Labs/Seamless) &nbsp;·&nbsp; Post-quantum reverse tunnels

Expose any local service through a relay you control — HTTP by subdomain, raw TCP by port. Client dials out through NAT, no port forwarding required. Built on Seam — every byte is post-quantum encrypted end-to-end.

```sh
curl -fsSL https://install.north9.org/seamless.sh | sh
```

---

## Cryptographic Systems

### [Signet](https://github.com/North9-Labs/Signet) &nbsp;·&nbsp; Cryptographic photo watermarking SDK

Camera apps embed an unforgeable drand beacon proof at shutter press — before encoding. Verification is binary, non-interactive, and decentralized. iOS, Android, and C/C++ via FFI.

### [Fob](https://github.com/North9-Labs/Fob) &nbsp;·&nbsp; Encrypted vault on any USB drive

Passwords, TOTP, SSH keys, and secure notes. Argon2id + XChaCha20-Poly1305. Plausible deniability. No install required on the host machine.

```sh
curl -fsSL https://install.north9.org/fob.sh | sh
```

---

<div align="center">

MIT / AGPL-3.0 &nbsp;·&nbsp; [north9.org](https://north9.org)

</div>
