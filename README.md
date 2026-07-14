<!--
  drafts/github-technical-v2.md
  Stage: local-only. NO push until operator phrase
    "approve publish profile-readme" / "apruebo publicar profile-readme"
  Pipeline: make check FILE=drafts/github-technical-v2.md && make preview FILE=drafts/github-technical-v2.md
  Pre-staging sweep: lzt-secret-scrubber + lzt-public-surface-curator
  Source: PROFILE_SPEC.md + lzt-profile-readme skill + lzt-louzt-profile-cartographer wrapper

  Block-level structure (researcher-first funnel, 2026-07-13 + Public Signal merged 2026-07-14):
    [HEADER SVG] → metadata table (4 rows: contact / identity / tech / categories) →
    About (no title, single long hook line) →
    [How I work] →
    [Selected Work + Posture summary] (Public Signal fused into Selected Work 2026-07-14;
      Posture summary table sits above the project table under the same section SVG;
      duplicates trimmed; SRE Harness sovereign-math gist + 5-tier proxy 2 gists added) →
    [What we ship at loust.pro] →
    [Research & Publications] → [Investigations & Notes] →
    [FOOTER SVG] → doc meta
  Visual rhythm: SVG blocks, mermaid blocks, and table blocks intersperse
  paragraphs so the read alternates between narrative and structured data.
  Mermaid blocks retained: Sovereign RAG (TB, theorems) only.
  Selected Work ordering (2026-07-14 per operator directive): LZT SRE Harness →
  5-tier proxy → LOUST multi-tenant → Nexus Engine → SnapPipe → NetBoozt →
  TaxonRouter → SypremeMX+SYPREME combined → Tren Maya → spec-snapshot-scraper →
  Upstream hardening (Bottles/Waypaper/linux-wallpaperengine) → Built-in signal
  pipeline → public org repos (deterministic-sovereign-rag+dsvh-verification-suite,
  ical-to-caldav, LLMmempipe, Apr1ClaudeDirectives-Leak).
-->

<!-- ============================================================ -->
<!-- HEADER (minimal SVG: loust logo + status + Let's work        -->
<!-- together CTA + LinkedIn + partnership email).                 -->
<!-- ============================================================ -->
<div align="center">
  <!-- Header SVG: /static/profile-header.svg is served by the preview server.
         Production host (raw.githubusercontent.com or gist) decided at publish time. -->
  <img alt="loust.pro — Let's work together" src="/static/profile-header.svg" width="100%" />
</div>

