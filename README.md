# Andrew Klapper

Senior Full-Stack & Systems Engineer in Marietta, GA.

[andrew-k.us](https://andrew-k.us) | [Agensi Skills](https://agensi.io/creators/aklapper) | [JetBrains Marketplace](https://plugins.jetbrains.com/plugin/36539-solar-forge-theme) | [andrew@andrew-k.us](mailto:andrew@andrew-k.us)

I build production web platforms, distributed Go and .NET 10 backends, native C++/Qt6 desktop and Kotlin Android apps, and local multi-GPU AI tooling. Before moving into software full time, I owned and ran a freight brokerage in Marietta, GA. Physical logistics taught me to prefer explicit failure modes and clear state transitions over software that quietly papers over bad inputs.

For an interactive look at my work, visit [andrew-k.us](https://andrew-k.us). The site runs as a browser terminal workspace with an AI assistant grounded in my published career dossiers at [`/chat`](https://andrew-k.us/chat) (including job-description fit checks) and a live specification-to-sandbox workbench at [`/cadence`](https://andrew-k.us/cadence).

---

## Featured projects

### [andrew-k.us (`aklapper`)](https://github.com/AndrewK4758/aklapper) (`v1.0.0`)

My personal engineering portfolio, grounded AI career assistant, interactive CADENCE sandbox, and Direct-IAP admin console. Built as an Nx 24 monorepo with React 19 and React Router 8 streaming SSR on Fastify 5, Go 1.27 AI and sandbox microservices, PostgreSQL 19 with Drizzle ORM, Qdrant vector search, cookieless in-process MaxMind GeoLite2 analytics, and WebAuthn passkeys, Argon2id, and TOTP admin authentication, deployed scale-to-zero on Google Cloud Run.

### [Ghostty Union](https://github.com/AndrewK4758/ghostty-union) (`v1.0.0`)

Native cross-platform C++20 and Qt6 Widgets terminal emulator powered by `libghostty-vt 1.0+` for Linux, WSL2, macOS, and Windows (ConPTY). Supports Kitty Graphics Protocol and iTerm2 inline images with 5-layer HiDPI compositing and a built-in image inspector, drag-and-drop nested split trees, session and layout persistence, leaked TUI mode recovery after `OSC 133;D`, and a mounted 74px live system telemetry bar.

### [Solar Forge Theme](https://github.com/AndrewK4758/jetbrains-solar-forge-theme) (`v1.0.0`, [JetBrains Marketplace](https://plugins.jetbrains.com/plugin/36539-solar-forge-theme))

Native JetBrains Islands Dark UI theme and matching editor and terminal color scheme. Shipped as a pure resource-only plugin with zero Java classes and no Material Theme UI dependency, built around Warm Tungsten Ash surfaces (`#24221F` / `#181716`) with Cyber Gold (`#FFD300`) and Vermilion Blaze (`#FF3D00`) accents.

### [Gemma 4 Dual-GPU Coding Pipeline](https://github.com/AndrewK4758/gemma-coding-pipeline)

End-to-end local fine-tuning and export pipeline for Gemma 4 (`E4B` and `26B-A4B MoE`) on an asymmetric 16 GB + 12 GB dual-GPU Linux workstation. Uses static layer sharding across slow PCIe links, 256-token chunked vocabulary cross-entropy for the 262K vocab, bfloat16/NF4 QLoRA SFT, compiler-verified DPO with zero-VRAM reference log-probability caching, online GRPO across 32-thread compiler sandboxes (`tsc`, `go`, `.NET 10 Roslyn`, `gcc`/`g++`), and export to `llama.cpp` GGUF, Ollama, and vLLM.

### [Antigravity Remote Android](https://github.com/AndrewK4758/Antigravity-Android-Wrapper)

Standalone Kotlin Android client for Google Antigravity Remote Control built on embedded Mozilla GeckoView (`org.mozilla.geckoview`). Keeps persistent session storage, handles Google Account sign-in without WebView user-agent blocks, and supports `/r/<instance-id>` deep links across Android 10 through 17.

### Distributed AI document processing microservices

Stateless gRPC, Protobuf, and NATS JetStream DAG pipeline for multi-tenant document extraction, semantic caching, human-in-the-loop escalation, and immutable audit trails across Go, C++, and C#:

[`orchestrator_service`](https://github.com/AndrewK4758/orchestrator_service) | [`ai_service`](https://github.com/AndrewK4758/ai_service) | [`semantic-cache`](https://github.com/AndrewK4758/semantic-cache) | [`human_in_the_middle_service`](https://github.com/AndrewK4758/human_in_the_middle_service) | [`document-chunking-service`](https://github.com/AndrewK4758/document-chunking-service) | [`traceability_service`](https://github.com/AndrewK4758/traceability_service) | [`shared_protos`](https://github.com/AndrewK4758/shared_protos)

### Open-source contributions

Contributor to [Blitz](https://github.com/retail-cortex/blitz), a Go coding agent built on Google ADK.

---

## CADENCE and published agent skills

I build and maintain CADENCE, a provider-neutral, 7-phase governed agentic SDLC framework paired with a strictly read-only local GPU FastMCP coprocessor (`llama.cpp` and `llama-swap`) for AST semantic code search, test and build log compaction, and pre-PR review. Try the interactive workflow at [andrew-k.us/cadence](https://andrew-k.us/cadence) or browse my published skills on [Agensi](https://agensi.io/creators/aklapper):

| Skill | Focus |
| --- | --- |
| [CADENCE: Governed Agentic SDLC Framework](https://agensi.io/skills/cadence-governed-agentic-sdlc-framework) | 7-phase workflow, 12 specialist roles, CHORD behavioral specs, strict BDD/TDD, and 4 human approval gates |
| [Local GPU Coprocessor Offload (FastMCP)](https://agensi.io/skills/local-gpu-coprocessor-offload-for-coding-agents-fastmcp) | Read-only local GPU AST semantic search, 30-line log compaction, and pre-PR diff review |
| [CADENCE CHORD Specification & Spec Challenger](https://agensi.io/skills/cadence-chord-specification-spec-challenger) | Multi-option design exploration, CHORD behavioral specs, Gherkin test plans, and pre-gate spec challenge |
| [CADENCE Adversarial Pre-PR Review Gate](https://agensi.io/skills/cadence-adversarial-pre-pr-review-gate) | Contract review, zero-spec `/tmp` fault-injection probes, and security and concurrency auditing |
| [CADENCE Safe Database Migration Author](https://agensi.io/skills/cadence-safe-database-migration-author-expand-contract) | Zero-downtime expand/contract migrations for EF Core, Alembic, Prisma, Drizzle, Room, and SQL |
| [CADENCE Triage & Risk Classifier](https://agensi.io/skills/cadence-triage-risk-classifier) | 4-axis task classification, bounded codebase recon, and structured ticket setup |

---

## Production engineering

### Build Technology Group (Software Engineer)

Architected and delivered a full-stack laboratory hardware orchestration platform as sole developer. The `.NET 10` (C#) REST API talks directly to diagnostic machinery to manage calibration state, robotic execution sequences, and regulatory audit trails, backed by a TypeScript SPA for live monitoring and control.

Modernized a legacy PHP monolith into a containerized `.NET 10` and MySQL ERP platform. Reworked Entity Framework Core data access with compiled queries and connection pooling to cut query latency by more than 40%, and moved invoicing, inbound document routing, PDF generation, and payment reconciliation onto Hangfire background pipelines.

### Gitasy (Software Engineer)

Built a distributed Go backend handling high-concurrency WebSocket connections for live drafts and notifications on a real-time daily fantasy sports platform, along with the TypeScript SPA frontend, PostgreSQL and Redis data layer, and automated Docker and GitHub Actions deployments to Azure Kubernetes Service (AKS).

---

## Core stack

| Area | Technologies |
| --- | --- |
| Languages | C# (.NET 10), Go, TypeScript, C++20, Kotlin, Python, SQL |
| Web & Native UI | React 19, React Router 8 (Streaming SSR), Fastify 5, Qt6 Widgets (`libghostty-vt`), Android SDK / Mozilla GeckoView |
| Backend & Distributed | ASP.NET Core, Entity Framework Core, gRPC, Protobuf, NATS JetStream, WebSockets, Hangfire, Bazel |
| Data & AI/ML | PostgreSQL 19 (Drizzle), MySQL, Redis, Qdrant, PyTorch (QLoRA / DPO / GRPO), `llama.cpp` / GGUF, FastMCP |
| Cloud & Tooling | Docker, Kubernetes (AKS), Google Cloud Run, GCP, Azure, AWS, GitHub Actions, Nx, Linux |

---

## Community

I instruct and mentor weekly at the Woodstock Developers Group in Woodstock, GA, covering software architecture, TDD, pair programming, code reviews, Agile/Scrum workflows, and CI/CD.
