# Mohit Singh

Backend & systems developer. I spend most of my time hunting edge-case bugs in large open-source codebases and building developer tools.

[Website](https://mohitbuilds.in) · [LinkedIn](https://linkedin.com/in/mohitdebian) · [GitHub](https://github.com/mohitdebian) · [Email](mailto:mohitdebian@gmail.com)

---

### What I Do

I like digging into code where things break in subtle ways—concurrency races, memory leaks, panics in edge cases, and unexpected state transitions. 

Over the past year, I've opened **77 pull requests across 16 open-source projects** (Kubernetes, gRPC, Redis, Grafana, OpenHands, Pixi, Rattler, and others), with 12+ merged directly upstream.

---

### Selected Upstream Contributions

#### Kubernetes
- **[kubernetes/kubernetes #141086](https://github.com/kubernetes/kubernetes/pull/141086)** (Merged) — Added atomic struct markers to `EventSeries` to fix OpenAPI schema generation in the API machinery.
- **[kubernetes/kubernetes #141089](https://github.com/kubernetes/kubernetes/pull/141089)** (Open) — Fix node lifecycle controller to mark pods `NotReady` on `False -> Unknown` node transitions.
- **[kubernetes/kubernetes #141128](https://github.com/kubernetes/kubernetes/pull/141128)** (Open) — Seed ClusterIP allocator metrics on `EnableMetrics()`.

#### gRPC
- **[grpc/grpc #43432](https://github.com/grpc/grpc/pull/43432)** (Open) — Route C-core fork handlers through Python's `os.register_at_fork` to stop epoll `EBADF` crashes in multi-process apps.
- **[grpc/grpc #43158](https://github.com/grpc/grpc/pull/43158)** (Open) — Lazy-initialize `SharedBitGen` to prevent static init hangs on Windows.
- **[grpc/grpc #43160](https://github.com/grpc/grpc/pull/43160)** (Open) — Prevent missing dynamic clusters from stalling static xDS updates.

#### Redis
- **[redis/redis #15576](https://github.com/redis/redis/pull/15576)** (Open) — Fix recursive crashes in signal handlers when child processes crash.
- **[redis/redis #15573](https://github.com/redis/redis/pull/15573)** (Open) — Guard against null pointer dereference in `VRANDMEMBER`.
- **[redis/redis #15594](https://github.com/redis/redis/pull/15594)** — Root-cause investigation on heap use-after-free and iterator invalidation in `handleClientsBlockedOnKey`.

#### Grafana
- **[grafana/grafana #129900](https://github.com/grafana/grafana/pull/129900)** (Merged) — Fixed a UI race condition in Alerting rule editor where tooltip values were lost on outside click.

#### Rust Ecosystem (Prefix.dev / Conda / Pixi)
- **[prefix-dev/rattler-build #2266](https://github.com/prefix-dev/rattler-build/pull/2266)** (Merged) — Added command execution tracing in the bash runner while masking sensitive environment credentials in CI.
- **[prefix-dev/recipe-format #77](https://github.com/prefix-dev/recipe-format/pull/77)** (Merged) — Authored the canonical `build.post_process` schema and test suite for the recipe specification.
- **[conda/rattler #2183](https://github.com/conda/rattler/pull/2183)** (Merged) — Fixed HTTP 404s when downloading from corporate proxy mirrors by enforcing RFC 3986 path joining.
- **[prefix-dev/pixi #5652](https://github.com/prefix-dev/pixi/pull/5652)** (Merged) — Handled CLI panics when running commands in deleted working directories.

#### Agent Runtimes & Dev Tools
- **[OpenHands #16444](https://github.com/All-Hands-AI/OpenHands/pull/16444)** (Merged) — Fixed workspace folder rendering so all files remain accessible past API pagination limits.
- **[QwenPaw #6833](https://github.com/agentscope-ai/QwenPaw/pull/6833)** (Merged) & **[#6615](https://github.com/agentscope-ai/QwenPaw/pull/6615)** (Merged) — Fixed driver gate channel routing and added recovery for corrupted agent config files.
- **[QwenPaw #6595](https://github.com/agentscope-ai/QwenPaw/pull/6595)** (Merged) — Blocked directory traversal in agent tool execution using strict `realpath` containment.
- **[cline #13101](https://github.com/cline/cline/pull/13101)** (Open) — Optimized Levenshtein distance in `apply_patch` to prevent UI thread hangs on large diffs.

---

### Projects

- **[AgentGate](https://github.com/mohitdebian/AgentGate)** — Runtime authorization firewall for AI agents. Intercepts bash/sql/webhook calls out-of-process and scores injection and blast radius in under 35ms using a fine-tuned Qwen 0.8B head + deterministic `policy.yaml`. Includes a React dashboard, live [Hugging Face Space](https://huggingface.co/spaces/codeload/agentgate-demo), and published [model checkpoints](https://huggingface.co/codeload/agentgate-qwen-0.8b).
- **[Relay](https://github.com/mohitdebian/relay)** — API gateway written in Go. Token-bucket rate limiting, non-blocking PostgreSQL audit logger, and a Next.js admin dashboard.
- **[Volt](https://github.com/mohitdebian/Volt)** — Lightweight native terminal in Rust and Tauri with sub-100MB RAM usage, sub-40ms cold start, and AST-based command interception for dangerous operations.
- **[Kairo](https://github.com/mohitdebian/Kairo)** — Multi-process desktop browser built with Electron, TypeScript, and React with tab-level process isolation and automatic memory cleanup for idle tabs.

---

### Stack

- **Languages:** Rust, C++, Go, TypeScript, Python, C
- **Systems & Infra:** Linux, POSIX Threads, AsyncIO, Docker, Kubernetes, PostgreSQL, Redis, gRPC
