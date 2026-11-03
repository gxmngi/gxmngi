<div align="center">
  <img src="./rusdan-matrix.svg" alt="Rusdan Systems Architecture" width="100%" />
</div>

# Rusdan Lamsa (`@gxmngi`)

> **Systems & Full-Stack Software Engineer**  
> Focused on Distributed Systems, Storage Engine Architecture, and Cloud Infrastructure Platforms.  
> Engineering from first principles with **Go**, **Rust**, and **TypeScript**.

[![GitHub followers](https://img.shields.io/github/followers/gxmngi?label=Followers&style=flat-square&color=24292e)](https://github.com/gxmngi)
[![Top Languages](https://img.shields.io/badge/Stack-Go%20%7C%20Rust%20%7C%20TypeScript-007acc?style=flat-square)](https://github.com/gxmngi)
[![Status](https://img.shields.io/badge/Status-Open%20to%20Opportunities-success?style=flat-square)](https://github.com/gxmngi)

---

## 🏛️ Core Architectural Pillars & Selected Systems

Below is an overview of core production-grade and systems-level projects engineered from first principles:

| System / Project | Domain & Stack | Architectural Mechanism & Highlights | Benchmarks / Invariants |
| :--- | :--- | :--- | :--- |
| [**Stratus Cloud**](https://github.com/gxmngi/stratus-cloud) | **Cloud PaaS & Orchestrator**<br>`Go` `Next.js 15` `Docker` `Redis` | • Ephemeral Docker sandboxing (`CapDrop: ALL`, `PidsLimit: 256`, 1GB RAM quota)<br>• In-memory `O(1)` Go Edge Reverse Proxy with Redis Pub/Sub routing<br>• Resilient task queue via Redis Streams (`XADD`/`XAUTOCLAIM`)<br>• Real-time log pipeline to WebSockets & embedded `xterm.js`<br>• 1-Click zero-downtime blue-green aliases & atomic rollback | Sub-millisecond proxy routing, zero leaked resources, scale-to-zero serverless auto-sleep |
| [**LithosDB**](https://github.com/gxmngi/lithos-db) | **On-Disk Database Engine**<br>`Rust` *(Zero external crates)* | • 4096-Byte Slotted-Page hardware virtual memory alignment<br>• Dynamic 50/50 B+Tree node splitting & leaf pointer elevation<br>• Write-Ahead Logging (WAL) with 64-bit FNV-1a checksum frames<br>• Automatic dirty crash recovery on boot (ACID durability)<br>• Interactive REPL with ASCII `.btree` visualizer | **151,226 QPS** Point Search (6.61 μs latency)<br>**4.27M recs/sec** linked-leaf scan<br>Synchronous WAL `fsync` |
| [**VortexTorrent**](https://github.com/gxmngi/vortex-torrent) | **P2P Network Protocol**<br>`Go` *(Standard library only)* | • BEP 0003 BitTorrent state machine & TCP wire protocol<br>• Zero-copy raw bencode byte slicing for 20-byte SHA-1 `info_hash`<br>• Pipelined 16KB block requests (`MaxBacklog = 5`) for saturated pipes<br>• End-Game Mode tail-latency cancellation for lingering pieces<br>• Concurrent multi-peer worker pool using native Goroutines & channels | Wire-speed swarm downloads, 100% cryptographic piece validation |
| [**MiniGit**](https://github.com/gxmngi/minigit-py) | **VCS Internals**<br>`Python` | • Git plumbing engine: Blobs, Trees, Commits, and Tag objects<br>• SHA-1 content-addressable storage & zlib byte-level compression<br>• Branching, checkout, and commit graph traversal | Deterministic Git object hash parity with native Git CLI |

---

## 🛠️ Technical Competencies

- **Systems & Concurrency:** Rust (Memory Safety, RAII, Systems Programming), Go (Goroutines, Channels, Low-latency I/O), C/C++
- **Full-Stack & Web Platforms:** TypeScript, Next.js 15 (App Router, Server Components), Node.js, WebSockets, Tailwind CSS
- **Data & Storage Internals:** On-disk B+Tree engines, Slotted-Page architecture, WAL, PostgreSQL, SQLite, Redis (Streams & Pub/Sub)
- **Infrastructure & Sandbox Security:** Docker Engine API, Linux cgroups/namespaces, Capability Dropping, Reverse Proxies, CI/CD GitHub Actions

---

## 📐 Engineering Philosophy

> **"Correctness by Construction & Zero-Lookahead Invariants."**  
> We make illegal states unrepresentable through strict typing, deterministic test harnesses, pure functional cores with imperative shells, and defensive hardware-aligned resource quotas.

---

<p align="center">
  <i>Maintained by Rusdan Lamsa (<a href="https://github.com/gxmngi">@gxmngi</a>)</i>
</p>