<!-- ============================================================ -->
<!-- METADATA: 4-row stack, left-aligned.                        -->
<!-- Row 1 (NEW 2026-07-14): contact channels — LinkedIn,        -->
<!--   GitLab, X.com, Matrix. Same style as the SVG pills so the  -->
<!--   reader can match them visually.                            -->
<!-- Row 2: identity — ProfileViews + ORCID + OSI + Linux Kernel.  -->
<!-- Row 3: tech stack (programming langs + infra).              -->
<!-- Row 4: tech categories + Call-to-Value recruitment badge.   -->
<!-- ============================================================ -->
<table width="100%">
  <tr>
    <td align="left" valign="middle">
      <a href="https://www.linkedin.com/in/davidmirelesll/?locale=es_ES"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
      <a href="#"><img src="https://img.shields.io/badge/GitLab-FC6D26?style=flat-square&logo=gitlab&logoColor=white" alt="GitLab"/></a>
      <a href="#"><img src="https://img.shields.io/badge/X-000000?style=flat-square&logo=x&logoColor=white" alt="X.com"/></a>
      <a href="#"><img src="https://img.shields.io/badge/Matrix-000000?style=flat-square&logo=matrix&logoColor=white" alt="Matrix"/></a>
    </td>
  </tr>
  <tr>
    <td align="left" valign="middle">
      <a href="https://komarev.com/ghpvc/?username=louzt&label=profile+views&color=1e293b&style=flat-square"><img src="https://komarev.com/ghpvc/?username=louzt&label=profile+views&color=1e293b&style=flat-square" alt="Profile Views"/></a>
      <a href="https://orcid.org/0009-0008-4374-2254"><img src="https://img.shields.io/badge/ORCID-0009--0008--4374--2254-A6CE39?style=flat-square&logo=orcid&logoColor=white" alt="ORCID iD 0009-0008-4374-2254"/></a>
      <a href="https://opensource.org/"><img src="https://img.shields.io/badge/OSI-Member-3DA639?style=flat-square&logo=opensourceinitiative&logoColor=white" alt="OSI Member"/></a>
      <a href="https://kernel.org/"><img src="https://img.shields.io/badge/Linux_Kernel-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux Kernel"/></a>
    </td>
  </tr>
  <tr>
    <td align="left" valign="middle">
      <a href="#"><img src="https://img.shields.io/badge/rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust"/></a>
      <a href="#"><img src="https://img.shields.io/badge/go-00add8?style=flat-square&logo=go&logoColor=white" alt="Go"/></a>
      <a href="#"><img src="https://img.shields.io/badge/typescript-3178c6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/></a>
      <a href="#"><img src="https://img.shields.io/badge/python-3776ab?style=flat-square&logo=python&logoColor=ffd43b" alt="Python"/></a>
      <a href="#"><img src="https://img.shields.io/badge/perl-0298c3?style=flat-square&logo=perl&logoColor=white" alt="Perl"/></a>
      <a href="#"><img src="https://img.shields.io/badge/graphql-e10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/></a>
      <a href="#"><img src="https://img.shields.io/badge/postgresql-4169e1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/></a>
      <a href="#"><img src="https://img.shields.io/badge/redis-dc382d?style=flat-square&logo=redis&logoColor=white" alt="Redis"/></a>
      <a href="#"><img src="https://img.shields.io/badge/k3s-ffc61c?style=flat-square&logo=kubernetes&logoColor=black" alt="k3s"/></a>
      <a href="#"><img src="https://img.shields.io/badge/docker-2496ed?style=flat-square&logo=docker&logoColor=white" alt="Docker"/></a>
      <a href="#"><img src="https://img.shields.io/badge/c-A8B9CC?style=flat-square&logo=c&logoColor=white" alt="C"/></a>
      <a href="#"><img src="https://img.shields.io/badge/c++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white" alt="C++"/></a>
      <a href="#"><img src="https://img.shields.io/badge/flutter-02569B?style=flat-square&logo=flutter&logoColor=white" alt="Flutter"/></a>
      <a href="#"><img src="https://img.shields.io/badge/WebRTC-333333?style=flat-square&logo=webrtc&logoColor=white" alt="WebRTC"/></a>
      <a href="#"><img src="https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white" alt="PHP"/></a>
      <a href="#"><img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white" alt="Node.js"/></a>
      <a href="#"><img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"/></a>
      <a href="#"><img src="https://img.shields.io/badge/Lua-2C2D72?style=flat-square&logo=lua&logoColor=white" alt="Lua"/></a>
      <a href="#"><img src="https://img.shields.io/badge/Ruby-CC342D?style=flat-square&logo=ruby&logoColor=white" alt="Ruby"/></a>
      <a href="#"><img src="https://img.shields.io/badge/Always_curious_to_debug_in_another_language-8b5cf6?style=flat-square&logoColor=white" alt="Always curious to debug in another language"/></a>
    </td>
  </tr>
  <tr>
    <td align="left" valign="middle">
      <a href="#"><img src="https://img.shields.io/badge/google-4285f4?style=flat-square&logo=google&logoColor=white" alt="Google Ads"/></a>
      <a href="#"><img src="https://img.shields.io/badge/meta-1877f2?style=flat-square&logo=meta&logoColor=white" alt="Meta Ads"/></a>
      <a href="#"><img src="https://img.shields.io/badge/blockchain-121D33?style=flat-square&logo=blockchaindotcom&logoColor=white" alt="Blockchain"/></a>
      <a href="#"><img src="https://img.shields.io/badge/CRM-00A1E0?style=flat-square&logo=salesforce&logoColor=white" alt="CRM"/></a>
      <a href="#"><img src="https://img.shields.io/badge/ERP-714B67?style=flat-square" alt="ERP"/></a>
      <a href="#"><img src="https://img.shields.io/badge/SaaS--to--SaaS-2C3E50?style=flat-square" alt="SaaS-to-SaaS"/></a>
      <a href="#"><img src="https://img.shields.io/badge/IA--Research-7c3aed?style=flat-square" alt="IA Research"/></a>
      <a href="mailto:partnership@loust.pro?subject=We'd%20like%20to%20contribute%20to%20your%20infrastructure"><img src="https://img.shields.io/badge/Open_to_contribute-22d3ee?style=flat-square&logoColor=020617" alt="Open to contribute — we'd like to support your infrastructure"/></a>
    </td>
  </tr>
</table>

I design and ship production systems where the boundary between application delivery and systems engineering has to hold. Most of my work is research-flavored engineering: the abstractions are reusable, the proofs are formal where they need to be, and the operational evidence is auditable end-to-end.

<p align="center"><img src="/static/section-how-i-work.svg" width="100%" alt="How I work — section banner"/></p>

- **Infrastructure as substrate.** I harden network and service layers before asking application code to carry business load.
- **Decision plane first.** I reverse-engineer edge cases down to runtime behaviour until root cause and architectural boundary are explicit.
- **Atomic abstraction.** I build with reusable adapters, wrappers, and isolated components so complexity does not decay into legacy glue.
- **Flow-first AI.** I optimize context reuse, caching, and execution loops before paying for token bloat.
- **KPI-driven optimization.** I benchmark and stress-test until throughput, cost, latency, and operational KPIs are genuinely competitive.
- **Governance and review.** I keep sensitive infrastructure redacted, ship scoped PRs, and use review as a two-way learning loop.

<p align="center"><img src="/static/section-working-with-me.svg" width="100%" alt="Working with me — section banner"/></p>

### Working with me

- **Feedback and learning** — if you see me somewhere learning to work better inside a software team, I'm interested. Senior reviewers, engineering leads, or teammates who have a specific technical observation — a code review thread, a shared codebase, a process friction — are welcome to reach out. I treat feedback as a two-way loop, not a one-way deliverable; the best learning posture is to keep the audit trail legible on both sides.
- **HackerOne disclosure track** — vulnerability reports and coordinated disclosure for infrastructure under our scope route through [security@loust.pro](mailto:security@loust.pro). Triaged within 72 hours; reproducible PoCs and a minimum-scope patch suggestion move reports to the front of the queue. Out-of-scope signals (DMS, PipeWire hardening) and known-busy triage windows are documented so reporters don't spin.
- **Research collaborations** — formal proofs, deterministic systems, transport-layer hardening, sovereign AI infra. Best fit: PhD-track independent researchers, applied-probability / IR communities, agent-framework authors. Reach out at [research@loust.pro](mailto:research@loust.pro) with a 1-paragraph abstract and a concrete artifact (gist, paper draft, benchmark).
- **OSS upstream hardening** — if you maintain an OSS project where the runtime model is well-bounded (lifecycle contracts, allocator hot paths, compositor or daemon boundaries), I'd like to talk. I take scoped PRs against the runtime boundary; bring a reproducer + a minimum-scope patch, not a slide deck. Open invite — long-running contributor or co-maintainer track.
- **B2B platform work / partnerships** — long-horizon engagements only. No sprint theatre; we build the substrate, the observability, and the audit trail first. Reach out at [partnership@loust.pro](mailto:partnership@loust.pro).
- **Reference policy** — I write public references for shipped work with measurable outcomes. Send the PR / artifact link and a 1-line outcome metric; I respond within a week.

