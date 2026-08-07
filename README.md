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

## Selected projects

These are the projects from my own repos that are worth featuring right now. I am intentionally leaving out forks, placeholders, and low-signal repos.

### [Kairo](https://github.com/mohitdebian/Kairo)
Browsing, organized. A product direction around making the browser a more structured workspace.

### [Senior-Open-Source-Engineer-Skill](https://github.com/mohitdebian/Senior-Open-Source-Engineer-Skill)
A reusable workflow for AI coding agents contributing to mature open-source repositories with smaller diffs, stronger debugging, and maintainer-friendly output.

### [YOINK](https://github.com/mohitdebian/YOINK)
A tool for extracting data or actions from sites and APIs when the clean integration path does not already exist.

### [Volt](https://github.com/mohitdebian/Volt)
An ultra-lightweight AI terminal project built around fast local workflows.

### [GitSweep](https://github.com/mohitdebian/GitSweep)
A terminal utility for safely bulk-deleting GitHub repositories with explicit confirmation.

### [AlgoMerge](https://github.com/mohitdebian/AlgoMerge)
A project focused on finding promising open-source issues with lower contributor competition.

## Stack

```txt
Go · Rust · TypeScript · Python · C · C++ · Node.js
Systems debugging · CLI tooling · OSS contribution workflows · full-stack product work
```

<div align="center">
<sub>No stat cards here on purpose. Reliability is better than broken vanity widgets.</sub>
</div>
