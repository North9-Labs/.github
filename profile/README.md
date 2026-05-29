<div align="center">

# North9 Labs

**Tools for serious AI agents and secure infrastructure.**

[north9.org](https://north9.org) &nbsp;·&nbsp; [contact@north9.org](mailto:contact@north9.org)

</div>

---

We build the parts that don't exist yet — AI agent runtimes, post-quantum transports, and cryptographic systems that have to work when everything else fails. Everything ships under MIT.

---

## AI Agents

### [north9](https://github.com/North9-Labs/north9) &nbsp;·&nbsp; Sandbox + memory for autonomous agents

The missing runtime for long-running AI agents. Every command runs inside an isolated Docker container — the agent can `rm -rf`, install malware, loop forever, and your machine is fine. Structured memory survives every `/compact` and session restart, so the agent knows exactly where it left off: which files it touched, which approaches failed, what commands to run next.

One install wires it into Claude Code with automatic state saving before every compaction.

```sh
curl -fsSL https://install.north9.org/north9.sh | sh
```

### [Prism](https://github.com/North9-Labs/Prism) &nbsp;·&nbsp; Time-travel debugger for AI agents

Record every LLM call and tool execution into a compact session file. Replay it offline, fork it at any frame with a different input, and diff what changed. Git bisect for AI agents — isolate exactly which message, tool result, or model parameter caused bad output without re-running the entire expensive session from scratch.

---

## Secure Infrastructure

### [Seam](https://github.com/North9-Labs/Seam) &nbsp;·&nbsp; Post-quantum transport protocol

User-space UDP transport built in Rust. Hybrid Noise_XX + ML-KEM-768 handshake — post-quantum encryption baked in from the start, not bolted on top. Multi-stream multiplexing, forward error correction, token-bucket pacing, DDoS-resistant stateless cookies. 247 µs full handshake. 568 MiB/s encrypted throughput per core.

### [Seamless](https://github.com/North9-Labs/Seamless) &nbsp;·&nbsp; Post-quantum reverse tunnels

Expose any local service through a relay you control — HTTP by subdomain, raw TCP by port. Built on Seam, so every byte is post-quantum encrypted end-to-end. Client dials out through NAT with no port forwarding or firewall rules.

### [Signet](https://github.com/North9-Labs/Signet) &nbsp;·&nbsp; Cryptographic photo watermarking SDK

Camera apps embed an unforgeable proof at the moment the shutter fires, derived from the [drand](https://drand.love/) public randomness beacon (Cloudflare, EPFL, Protocol Labs). Verification is binary, non-interactive, and decentralized — the math either checks out or it doesn't. iOS, Android, and C/C++ via FFI.

---

<div align="center">

MIT &nbsp;·&nbsp; [north9.org](https://north9.org)

</div>
