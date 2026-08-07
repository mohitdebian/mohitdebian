<div align="center">

# Mohit

### Open-source bug fixer and builder of developer tools, agentic workflows, and terminal-first products.

[![X](https://img.shields.io/badge/@mohitdebian-111111?logo=x&logoColor=white&style=flat-square)](https://x.com/mohitdebian)
[![LinkedIn](https://img.shields.io/badge/mohitdebian-0A66C2?logo=linkedin&logoColor=white&style=flat-square)](https://linkedin.com/in/mohitdebian)
[![Peerlist](https://img.shields.io/badge/mohitdevlabs-00AA45?logo=peerlist&logoColor=white&style=flat-square)](https://peerlist.io/mohitdevlabs)
[![Website](https://img.shields.io/badge/mohitbuilds.in-F25C2A?style=flat-square)](https://mohitbuilds.in)

</div>

I like working on code that has sharp edges.

That usually means one of two things:

- fixing crashes, panics, invalid states, and edge-case behavior in large open-source systems
- building tools for developers around terminals, browsing, automation, and contribution workflows

## Open source snapshot

This is a real snapshot of the work visible on my GitHub as of August 2, 2026.

### Recent upstream contribution targets

- [Kubernetes](https://github.com/kubernetes/kubernetes): metrics, API schema correctness, controller behavior, and kubectl fixes
- [Redis](https://github.com/redis/redis): crash fixes, null dereferences, use-after-free bugs, and integer overflow cases
- [gRPC](https://github.com/grpc/grpc): core/compiler warnings and Python runtime behavior
- [Envoy](https://github.com/envoyproxy/envoy): transport socket edge-case fixes
- [Grafana](https://github.com/grafana/grafana): dashboard, alerting, and date/week-resolution fixes
- [Openwork](https://github.com/different-ai/openwork): startup, config, and local MCP server fixes
- [QwenPaw](https://github.com/agentscope-ai/QwenPaw): agent config, shell execution, subagent schema, and provider support

### Merged or landed contribution examples

I actively contribute to the Rust package-management ecosystem and core systems architecture. **Currently at 7 PRs merged directly into production by core maintainers across 4 repositories.**

#### 🦀 Rust Ecosystem (Prefix.dev, Conda, Pixi)
* **[Prefix.dev / Rattler-Build](https://github.com/prefix-dev/rattler-build):** 
  * Added command execution tracing in the native bash runner to isolate error diagnostics while masking sensitive environment credentials from public CI logs ([Merged PR #2266](https://github.com/prefix-dev/rattler-build/pull/2266)). 
  * Authored the `build.post_process` schema documentation ([Merged PR #2254](https://github.com/prefix-dev/rattler-build/pull/2254)).
  * Documented the multi-output recipe DAG reference architecture for multi-package build pipelines ([Merged PR #2200](https://github.com/prefix-dev/rattler-build/pull/2200)).
* **[Prefix.dev / Recipe-Format](https://github.com/prefix-dev/recipe-format):** 
  * Authored the canonical `build.post_process` schema and accompanying test suite, adopted across the recipe specification at the maintainer's invitation ([Merged PR #77](https://github.com/prefix-dev/recipe-format/pull/77)).
* **[Conda / Rattler](https://github.com/conda/rattler):** 
  * Resolved HTTP 404 package download failures across corporate proxy environments by implementing RFC 3986-compliant URL path joining, preserving enterprise mirror sub-path hierarchies ([Merged PR #2183](https://github.com/conda/rattler/pull/2183)).
* **[Prefix.dev / Pixi](https://github.com/prefix-dev/pixi):** 
  * Fixed unhandled CLI panics from deleted working directories via fallback path resolution in `std::env` error handlers ([Merged PR #5652](https://github.com/prefix-dev/pixi/pull/5652)).
  * Tuned cache version-conflict log severity to cut CI diagnostic noise ([Merged PR #5630](https://github.com/prefix-dev/pixi/pull/5630)).

#### 🛡️ C & Python Security Contributions
* **[Redis Core](https://github.com/redis/redis):** Investigated a critical use-after-free vulnerability and iterator invalidation in the core blocking-key wakeup engine (`handleClientsBlockedOnKey`). Root-cause analysis adopted upstream by core maintainers ([Adopted PR #15594](https://github.com/redis/redis/pull/15594)).
* **[QwenPaw (AgentScope)](https://github.com/agentscope-ai/QwenPaw):** Secured autonomous LLM tool execution by identifying directory traversal vulnerabilities and designing strict realpath workspace containment validation ([Adopted PR #6595](https://github.com/agentscope-ai/QwenPaw/pull/6595)).

### Active contribution examples

- [kubernetes/kubernetes](https://github.com/kubernetes/kubernetes): [Seed ClusterIP allocator metrics on EnableMetrics()](https://github.com/kubernetes/kubernetes/pull/141128)
- [redis/redis](https://github.com/redis/redis): [Fix recursive crash in signal handler when child process crashes](https://github.com/redis/redis/pull/15576)
- [grpc/grpc](https://github.com/grpc/grpc): [[Python] Fix SyncServicerContext abort not raising exception](https://github.com/grpc/grpc/pull/43126)
- [envoyproxy/envoy](https://github.com/envoyproxy/envoy): [fix proxy protocol format_string in added_tlvs](https://github.com/envoyproxy/envoy/pull/46497)

## 🚀 Selected Projects

These are the projects from my own repositories that are worth featuring right now, intentionally leaving out forks and placeholders to focus on high-signal engineering.

### [Volt](https://github.com/mohitdebian/Volt) | Native AI Terminal
* **Stack:** Rust, Tauri, PTY, xterm.js
* Built a native terminal achieving sub-100MB RAM usage and 40ms cold starts (verified via Valgrind & Hyperfine) by leveraging Rust `portable-pty` bindings.
* Includes a Rust AST-based command safety analyzer that evaluates input execution risks and dynamically intercepts destructive OS operations before execution.

### [Kairo](https://github.com/mohitdebian/Kairo) | Multi-Process Desktop Browser
* **Stack:** Electron, TypeScript, React, IPC
* Developed a multi-process browser isolating web content into secure containers for enhanced rendering stability, featuring an LLM-assisted context grouping engine.
* Designed an aggressive memory manager that automatically deallocates inactive background tab renderer processes, preventing memory leaks during heavy multitasking.

### [AlgoMerge](https://github.com/mohitdebian/AlgoMerge) | Open-Source Issue Discovery
* **Stack:** React, Next.js, GraphQL, Node.js
* Engineered a GraphQL-powered algorithmic contribution scoring engine that analyzes repository metadata to rank open-source issues by lowest contributor competition.
* Optimized GitHub API integration with client-side state caching, drastically reducing API latency and preventing rate-limit throttling.

### [Senior OSS Engineer Skill](https://github.com/mohitdebian/Senior-Open-Source-Engineer-Skill) | AI Agent Workflow
* A robust, reusable workflow architecture for autonomous AI coding agents designed specifically for contributing to mature open-source codebases.
* Enforces strict engineering rigor: smaller Git diffs, strong pre-commit debugging, and maintainer-friendly PR formatting.

### [GitSweep](https://github.com/mohitdebian/GitSweep) | CLI Automation Utility
* Developed a high-speed terminal utility for safely parsing and bulk-deleting GitHub repositories.
* Implemented strict explicit confirmation safeguards and optimized network requests for rapid repository lifecycle management.

### [YOINK](https://github.com/mohitdebian/YOINK) | Data Extraction Engine
* Built a dynamic extraction tool for reliably harvesting data or actions from obfuscated websites and internal APIs when clean integration paths do not exist.

## Stack

```txt
Go · Rust · TypeScript · Python · C · C++ · Node.js
Systems debugging · CLI tooling · OSS contribution workflows · full-stack product work
```

<div align="center">
<sub>No stat cards here on purpose. Reliability is better than broken vanity widgets.</sub>
</div>