<p align="center"><img src="/static/section-selected-work.svg" width="100%" alt="Selected Work — section banner"/></p>

Production systems that have either shipped to real users, merged into upstreams, or run as long-lived client platforms — plus the cross-cutting posture they map to. Public artefacts link out; private platforms are referenced by name only — the boundary between public proof and client-confidential work is deliberate, reviewable, and unchanged across engagements.

| Project | Focus | Why it matters |
| --- | --- | --- |
| **OSS hardening upstream** | PipeWire / Freedesktop (handshake timeout in `module-protocol-native`), NGINX Core (CRLF sanitization via `r->pool`), Bottles (Manager lifecycle isolation), Waypaper (#278-#286), linux-wallpaperengine (#574, #576), Chromium 148 CSP (Opera GB-80414) | Cross-runtime model coverage: pipewire C daemon, nginx `r->pool` allocator, GTK subprocess teardown, wlr-layer-shell + presentation-time contracts, browser CSP L3 |
| **AI / RAG systems** | 50K embeddings queried in 188 ms across GPU-backed retrieval pipelines. MCP surfaces shipped as JSON-RPC stdio servers for agent tooling (image / TTS / video / web search) | Local RAG substrate with O(1) compaction, FNV-1a 64-bit signed-hash projection, and zero telemetry egress |
| **Network & infrastructure** | 15-20% throughput improvements in NetBoozt test cases. Hardened Linux VPS from bare-metal substrate up: sshd hardening, multi-tenant isolation, automated state snapshots, 5-tier QUIC/SSH fallback proxy | Bare-metal-to-app substrate kept under one operator's audit trail |
| **Release hygiene** | Scoped PRs, deterministic tooling, audit-first workflows, evidence chains and provenance over volume | OSS-safe extraction only when the abstraction boundary is legible and useful to other engineers |
| **LZT SRE Harness** (private) | Distributed data plane in Rust + Go: routing, cache control, and a hardened tool-call pipeline for autonomous agents. Backed by the [Sovereign RAG math gist](https://gist.github.com/louzt/d1ce71c05460c2c32bf31342cd0c6a3f) (English) / [Las Matemáticas del Sovereign RAG](https://gist.github.com/louzt/a75f9cf1a2f2edbd5af0e8d23526871d) (Español) | Decouples orchestration from model-provider volatility; 3-way semantic sync + Bayesian Stream Guard with <0.5s kill-switch on hallucination risk. Sovereign-RAG substrate gives the control plane a deterministic, locally-auditable retrieval signal.<br/><br/><a href="#"><img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust"/></a> <a href="#"><img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white" alt="Go"/></a> <a href="#"><img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/></a> <a href="#"><img src="https://img.shields.io/badge/Bayesian_Stream_Guard-8B5CF6?style=flat-square" alt="Bayesian Stream Guard"/></a> <a href="#"><img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis"/></a> |
| **5-tier multi-protocol transport proxy** (private) | Go + Rust proxy that races QUIC / Hysteria2 / direct TLS / SSH to evade ISP-grade DPI and TCP Cubic collapse under 5% packet drops. Public gists: [5-tier evasion chain (v1.0)](https://gist.github.com/louzt/3991f144c7d67726045af3cefc60f42a) + [5-layer fallback SSH chain](https://gist.github.com/louzt/e318d7e0ae1fd676d124311c80585f74) | First-healthy-stream promotion in <200 ms sidesteps Linux exponential retransmits; CA-pinning closes MITM and POSIX-safe atomic writes keep state file drift off the NVMe.<br/><br/><a href="#"><img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white" alt="Go"/></a> <a href="#"><img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust"/></a> <a href="#"><img src="https://img.shields.io/badge/QUIC-0093D0?style=flat-square" alt="QUIC"/></a> <a href="#"><img src="https://img.shields.io/badge/Hysteria2-1F2937?style=flat-square" alt="Hysteria2"/></a> <a href="#"><img src="https://img.shields.io/badge/TLS-2C3E50?style=flat-square" alt="TLS"/></a> <a href="#"><img src="https://img.shields.io/badge/SSH-000000?style=flat-square" alt="SSH"/></a> |
| **h4kken** (private, deployed at h4kken.loust.pro) | 3D fighting game with rollback netcode, WebSocket relay that upgrades to WebRTC DataChannel, optional TURN/COTURN credentials. Babylon.js 8 renderer, Bun + Vite + TypeScript strict | Online matches survive flaky NATs and ISP DPI: WebSocket→WebRTC upgrade, WebSocket fallback if upgrade fails, optional TURN keeps mobile peers reachable. Rollback netcode keeps input resolution deterministic across independent client clocks.<br/><br/><a href="#"><img src="https://img.shields.io/badge/Bun-000000?style=flat-square&logo=bun&logoColor=white" alt="Bun"/></a> <a href="#"><img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/></a> <a href="#"><img src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white" alt="Vite"/></a> <a href="#"><img src="https://img.shields.io/badge/Babylon.js_8-000000?style=flat-square&logo=babylondotjs&logoColor=white" alt="Babylon.js 8"/></a> <a href="#"><img src="https://img.shields.io/badge/WebSocket-2C3E50?style=flat-square" alt="WebSocket"/></a> <a href="#"><img src="https://img.shields.io/badge/WebRTC-333333?style=flat-square&logo=webrtc&logoColor=white" alt="WebRTC"/></a> <a href="#"><img src="https://img.shields.io/badge/TURN%2FCOTURN-7C3AED?style=flat-square" alt="TURN/COTURN"/></a> |
| **LOUST multi-tenant platform** (current, 7y6m) | Founder + principal architect across CRMs, ERPs, booking, ads ingestion (Meta + Google Ads → PostgreSQL), and a provisioned Linux VPS substrate | Long-horizon evidence — seven years shipping production B2B without resetting the substrate; concurrent ingestion pipelines and isolated PG/Redis namespaces keep tenants off each other.<br/><br/><a href="#"><img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/></a> <a href="#"><img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis"/></a> <a href="#"><img src="https://img.shields.io/badge/Prisma-3982CE?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/></a> <a href="#"><img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/></a> <a href="#"><img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"/></a> <a href="#"><img src="https://img.shields.io/badge/Astro-BC52EE?style=flat-square&logo=astro&logoColor=white" alt="Astro"/></a> <a href="#"><img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/></a> |
| **Nexus Engine** (private) | Spec-driven generators and platform scaffolding across multi-app TypeScript ecosystems | 9 packages / 391 TypeScript files keep larger ecosystems consistent from a single source of truth instead of copy-pasting boilerplate.<br/><br/><a href="#"><img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/></a> <a href="#"><img src="https://img.shields.io/badge/Bun-000000?style=flat-square&logo=bun&logoColor=white" alt="Bun"/></a> <a href="#"><img src="https://img.shields.io/badge/esbuild-FFCF00?style=flat-square&logo=esbuild&logoColor=black" alt="esbuild"/></a> <a href="#"><img src="https://img.shields.io/badge/vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white" alt="vitest"/></a> |
| [SnapPipe](https://github.com/LOUST-PRO/SnapPipe) | Identity-based QUIC transport toolkit with Ed25519-signed tickets, server-side subject binding, and self-hosted relay scaffolding | QUIC connection-migration with subject-pinned ticket rotation keeps signed-session control planes alive across NAT rebinds; Rust core keeps the relay primitive auditable (no vendor crypto, no kernel bypass).<br/><br/><a href="#"><img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust"/></a> <a href="#"><img src="https://img.shields.io/badge/QUIC-0093D0?style=flat-square" alt="QUIC"/></a> <a href="#"><img src="https://img.shields.io/badge/Ed25519-2C3E50?style=flat-square" alt="Ed25519"/></a> |
| [NetBoozt](https://github.com/LOUST-PRO/NetBoozt_InternetUpgrade) | Linux network tuning: BBR-like TCP optimisations, intelligent failover, and DNS protection | 15–20% throughput lifts in test cases by squeezing Linux defaults (congestion control, queueing, DNS cache) instead of buying more bandwidth.<br/><br/><a href="#"><img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux"/></a> <a href="#"><img src="https://img.shields.io/badge/BBR-4285F4?style=flat-square" alt="BBR"/></a> <a href="#"><img src="https://img.shields.io/badge/TCP--BBR-2C3E50?style=flat-square" alt="TCP/BBR"/></a> <a href="#"><img src="https://img.shields.io/badge/DNS-1F2937?style=flat-square" alt="DNS"/></a> |
| [TaxonRouter](https://github.com/LOUST-PRO/TaxonRouter) | Dual-binary GitHub automation: MCP server + webhook auto-tagger. Pulls repository metadata through a JSON-RPC stdio surface and emits labels into GitHub Projects for triage | Backbone of the operator's own PR slicing, F80.9 batch classification, and the `lzt-pr-cadence-router` decision flow. Single-binary deploy, zero outbound dependencies, idempotent label reconciliation.<br/><br/><a href="#"><img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white" alt="Go"/></a> <a href="#"><img src="https://img.shields.io/badge/MCP-7C3AED?style=flat-square" alt="MCP"/></a> <a href="#"><img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub"/></a> |
| **SypremeMX + SYPREME Sybarite Premium Meats** (public repo + 6y7m, concurrent) | Public artefact: [LOUST-PRO/syprememx](https://github.com/LOUST-PRO/syprememx) — multi-tenant brand platform (CRM, ERP-style flows, bookings, e-commerce, Astro + Next.js + TypeScript + Prisma + GraphQL). Co-founder + CTO of the operating company SYPREME: campaign automation, CRM, atomic CFDI 4.0 invoicing, Stripe payments, multi-tenant e-commerce marketplace | 42 Prisma models and 600+ GraphQL endpoints back the same codebase that runs marketing, operations, and storefront surfaces — one source of truth for product and ops teams. Sub-2-minute lead-to-quote latency under exhibition pressure; LATAM Top 10/2023, Top 20/2024, Top 40/2025 at HEB Grill Master and 1st/2nd at Humo y Parrilla Fest 2024.<br/><br/><a href="#"><img src="https://img.shields.io/badge/Astro-BC52EE?style=flat-square&logo=astro&logoColor=white" alt="Astro"/></a> <a href="#"><img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"/></a> <a href="#"><img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/></a> <a href="#"><img src="https://img.shields.io/badge/Prisma-3982CE?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/></a> <a href="#"><img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/></a> <a href="#"><img src="https://img.shields.io/badge/Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white" alt="Stripe"/></a> <a href="#"><img src="https://img.shields.io/badge/CFDI_4.0-2C3E50?style=flat-square" alt="CFDI 4.0"/></a> |
| **Tren Maya smart-card credentials** (2025, 2mo contractor) | Visual identity, access hierarchy, and turnstile validation layout for regional mass-transit credentials (2025–2026 cycle) | Card usability had to hold up under high-density passenger traffic and multi-tier permission zoning — designed inside security-driven constraints, not around them. |
| [spec-snapshot-scraper](https://github.com/LOUST-PRO/spec-snapshot-scraper) | Documentation snapshots with content-addressed change-tracked corpora (BLAKE3 + git-tree-style manifest) | Stable corpora feed the Sovereign RAG (DSVH) index bootstrap and the Virtuoso 7.2.6 ingest pipeline — raw web search becomes obsolete once grounding is local and reproducible.<br/><br/><a href="#"><img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=FFD43B" alt="Python"/></a> <a href="#"><img src="https://img.shields.io/badge/BLAKE3-2C3E50?style=flat-square" alt="BLAKE3"/></a> <a href="#"><img src="https://img.shields.io/badge/Git_Tree-181717?style=flat-square&logo=git&logoColor=white" alt="Git tree"/></a> <a href="#"><img src="https://img.shields.io/badge/Virtuoso_7.2.6-2C3E50?style=flat-square" alt="Virtuoso 7.2.6"/></a> |
| **Upstream hardening** — Bottles · Waypaper · linux-wallpaperengine | Lifecycle, launch paths, and Wayland compositor contracts (`wlr-layer-shell`, `presentation-time`, `xdg-output`) across 3 upstreams | Each PR had to respect a different runtime model — GTK subprocess teardown ordering (Bottles Manager), frame-callback races on `wlr-layer-shell` (linux-wallpaperengine), and filter-matrix exposure across swww/awww/IPC backends (Waypaper).<br/><br/><a href="#"><img src="https://img.shields.io/badge/Wayland-000000?style=flat-square" alt="Wayland"/></a> <a href="#"><img src="https://img.shields.io/badge/wlr--layer--shell-7FE719?style=flat-square" alt="wlr-layer-shell"/></a> <a href="#"><img src="https://img.shields.io/badge/GTK-7FE719?style=flat-square" alt="GTK"/></a> <a href="#"><img src="https://img.shields.io/badge/presentation--time-2C3E50?style=flat-square" alt="presentation-time"/></a> |
| **Built-in signal pipeline** (drafting) | Recording + headless renderer stack for OSS demos, benchmarking, and self-hosted docs workflows | Re-uses the same render seam so screenshots and metrics stay reproducible across laptop and CI without a second toolchain.<br/><br/><a href="#"><img src="https://img.shields.io/badge/Headless_Renderer-2C3E50?style=flat-square" alt="Headless Renderer"/></a> <a href="#"><img src="https://img.shields.io/badge/Screenshot_Repro-8B5CF6?style=flat-square" alt="Screenshot Repro"/></a> |
| [deterministic-sovereign-rag](https://github.com/LOUST-PRO/deterministic-sovereign-rag) + [dsvh-verification-suite](https://github.com/LOUST-PRO/dsvh-verification-suite) | arXiv preprint LaTeX source + companion verification suite for the FNV-1a + L2 + cosine pipeline | Public companion to the Sovereign RAG paper: theorem proofs, reproducible build, IP-boundary contract. The verification suite asserts every empirical claim with a 25/25 concurrency stress test.<br/><br/><a href="#"><img src="https://img.shields.io/badge/LaTeX-008080?style=flat-square&logo=latex&logoColor=white" alt="LaTeX"/></a> <a href="#"><img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust"/></a> <a href="#"><img src="https://img.shields.io/badge/FNV--1a_64bit-2C3E50?style=flat-square" alt="FNV-1a 64-bit"/></a> <a href="#"><img src="https://img.shields.io/badge/Virtuoso_7.2.6-2C3E50?style=flat-square" alt="Virtuoso 7.2.6"/></a> |
| [ical-to-caldav](https://github.com/LOUST-PRO/ical-to-caldav) | iCal-to-CalDAV bridge daemon: converts public ICS subscription URLs into a CalDAV server for khal, DankCalendar, Evolution | Apache 2.0; small, focused Linux-runtime primitive that turns subscription calendars into native CalDAV sources.<br/><br/><a href="#"><img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust"/></a> <a href="#"><img src="https://img.shields.io/badge/CalDAV-4285F4?style=flat-square" alt="CalDAV"/></a> <a href="#"><img src="https://img.shields.io/badge/Apache_2.0-D22128?style=flat-square&logo=apache&logoColor=white" alt="Apache 2.0"/></a> |
| [LLMmempipe](https://github.com/LOUST-PRO/LLMmempipe) | Compile noisy LLM exports (ChatGPT, Claude, Gemini) into token-efficient JSONL + Markdown for Claude Code, Projects, and agent runtimes | Re-shapes vendor export shapes into a single canonical record stream — drops ~60% token bloat vs. raw paste.<br/><br/><a href="#"><img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/></a> <a href="#"><img src="https://img.shields.io/badge/JSONL-1F2937?style=flat-square" alt="JSONL"/></a> <a href="#"><img src="https://img.shields.io/badge/Claude-CC785C?style=flat-square&logo=anthropic&logoColor=white" alt="Claude"/></a> <a href="#"><img src="https://img.shields.io/badge/ChatGPT-74AA9C?style=flat-square&logo=openai&logoColor=white" alt="ChatGPT"/></a> |

<details>
<summary>Representative build signals from shipped systems</summary>

- 9 packages and 391 TypeScript files in Nexus Engine
- 42 Prisma models and 600+ GraphQL endpoints in larger platform work
- 50K embeddings queried in 188 ms in GPU-oriented retrieval
- 15-20% throughput improvements in NetBoozt test cases
- <2 minute lead-to-quote response latency in SYPREME conversion-attribution pipeline
- Atomic CFDI 4.0 invoicing pipeline (multi-tenant e-commerce + Stripe)
- Redis channel count reduced 59 → 18 via SCAN/COUNT migration over KEYS

</details>


<p align="center"><img src="/static/section-what-we-ship.svg" width="100%" alt="What we ship at loust.pro — Software company section banner"/></p>

The technology provider behind my work — multi-protocol transport, hardened Linux substrate, and B2B platforms that survive multi-year horizons. Public artefacts land in **Research & Publications** and **Investigations & Notes**; this section is the product surface I run day-to-day.

<p align="right"><sub><em>LOUST · Leverage Opportunities Unleashing Success and Transformation</em></sub></p>

<table>
  <tr>
    <td valign="top" width="50%">
      <strong>Enterprise CMS</strong><br/>
      <sub>Multi-tenant content + commerce + operations platform with isolated Postgres/Redis namespaces per tenant. Single codebase runs marketing, ERP-lite flows, bookings, and storefronts.</sub><br/>
      <sub>
        <a href="#"><img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"/></a>
        <a href="#"><img src="https://img.shields.io/badge/Astro-BC52EE?style=flat-square&logo=astro&logoColor=white" alt="Astro"/></a>
        <a href="#"><img src="https://img.shields.io/badge/Prisma-3982CE?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/></a>
        <a href="#"><img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/></a>
        <a href="#"><img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/></a>
        <a href="#"><img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis"/></a>
        <a href="#"><img src="https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white" alt="Cloudflare"/></a>
      </sub>
    </td>
    <td valign="top" width="50%">
      <strong>Automations</strong><br/>
      <sub>Rule + webhook engine for client operations. Connects Meta Ads, Google Ads, Stripe, MercadoPago, and CFDI 4.0 invoicing into auditable workflows with run history and replay.</sub><br/>
      <sub>
        <a href="#"><img src="https://img.shields.io/badge/Bun-000000?style=flat-square&logo=bun&logoColor=white" alt="Bun"/></a>
        <a href="#"><img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/></a>
        <a href="#"><img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/></a>
        <a href="#"><img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/></a>
        <a href="#"><img src="https://img.shields.io/badge/Redis_Streams-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis Streams"/></a>
      </sub>
    </td>
  </tr>
  <tr>
    <td valign="top" width="50%">
      <strong>CRM Hub</strong><br/>
      <sub>Pipeline + contact + closing surfaces for sales teams. Sub-2-minute lead-to-quote latency under exhibition pressure. Native multi-tenant isolation.</sub><br/>
      <sub>
        <a href="#"><img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"/></a>
        <a href="#"><img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/></a>
        <a href="#"><img src="https://img.shields.io/badge/Prisma-3982CE?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/></a>
        <a href="#"><img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/></a>
        <a href="#"><img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/></a>
      </sub>
    </td>
    <td valign="top" width="50%">
      <strong><a href="https://loust.pro/socialsphere">SocialSphere</a></strong><br/>
      <sub>PropTech + hospitality ERP. Multi-property booking, turnover calendars, and channel-manager hooks. CTO since Dec 2025.</sub><br/>
      <sub>
        <a href="#"><img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"/></a>
        <a href="#"><img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/></a>
        <a href="#"><img src="https://img.shields.io/badge/Prisma-3982CE?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/></a>
        <a href="#"><img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/></a>
        <a href="#"><img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/></a>
        <a href="#"><img src="https://img.shields.io/badge/Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white" alt="Stripe"/></a>
        <a href="#"><img src="https://img.shields.io/badge/Tauri-FFC131?style=flat-square&logo=tauri&logoColor=black" alt="Tauri"/></a>
      </sub>
    </td>
  </tr>
  <tr>
    <td valign="top" width="50%">
      <strong>Nexus Apps</strong><br/>
      <sub>Spec-driven generators and platform scaffolding. 9 packages and 391 TypeScript files keep multi-app ecosystems consistent from one source of truth instead of copy-paste.</sub><br/>
      <sub>
        <a href="#"><img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/></a>
        <a href="#"><img src="https://img.shields.io/badge/Bun-000000?style=flat-square&logo=bun&logoColor=white" alt="Bun"/></a>
        <a href="#"><img src="https://img.shields.io/badge/esbuild-FFCF00?style=flat-square&logo=esbuild&logoColor=black" alt="esbuild"/></a>
        <a href="#"><img src="https://img.shields.io/badge/tsc-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="tsc"/></a>
        <a href="#"><img src="https://img.shields.io/badge/vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white" alt="vitest"/></a>
      </sub>
    </td>
    <td valign="top" width="50%">
      <strong>Marketplace</strong><br/>
      <sub>Multi-vendor e-commerce with CFDI 4.0 invoicing, Stripe + MercadoPago splits, and a verified directory for sellers. Atomic invoicing pipeline keeps the trail auditable end-to-end.</sub><br/>
      <sub>
        <a href="#"><img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"/></a>
        <a href="#"><img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/></a>
        <a href="#"><img src="https://img.shields.io/badge/Prisma-3982CE?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/></a>
        <a href="#"><img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/></a>
        <a href="#"><img src="https://img.shields.io/badge/Stripe_Connect-635BFF?style=flat-square&logo=stripe&logoColor=white" alt="Stripe Connect"/></a>
        <a href="#"><img src="https://img.shields.io/badge/CFDI_4.0-2C3E50?style=flat-square" alt="CFDI 4.0"/></a>
      </sub>
    </td>
  </tr>
  <tr>
    <td valign="top" width="50%">
      <strong>AI Chatbot</strong><br/>
      <sub>Multi-tenant conversational surface for client ops. ReAct reasoning loop with provider-rotation across MiniMax M3, ChatGPT, Claude, DeepSeek, Gemini, Llama, and free-tier fallbacks; per-tenant retry budget keeps cost bounded. Routes to human handoff with full context, sessions in tenant-isolated Redis namespaces, exports to CRM Hub on close.</sub><br/>
      <sub>
        <a href="#"><img src="https://img.shields.io/badge/Bun-000000?style=flat-square&logo=bun&logoColor=white" alt="Bun"/></a>
        <a href="#"><img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/></a>
        <a href="#"><img src="https://img.shields.io/badge/MiniMax_M3-FF6B6B?style=flat-square" alt="MiniMax M3"/></a>
        <a href="#"><img src="https://img.shields.io/badge/Pollinations-FF6B6B?style=flat-square" alt="Pollinations"/></a>
        <a href="#"><img src="https://img.shields.io/badge/ChatGPT-74AA9C?style=flat-square&logo=openai&logoColor=white" alt="ChatGPT"/></a>
        <a href="#"><img src="https://img.shields.io/badge/Claude-CC785C?style=flat-square&logo=anthropic&logoColor=white" alt="Claude"/></a>
        <a href="#"><img src="https://img.shields.io/badge/DeepSeek-1A4F8C?style=flat-square" alt="DeepSeek"/></a>
        <a href="#"><img src="https://img.shields.io/badge/Gemini-4285F4?style=flat-square&logo=google&logoColor=white" alt="Gemini"/></a>
        <a href="#"><img src="https://img.shields.io/badge/Llama-0467DF?style=flat-square&logo=meta&logoColor=white" alt="Llama"/></a>
        <a href="#"><img src="https://img.shields.io/badge/ReAct-7C3AED?style=flat-square" alt="ReAct"/></a>
        <a href="#"><img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis"/></a>
        <a href="#"><img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/></a>
      </sub>
    </td>
    <td valign="top" width="50%">
      <strong>Public Research Notes</strong><br/>
      <sub>Long-form writeups on sovereign RAG, transport-layer hardening, kernel regressions, and infrastructure audits. Public-by-default where the abstraction boundary is legible.</sub><br/>
      <sub>
        <a href="#"><img src="https://img.shields.io/badge/Astro-BC52EE?style=flat-square&logo=astro&logoColor=white" alt="Astro"/></a>
        <a href="#"><img src="https://img.shields.io/badge/MDX-1B1F24?style=flat-square&logo=mdx&logoColor=white" alt="MDX"/></a>
        <a href="#"><img src="https://img.shields.io/badge/Gist-2C3E50?style=flat-square&logo=github&logoColor=white" alt="GitHub gist"/></a>
        <a href="#"><img src="https://img.shields.io/badge/ORCID-A6CE39?style=flat-square&logo=orcid&logoColor=white" alt="ORCID bridge"/></a>
      </sub>
    </td>
  </tr>
</table>


<p align="center"><img src="/static/section-research-and-publications.svg" width="100%" alt="Research and Publications — section banner"/></p>

Long-form research notes, paper drafts, and proof chains I maintain as part of day-to-day work. Each entry has a concrete artifact (gist, draft, or measurement) — no abstract ambitions.

### Deterministic Sovereign RAG via Signed-Hash Projection (paper draft, 2026)

A four-formula operator stack for reproducible retrieval on sovereign cloud corpora: FNV-1a 64-bit feature hashing into a fixed `D = 128` vector, `L2` spherical normalization, cosine reduced to a dot product on the unit hypersphere, and a pagination throughput window for upstream API rate-limit optimization. **Seven theorems** bound estimator unbiasedness, variance via Weinberger 2009, exponential collision concentration via the non-asymptotic Hanson–Wright inequality, `O(D)` storage/matching, scale invariance under `L2` normalization, the cosine/dot equivalence, and the `R_throughput` operational bound.

Validated empirically on a **4,458-document operator corpus** (MANIFESTs, memory entries, subagent specs, skill specs, hardening fragments) — indexed in 4.14 s on the operator's laptop with σ=0.18 s, 640 ns match latency (σ=85 ns) on the production virtualized substrate, and 0.78 top-5 recall. A 25/25 concurrency stress test on the production Rust implementation (`DSVH`) demonstrates stable operation under sustained workload. / _Cuatro fórmulas, siete teoremas. Retrieval soberano y determinista sobre infraestructura en la nube local._

<p align="center">
  <a href="https://gist.github.com/louzt/d1ce71c05460c2c32bf31342cd0c6a3f"><img src="https://img.shields.io/badge/Read_the_math_gist-English-7C3AED?style=for-the-badge&logo=github&logoColor=white" alt="Read the Sovereign RAG math gist (English)"/></a>
  &nbsp;
  <a href="https://gist.github.com/louzt/a75f9cf1a2f2edbd5af0e8d23526871d"><img src="https://img.shields.io/badge/Leer_las_matemáticas-Español-D97706?style=for-the-badge&logo=github&logoColor=white" alt="Leer las matemáticas del Sovereign RAG (Español)"/></a>
</p>

<sub>Stack: Rust (DSVH) + Go (APG) + Virtuoso 7.2.6 + FNV-1a 64-bit + L2 normalization. Open question: empirical head-to-head against dense embedders (BGE-M3, multilingual) — left for future work.</sub>

<p align="center"><img src="https://capsule-render.vercel.app/api?type=rect&color=0:0f172a,100:1e293b&height=2" width="100%"/></p>

### Zero-Prefill Keep-Alive Protocol (operator stack, 2026)

Cost-benefit gate for cache-warming probes against upstream GPU clusters. Three-step procedure: **monitor** the upstream's TTL state via a single `max_tokens=0` probe, **trigger** an asymmetric EMA update based on the boolean cache-hit response, **fire** the next probe only when the gate fires. The protocol is **800× cheaper** than a cold start at `K=1` and still 50× cheaper than an evict-and-compress cycle at `K=16`. The cadence is asymptotically optimal under the upstream's `5,000 req/hour` rate-limit constraint.

<sub>Stack: Go (APG) + Lamport happens-before ordering + Marzullo 1994 intersection bound + CLOCK_MONOTONIC. Documented in §5 (clock drift) + §8 (DET protocol) + §9 (zero-prefill) of the operator-stack paper draft.</sub>

<p align="center"><img src="https://capsule-render.vercel.app/api?type=rect&color=0:0f172a,100:1e293b&height=2" width="100%"/></p>

<p align="center"><img src="/static/section-investigations-and-notes.svg" width="100%" alt="Investigations and Notes — section banner"/></p>

Public research notes, snapshots, and audit logs from ongoing work. Updated as findings stabilize.

| Topic | Type | Notes |
| --- | --- | --- |
| [lzt-* gist collection](https://gist.github.com/louzt) | Mixed · 9+ gists | Bash hardening snippets, systemd unit definitions, MCP surface designs, certificate chains, transport proxy configs |
| [Resilient Transport vs Stateful DPI](https://gist.github.com/louzt/3991f144c7d67726045af3cefc60f42a) | Network engineering | 5-tier QUIC/Hysteria2/TLS/SSH fallback proxy; Happy Eyeballs racing in <200 ms; CA-pinned topology |
| [PipeWire handshake timeout (protocol-native)](https://github.com/louzt/pipewire/commit/2f747a7) | C / Linux core | 5s `spa timer` on `pw_protocol_native_connect_local_socket()`; prevents indefinite CLI hangs (`wpctl`/`pactl`) when daemon is alive but unresponsive. Published upstream on Freedesktop (PipeWire). |
| [Niri State Observability (Wayland typed-diagnostics)](https://gist.github.com/louzt/1c5230a2e9471faf9ce4243314361fa1) | Wayland compositor · Rust IPC | Pull-based typed diagnostics over Niri IPC; semantic asset labeling; per-output mutex; anchored 5 PRs upstream |
| [Waypaper image-filter PR #286](https://gist.github.com/louzt/761e227ad8cfe55b29e79cf861214a62) | Upstream OSS | Scaling algorithms exposed across swww/awww backends; HiDPI + pixel-art artifact resolution |
| [Zero-overhead observability](https://gist.github.com/louzt/b8349629b602a782ac98d0cbfd0df0c0) | Linux runtime | PSI over polling; inotify fork-bomb mitigation; Redis KEYS → SCAN/COUNT migration |
| [Chromium 148 CSP regression audit](https://gist.github.com/louzt/77f0804ca11bad6636f0ac67928bd384) | Web security | Accepted upstream under Opera GB-80414; CSP Level 3 + srcdoc sandbox collision isolation |
| [NVIDIA DKMS Kernel 7.0+ RFC](https://gist.github.com/louzt/1c85044d5090d19223c3f5edf426a19e) | Linux kernel · C | Forward-compat patch series for Kernel 7.0 API refactoring: VMA locking (`__is_vma_write_locked()` 2→1 args), DMA fence signal (`dma_fence_signal_locked()` int→void), `__vm_flags` removal in favor of `vm_flags_reset()`. 3-layer DKMS build-loop triage (`no-autoinstall` + `apt-mark hold` + unattended-upgrades blacklist). `NVreg_DynamicPowerManagement=0x02` modprobe rule for Optimus USB-C D3cold hotplug panics under hybrid GPUs. |

<p align="right"><sub><em>LOUST · Leverage Opportunities Unleashing Success and Transformation</em></sub></p>

> _Public gists are linked individually above as they ship. For private work-in-progress and operational forensics, see [LinkedIn](https://www.linkedin.com/in/davidmirelesll/?locale=es_ES) for the curated view._

<p align="center"><img src="https://capsule-render.vercel.app/api?type=rect&color=0:0f172a,100:1e293b&height=2" width="100%"/></p>

<!-- ============================================================ -->
<!-- FOOTER: animated squares grid + tagline (no operator name).  -->
<!-- loust.pro production path serves the same SVG; local mirror  -->
<!-- at .preview/static/profile-footer.svg until the upstream     -->
<!-- routing for /assets/* is fixed.                              -->
<!-- ============================================================ -->
<div align="center">
  <img alt="Animated footer tagline" src="https://loust.pro/assets/profile-footer.svg" width="100%" style="display:block;margin:0 auto"/>
</div>

<!-- ============================================================ -->
<!-- DOC META — keeps engineering provenance visible               -->
<!-- ============================================================ -->
<sub>
  <sup>Last validated: <a href="https://github.com/louzt/louzt/commits/main">commits</a> · <a href="https://gist.github.com/louzt">gists</a> · <a href="https://www.loust.pro/DavidMireles">portfolio</a></sup><br/>
  <sup>Source repo: <code>~/Proyectos/OSS/louzt-profile/</code> · <code>make doctor</code> for status</sup>
</sub>
