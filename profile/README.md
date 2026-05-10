<div align="center">

# North9

**Building infrastructure for a post-quantum internet.**

[north9.org](https://north9.org) &nbsp;·&nbsp; [contact@north9.org](mailto:contact@north9.org)

</div>

---

We build the hard parts — cryptography, transport stacks, and systems that have to work when everything else fails.

---

## Open Source

### [Seam](https://github.com/North9LLC/Seam)

Post-quantum encrypted transport protocol in Rust. UDP, multi-stream, hybrid Noise\_XX + ML-KEM-768 handshake — baked in, not bolted on. 247 µs handshake, 568 MiB/s encrypted throughput per core, forward error correction for lossy links.

```
cargo add seam-protocol --git https://github.com/North9LLC/Seam
```

### [Seamless](https://github.com/North9LLC/Seamless)

Reverse tunnel built on Seam. Expose any local service through a relay you control — HTTP by subdomain, raw TCP by port. Client dials out, no port forwarding needed. Post-quantum by default.

```
# relay
./seamless-relay --seam-addr 0.0.0.0:4443 --http-addr 0.0.0.0:80

# client (behind NAT)
./seamless --relay relay-ip:4443 --x25519 <key> --kem <key> http 3000
```

---

<div align="center">

MIT &nbsp;·&nbsp; [north9.org](https://north9.org)

</div>
