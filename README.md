<div align="center">

# Mohit Singh

### Systems & Backend Engineer · Open-Source Contributor (Kubernetes, gRPC, Redis, Rust Ecosystem)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-mohitdebian-0A66C2?logo=linkedin&logoColor=white&style=flat-square)](https://linkedin.com/in/mohitdebian)
[![GitHub](https://img.shields.io/badge/GitHub-mohitdebian-181717?logo=github&logoColor=white&style=flat-square)](https://github.com/mohitdebian)
[![Portfolio](https://img.shields.io/badge/Portfolio-mohitbuilds.in-F25C2A?logo=googlechrome&logoColor=white&style=flat-square)](https://mohitbuilds.in)
[![Peerlist](https://img.shields.io/badge/Peerlist-mohitdevlabs-00AA45?logo=peerlist&logoColor=white&style=flat-square)](https://peerlist.io/mohitdevlabs)
[![Email](https://img.shields.io/badge/Email-mohitdebian@gmail.com-D14836?logo=gmail&logoColor=white&style=flat-square)](mailto:mohitdebian@gmail.com)

</div>

---

### 💡 About Me

I specialize in **low-level systems debugging, distributed infrastructure, and developer platforms**. My work focuses on fixing edge-case crashes, memory safety vulnerabilities, and concurrency race conditions in large-scale production codebases—as well as engineering high-throughput developer tools, API gateways, and AI agent runtime firewalls.

- 🛠️ **Languages:** Rust, C++, Go, TypeScript, Python, C
- 🌐 **Systems & Core:** Concurrency & Asynchronous Runtimes, Linux Internals, IPC/PTY, Distributed Systems, Network Gateways
- 🔍 **Track Record:** **77 Pull Requests** across **16 top-tier open-source organizations** (Kubernetes, gRPC, Redis, Grafana, OpenHands, Prefix.dev, Conda).

---

## 🏆 Open Source Track Record

I contribute directly to tier-1 open source repositories, identifying root causes, authoring regression tests, and working closely with upstream maintainers to land production fixes.

```txt
┌─────────────────────────────────────────────────────────────────────────────────┐
│  77 PRs Authored  │  12+ Production PRs Merged  │  16 Upstream Organizations    │
│  Targeted: Kubernetes · gRPC · Redis · Grafana · OpenHands · Pixi · Rattler     │
└─────────────────────────────────────────────────────────────────────────────────┘
```

### 🎯 Featured Upstream Merged PRs

#### ☸️ Kubernetes (CNCF)
* **[kubernetes/kubernetes #141086](https://github.com/kubernetes/kubernetes/pull/141086):** Resolved a critical OpenAPI schema generation issue in the core API machinery by adding atomic struct markers to `EventSeries`, unblocking downstream data ingestion pipelines.

#### 📊 Grafana Labs
* **[grafana/grafana #129900](https://github.com/grafana/grafana/pull/129900):** Fixed a silent state-loss bug in the Alerting rule editor caused by an asynchronous UI race condition when dismissing the options tooltip.

#### 🤖 OpenHands (All-Hands-AI)
* **[OpenHands/OpenHands #16444](https://github.com/All-Hands-AI/OpenHands/pull/16444):** Repaired workspace directory rendering by eliminating pagination cutoff constraints, ensuring entire repository structures remain visible to autonomous agents.

#### 🦀 Rust Systems & Package Tooling (Prefix.dev, Conda, Pixi)
* **[prefix-dev/rattler-build #2266](https://github.com/prefix-dev/rattler-build/pull/2266):** Added credential-masking command execution tracing to the native bash runner, isolating build diagnostics without leaking CI secrets.
* **[prefix-dev/recipe-format #77](https://github.com/prefix-dev/recipe-format/pull/77):** Authored the canonical `build.post_process` schema specification and test suite, officially adopted maintainer-wide across the Prefix.dev ecosystem.
* **[prefix-dev/rattler-build #2254](https://github.com/prefix-dev/rattler-build/pull/2254) & [#2200](https://github.com/prefix-dev/rattler-build/pull/2200):** Authored the complete `build.post_process` specification documentation and the multi-output recipe DAG reference architecture.
* **[conda/rattler #2183](https://github.com/conda/rattler/pull/2183):** Resolved HTTP 404 package mirror download failures across enterprise corporate proxies via RFC 3986-compliant URL path joining.
* **[prefix-dev/pixi #5652](https://github.com/prefix-dev/pixi/pull/5652):** Fixed CLI panics when executing in deleted working directories through graceful fallback path resolution in `std::env` error handlers.
* **[prefix-dev/pixi #5630](https://github.com/prefix-dev/pixi/pull/5630):** Tuned cache version conflict log levels to eliminate false-alarm diagnostic spam in CI runs.

#### 🛡️ AI Agent Security & Reliability (AgentScope / QwenPaw)
* **[agentscope-ai/QwenPaw #6833](https://github.com/agentscope-ai/QwenPaw/pull/6833):** Passed required channel routing fields into the driver gate for resilient multi-agent orchestration.
* **[agentscope-ai/QwenPaw #6615](https://github.com/agentscope-ai/QwenPaw/pull/6615):** Added robust recovery handlers for corrupted agent configuration files and malformed JSON payloads.
* **[agentscope-ai/QwenPaw #6595](https://github.com/agentscope-ai/QwenPaw/pull/6595):** Secured tool execution environments against directory traversal attacks by implementing strict `realpath` containment validation.

---

### ⚡ Selected Active Contributions (In Review / Landed)

* **[grpc/grpc #43432](https://github.com/grpc/grpc/pull/43432):** Routed C-core fork handlers through `os.register_at_fork` in Python to eliminate epoll `EBADF` crashes during multi-process forking.
* **[grpc/grpc #43158](https://github.com/grpc/grpc/pull/43158):** Lazy-initialized `SharedBitGen` to prevent static initialization deadlocks on Windows platforms.
* **[grpc/grpc #43160](https://github.com/grpc/grpc/pull/43160):** Prevented static listener updates from being stalled by transiently missing dynamic xDS clusters.
* **[kubernetes/kubernetes #141089](https://github.com/kubernetes/kubernetes/pull/141089):** Fixed node lifecycle controller state machine to transition pods to `NotReady` on `False -> Unknown` node status flips.
* **[kubernetes/kubernetes #141128](https://github.com/kubernetes/kubernetes/pull/141128):** Seeded ClusterIP allocator metrics on `EnableMetrics()` to eliminate missing baseline Prometheus metrics.
* **[redis/redis #15576](https://github.com/redis/redis/pull/15576):** Fixed recursive signal handler crashes when a child fork terminates unexpectedly.
* **[redis/redis #15573](https://github.com/redis/redis/pull/15573):** Guarded against null pointer dereferences in `VRANDMEMBER` under empty-key edge cases.
* **[redis/redis #15594](https://github.com/redis/redis/pull/15594):** Root-cause investigation on heap use-after-free and iterator invalidation in `handleClientsBlockedOnKey`.
* **[cline/cline #13101](https://github.com/cline/cline/pull/13101):** Optimized the Levenshtein distance calculation in `apply_patch` to prevent UI thread freezes on massive file diffs.

---

## 🚀 Featured Engineering Projects

### [AgentGate](https://github.com/mohitdebian/AgentGate) · Runtime Authorization Firewall for AI Agents
* **Stack:** Python 3.11+, PyTorch, Qwen 0.8B, Hugging Face, Node.js 22+, React 19, Docker
* Designed an out-of-process, fail-closed authorization firewall that intercepts agent tool invocations (`bash`, `sql`, `webhooks`) before execution.
* Evaluates prompt injection, privilege escalation, and blast radius in **<35ms** via a custom neural classification head fine-tuned on Qwen-0.8B, enforcing determinism through `policy.yaml`.
* Deployed with a live [Hugging Face Space Interactive Playground](https://huggingface.co/spaces/codeload/agentgate-demo) and published [Hugging Face Model Checkpoints](https://huggingface.co/codeload/agentgate-qwen-0.8b).

### [Relay](https://github.com/mohitdebian/relay) · High-Performance API Management Platform & Gateway
* **Stack:** Go, PostgreSQL, Redis, Next.js, Docker
* Built a lightweight self-hosted API gateway providing millisecond-level reverse proxying, token-bucket rate limiting, and encrypted API key validation.
* Engineered an asynchronous, non-blocking PostgreSQL audit logger flushing high-volume request streams with zero proxy latency overhead.
* Features a full Next.js control plane with real-time analytics, per-key rate limit customization, and webhook dispatching.

### [Volt](https://github.com/mohitdebian/Volt) · Native AI Terminal
* **Stack:** Rust, Tauri, portable-pty, xterm.js
* Engineered a native terminal with sub-100MB memory footprint and sub-40ms cold start latency.
* Implemented a custom Rust AST parsing layer that analyzes input command syntax to detect and intercept destructive shell operations before dispatch.

### [Kairo](https://github.com/mohitdebian/Kairo) · Multi-Process Desktop Workspace
* **Stack:** Electron, TypeScript, React, Node.js IPC
* Built a multi-process browser and workspace isolating tabs into distinct OS-level containers for memory and security sandboxing.
* Features an aggressive memory manager that detects idle background renderer processes and reclaims inactive heap memory under high load.

---

## 🛠️ Technical Arsenal

| Category | Technologies & Tools |
|---|---|
| **Core Languages** | Rust · C++ · Go · TypeScript · Python · C · SQL · Bash |
| **Systems & Concurrency** | Linux Syscalls · POSIX Threads · AsyncIO · Goroutines · IPC · PTY · Valgrind |
| **Cloud & Infrastructure** | Kubernetes · Docker · PostgreSQL · Redis · gRPC · Envoy · Next.js · Prometheus |
| **Reliability & Security** | Static Analysis · AST Parsing · Fail-Closed Runtimes · Threat Modeling · CI/CD Pipelines |

---

<div align="center">

```txt
"Understanding complex distributed systems deeply and leaving them more reliable than found."
```

[![Connect on LinkedIn](https://img.shields.io/badge/Connect_on_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/mohitdebian)
[![Visit Portfolio](https://img.shields.io/badge/View_Portfolio-F25C2A?style=for-the-badge&logo=googlechrome&logoColor=white)](https://mohitbuilds.in)

</div>
