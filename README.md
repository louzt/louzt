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
  TaxonRouter → Tren Maya → spec-snapshot-scraper →
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
  <img alt="loust.pro — Let's work together" src="https://raw.githubusercontent.com/louzt/louzt/main/static/profile-header.svg" width="100%" />
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
    <!-- Row 1: contact channels — Schedule a meeting (CTA, NEW 2026-07-15) FIRST,
         then LinkedIn + GitLab + X.com + Matrix. Same shields.io ?style=flat-square
         as the other badges so they line up visually. -->
    <td align="left" valign="middle">
      <a href="https://calendar.app.google/XR7FkZXWVwfmZ57x6"><img src="https://img.shields.io/badge/Schedule_a_Meeting-34A853?style=flat-square&logo=googlecalendar&logoColor=white" alt="Schedule a Meeting (Google Calendar)"/></a>
      <a href="https://www.linkedin.com/in/davidmirelesll/?locale=es_ES"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
      <img src="https://img.shields.io/badge/GitLab-FC6D26?style=flat-square&logo=gitlab&logoColor=white" alt="GitLab"/>
      <img src="https://img.shields.io/badge/X-000000?style=flat-square&logo=x&logoColor=white" alt="X.com"/>
      <img src="https://img.shields.io/badge/Matrix-000000?style=flat-square&logo=matrix&logoColor=white" alt="Matrix"/>
    </td>
  </tr>
  <tr>
    <td align="left" valign="middle">
      <a href="https://komarev.com/ghpvc/?username=louzt&label=profile+views&color=1e293b&style=flat-square"><img src="https://komarev.com/ghpvc/?username=louzt&label=profile+views&color=1e293b&style=flat-square" alt="Profile Views"/></a>
      <a href="https://orcid.org/0009-0008-4374-2254"><img src="https://img.shields.io/badge/ORCID-0009--0008--4374--2254-A6CE39?style=flat-square&logo=orcid&logoColor=white" alt="ORCID iD 0009-0008-4374-2254"/></a>
      <a href="https://gist.github.com/louzt"><img src="https://img.shields.io/badge/Gists-181717?style=flat-square&logo=github&logoColor=white" alt="Gists"/></a>
      <a href="mailto:research@loust.pro"><img src="https://img.shields.io/badge/research%40loust.pro-7C3AED?style=flat-square&logo=protonmail&logoColor=white" alt="research@loust.pro"/></a>
      <a href="https://opensource.org/"><img src="https://img.shields.io/badge/OSI-Member-3DA639?style=flat-square&logo=opensourceinitiative&logoColor=white" alt="OSI Member"/></a>
      <a href="https://github.com/django-commons"><img src="https://img.shields.io/badge/Django_Commons-0C4B33?style=flat-square&logo=django&logoColor=white" alt="Django Commons Member"/></a>
      <a href="https://kernel.org/"><img src="https://img.shields.io/badge/Linux_Kernel-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux Kernel"/></a>
      <a href="https://crates.io/users/louzt"><img src="https://img.shields.io/badge/crates.io-000000?style=flat-square&logo=rust&logoColor=e43717" alt="crates.io packages"/></a>
      <img src="https://img.shields.io/badge/%2b_many_more-1E293B?style=flat-square" alt="+ many more communities"/>
    </td>
  </tr>
  <tr>
    <!-- Row 3: Core Programming Languages & Core Engine Technologies -->
    <td align="left" valign="middle">
      <img src="https://img.shields.io/badge/rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust"/>
      <img src="https://img.shields.io/badge/go-00add8?style=flat-square&logo=go&logoColor=white" alt="Go"/>
      <img src="https://img.shields.io/badge/typescript-3178c6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
      <img src="https://img.shields.io/badge/python-3776ab?style=flat-square&logo=python&logoColor=ffd43b" alt="Python"/>
      <img src="https://img.shields.io/badge/c-A8B9CC?style=flat-square&logo=c&logoColor=white" alt="C"/>
      <img src="https://img.shields.io/badge/c++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white" alt="C++"/>
      <img src="https://img.shields.io/badge/zig-F7A41D?style=flat-square&logo=zig&logoColor=white" alt="Zig"/>
      <img src="https://img.shields.io/badge/perl-0298c3?style=flat-square&logo=perl&logoColor=white" alt="Perl"/>
      <img src="https://img.shields.io/badge/Lua-2C2D72?style=flat-square&logo=lua&logoColor=white" alt="Lua"/>
      <img src="https://img.shields.io/badge/Ruby-CC342D?style=flat-square&logo=ruby&logoColor=white" alt="Ruby"/>
      <img src="https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white" alt="PHP"/>
      <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white" alt="Node.js"/>
      <img src="https://img.shields.io/badge/%7C-1e293b?style=flat-square" alt="|"/>
      <img src="https://img.shields.io/badge/Vulkan-AC162C?style=flat-square&logo=vulkan&logoColor=white" alt="Vulkan"/>
      <img src="https://img.shields.io/badge/WebGL-990000?style=flat-square&logo=webgl&logoColor=white" alt="WebGL"/>
      <img src="https://img.shields.io/badge/Three.js-000000?style=flat-square&logo=threedotjs&logoColor=white" alt="Three.js"/>
      <img src="https://img.shields.io/badge/Babylon.js_8-000000?style=flat-square&logo=babylondotjs&logoColor=white" alt="Babylon.js 8"/>
      <img src="https://img.shields.io/badge/WebRTC-333333?style=flat-square&logo=webrtc&logoColor=white" alt="WebRTC"/>
      <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"/>
      <img src="https://img.shields.io/badge/Astro-BC52EE?style=flat-square&logo=astro&logoColor=white" alt="Astro"/>
      <img src="https://img.shields.io/badge/Svelte-FF3E00?style=flat-square&logo=svelte&logoColor=white" alt="Svelte"/>
      <img src="https://img.shields.io/badge/flutter-02569B?style=flat-square&logo=flutter&logoColor=white" alt="Flutter"/>
      <img src="https://img.shields.io/badge/%7C-1e293b?style=flat-square" alt="|"/>
      <img src="https://img.shields.io/badge/postgresql-4169e1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
      <img src="https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white" alt="SQLite"/>
      <img src="https://img.shields.io/badge/redis-dc382d?style=flat-square&logo=redis&logoColor=white" alt="Redis"/>
      <img src="https://img.shields.io/badge/graphql-e10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/>
      <img src="https://img.shields.io/badge/Prisma-3982CE?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/>
      <img src="https://img.shields.io/badge/%7C-1e293b?style=flat-square" alt="|"/>
      <img src="https://img.shields.io/badge/k3s-ffc61c?style=flat-square&logo=kubernetes&logoColor=black" alt="k3s"/>
      <img src="https://img.shields.io/badge/docker-2496ed?style=flat-square&logo=docker&logoColor=white" alt="Docker"/>
      <img src="https://img.shields.io/badge/Always_curious_to_debug_in_another_tech_stack-8b5cf6?style=flat-square&logoColor=white" alt="Always curious to debug in another tech stack"/>
    </td>
  </tr>
  <tr>
    <!-- Row 4: MarTech & AdTech Infrastructure -->
    <td align="left" valign="middle">
      <img src="https://img.shields.io/badge/MarTech_%26_AdTech-FF5722?style=flat-square&logo=googleanalytics&logoColor=white" alt="MarTech & AdTech"/>
      <img src="https://img.shields.io/badge/Google_Ads_API-4285F4?style=flat-square&logo=googleads&logoColor=white" alt="Google Ads API"/>
      <img src="https://img.shields.io/badge/Meta_CAPI-1877F2?style=flat-square&logo=meta&logoColor=white" alt="Meta Conversions API"/>
      <img src="https://img.shields.io/badge/TikTok_Ads_API-000000?style=flat-square&logo=tiktok&logoColor=white" alt="TikTok Ads API"/>
      <img src="https://img.shields.io/badge/X_Ads_API-000000?style=flat-square&logo=x&logoColor=white" alt="X Ads API"/>
      <img src="https://img.shields.io/badge/Stripe_API-635BFF?style=flat-square&logo=stripe&logoColor=white" alt="Stripe API"/>
      <img src="https://img.shields.io/badge/PayPal_API-003087?style=flat-square&logo=paypal&logoColor=white" alt="PayPal API"/>
      <img src="https://img.shields.io/badge/MercadoPago_API-009EE3?style=flat-square&logo=mercadopago&logoColor=white" alt="MercadoPago API"/>
      <img src="https://img.shields.io/badge/Crypto_Payments_(BTC%2fSOL)-121D33?style=flat-square&logo=solana&logoColor=white" alt="Crypto Payments"/>
      <img src="https://img.shields.io/badge/Custom_REST_%26_GraphQL_APIs-00A1E0?style=flat-square" alt="Custom REST & GraphQL APIs"/>
      <img src="https://img.shields.io/badge/Server--Side_Tracking-00A1E0?style=flat-square&logo=salesforce&logoColor=white" alt="Server-Side Tracking"/>
      <img src="https://img.shields.io/badge/CRM-00A1E0?style=flat-square&logo=salesforce&logoColor=white" alt="CRM"/>
      <img src="https://img.shields.io/badge/ERP-714B67?style=flat-square" alt="ERP"/>
      <img src="https://img.shields.io/badge/SaaS--to--SaaS-2C3E50?style=flat-square" alt="SaaS-to-SaaS"/>
    </td>
  </tr>
  <tr>
    <!-- Row 5: Web3 & Decentralized Infrastructure -->
    <td align="left" valign="middle">
      <img src="https://img.shields.io/badge/Blockchain_%26_Web3-121D33?style=flat-square&logo=blockchaindotcom&logoColor=white" alt="Blockchain & Web3"/>
      <img src="https://img.shields.io/badge/MCP_%26_Agent_Protocols-000000?style=flat-square&logo=github&logoColor=white" alt="MCP & Agent Protocols"/>
      <img src="https://img.shields.io/badge/Agentic_Workflows-7c3aed?style=flat-square" alt="Agentic Workflows"/>
      <img src="https://img.shields.io/badge/RBAC_%26_Multi--Tenant_Isolation-0f172a?style=flat-square" alt="RBAC & Multi-Tenant Isolation"/>
      <img src="https://img.shields.io/badge/Ed25519_Identity-2C3E50?style=flat-square" alt="Ed25519 Identity"/>
      <img src="https://img.shields.io/badge/Virtuoso_Triples_%2f_SPARQL-2C3E50?style=flat-square" alt="Virtuoso Triples / SPARQL"/>
      <img src="https://img.shields.io/badge/Knowledge_Graphs-0f172a?style=flat-square" alt="Knowledge Graphs"/>
      <img src="https://img.shields.io/badge/Local--First_%26_CRDT-064E3B?style=flat-square" alt="Local-First & CRDT"/>
    </td>
  </tr>
  <tr>
    <!-- Row 6: Research Specializations, Engineering Categories & Community Call -->
    <td align="left" valign="middle">
      <a href="https://gist.github.com/louzt/3991f144c7d67726045af3cefc60f42a"><img src="https://img.shields.io/badge/Deterministic_Harnesses-8b5cf6?style=flat-square" alt="Deterministic Harnesses"/></a>
      <a href="https://gist.github.com/louzt/d1ce71c05460c2c32bf31342cd0c6a3f"><img src="https://img.shields.io/badge/Sovereign_RAG-7c3aed?style=flat-square" alt="Sovereign RAG"/></a>
      <img src="https://img.shields.io/badge/Spec--Driven_Engineering-0284c7?style=flat-square" alt="Spec-Driven Engineering"/>
      <img src="https://img.shields.io/badge/Zero--Egress_Security-1F2937?style=flat-square" alt="Zero-Egress Security"/>
      <img src="https://img.shields.io/badge/Kernel_%26_Runtime_Hardening-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Kernel & Runtime Hardening"/>
      <img src="https://img.shields.io/badge/CLA_%26_FOSS_Governance-004D40?style=flat-square" alt="CLA & FOSS Governance"/>
      <a href="mailto:partnership@loust.pro"><img src="https://img.shields.io/badge/partnership%40loust.pro-0A66C2?style=flat-square&logo=minutemailer&logoColor=white" alt="partnership@loust.pro"/></a>
      <a href="mailto:partnership@loust.pro?subject=FOSS%20Community%20Collaboration"><img src="https://img.shields.io/badge/Open_to_contribute_to_FOSS%2FOSS_Communities-34A853?style=flat-square&logo=opensourceinitiative&logoColor=white" alt="Open to contribute to FOSS/OSS Communities"/></a>
      <a href="mailto:partnership@loust.pro?subject=Peer%20Collaboration"><img src="https://img.shields.io/badge/Looking_for_peers_%26_exciting_projects-0284c7?style=flat-square" alt="Looking for peers & exciting projects"/></a>
    </td>
  </tr>
  <tr>
    <!-- Row 7: Roles, Infrastructure & Mindset -->
    <td align="left" valign="middle">
      <img src="https://img.shields.io/badge/Systems_Architect-0f172a?style=flat-square" alt="Systems Architect"/>
      <img src="https://img.shields.io/badge/DevOps_%26_SRE-2563eb?style=flat-square&logo=kubernetes&logoColor=white" alt="DevOps & SRE"/>
      <img src="https://img.shields.io/badge/Platform_Engineering-0891b2?style=flat-square" alt="Platform Engineering"/>
      <img src="https://img.shields.io/badge/Security_Researcher-eb0029?style=flat-square&logo=hackerone&logoColor=white" alt="Security Researcher"/>
      <img src="https://img.shields.io/badge/First--Principles_Engineering-6366f1?style=flat-square" alt="First-Principles Engineering"/>
      <img src="https://img.shields.io/badge/Zero--Trust_Infrastructure-1e293b?style=flat-square" alt="Zero-Trust Infrastructure"/>
      <img src="https://img.shields.io/badge/Kernel_%26_Systems_Research-0f172a?style=flat-square&logo=linux&logoColor=white" alt="Kernel & Systems Research"/>
      <img src="https://img.shields.io/badge/Lifelong_Student-7c3aed?style=flat-square" alt="Lifelong Student"/>
    </td>
  </tr>
</table>

<div align="center">
  <img alt="Systems Architecture &amp; Operational Posture — section banner" src="https://raw.githubusercontent.com/louzt/louzt/main/static/section-tactical-posture.svg" width="100%" />
</div>

I maintain a prophylactic, respectful, and deterministic engineering posture — continuously calibrating reasoning, transport layers, and operational workflows against empirical evidence. I design and ship production systems where the boundary between application delivery and systems engineering has to hold. Most of my work is research-flavored engineering: the abstractions are reusable, the proofs are formal where they need to be, and the operational evidence is auditable end-to-end.

<blockquote style="border-left: 3px solid #10b981; background: #0f172a; padding: 12px 16px; margin: 16px 0; border-radius: 0 6px 6px 0; color: #e2e8f0;">
  <b>Confucius</b> <i>(Philosopher)</i>: <i>"Choose a job you love, and you will never have to work a day in your life."</i>
</blockquote>

<blockquote style="border-left: 3px solid #38bdf8; background: #0f172a; padding: 12px 16px; margin: 16px 0; border-radius: 0 6px 6px 0; color: #e2e8f0;">
  <b>Rob Pike</b> <i>(Co-creator of Go &amp; UTF-8)</i>: <i>"Data dominates. If you've chosen the right data structures and organized things well, the algorithms will almost always be self-evident."</i>
</blockquote>

<blockquote style="border-left: 3px solid #8b5cf6; background: #0f172a; padding: 12px 16px; margin: 16px 0; border-radius: 0 6px 6px 0; color: #e2e8f0;">
  <b>Rich Hickey</b> <i>(Creator of Clojure &amp; Datomic)</i>: <i>"Simplicity is a prerequisite for reliability."</i>
</blockquote>

<blockquote style="border-left: 3px solid #ec4899; background: #0f172a; padding: 12px 16px; margin: 16px 0; border-radius: 0 6px 6px 0; color: #e2e8f0;">
  <b>Fred Brooks</b> <i>(Turing Award Winner &amp; Author of The Mythical Man-Month)</i>: <i>"Conceptual integrity is the most important consideration in system design. Good judgment comes from experience, and experience comes from bad judgment."</i>
</blockquote>

<blockquote style="border-left: 3px solid #f59e0b; background: #0f172a; padding: 12px 16px; margin: 16px 0; border-radius: 0 6px 6px 0; color: #e2e8f0;">
  <b>Werner Vogels</b> <i>(CTO of Amazon)</i>: <i>"Everything fails, all the time. Design for recovery, not perfection."</i>
</blockquote>

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/section-how-i-work.svg" width="100%" alt="How I work — section banner"/></p>

- I approach systems engineering much like a craftsman in a workshop—studying product architecture, transport bottlenecks, and telemetry end-to-end before touching code or proposing refactors.
- I maintain a devoted, methodical patience for extracting deterministic telemetry down to the last data point—building custom test harnesses, watchdog reapers, and verification suites whenever existing tooling leaves room for ambiguity.
- I digest and compile raw upstream artifacts—issues, PRs, historical commit trees, and vendor API specifications—into hyper-efficient knowledge graphs for zero-overhead token budgeting, context compaction, and multi-branch differential analysis.
- I design self-healing, self-improving systems built around explicit opportunity-cost evaluation—recognizing early on that human vision has blind spots, so the system itself must auto-calibrate, prune stale specs, and enforce invariants.
- I execute problem-tailored SAST triage and OSINT synthesis across publicly documented vulnerabilities and technical papers, synthesizing empirical findings into reproducible test suites before validating hypotheses against candidate implementations.
- I balance rapid innovation cycles with long-term leverage—structuring technical breakthroughs into quarterly roadmap milestones, reusable pattern libraries, and durable architecture decisions that survive maintainer churn.
- I respect and adopt maintainer vision when contributing to external codebases—framing proposals through clear architectural dimensions (orthogonal, horizontal, or vertical) and providing minimal-scope patches that minimize reviewer friction.
- I have operated at the intersection of systems engineering and AI agents long before commercial AI IDEs existed—building CLI-first terminal agent loops, custom MCP bridges, and publishing reproducible **Investigaciones** (detailed in the research section below).
- I harden network, IPC, and service layers first, ensuring the underlying substrate is secure and resilient before asking application code to carry production workloads.
- I trace edge cases directly back to runtime behavior until the underlying contract is explicit, fixing structural boundaries rather than applying superficial patches.
- I run targeted triage, SAST, and benchmarks across C, Rust, Go, Bun, Zig, and Python in lab setups, evaluating real-world trade-offs in memory, latency, and state to build a practical pattern library.
- I integrate new capabilities through clean, isolated adapters that respect working production logic, allowing established platforms to scale safely without breaking core business flows.
- I address AI scaling inefficiencies at the root—optimizing local RAG substrates, execution loops, and context compaction from the bare-metal up before paying for raw model overhead.
- I maintain a self-reliant, transparent posture: sensitive infrastructure redacted, pull requests tightly scoped, and code reviews handled as a constructive, two-way technical dialogue.

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/section-working-with-me.svg" width="100%" alt="Working with me — section banner"/></p>

### Working with me

- **Feedback and learning** — if you see me somewhere learning to work better inside a software team, I'm interested. Senior reviewers, engineering leads, or teammates who have a specific technical observation — a code review thread, a shared codebase, a process friction — are welcome to reach out. I consider your opinion useful and treat feedback as a two-way loop, not a one-way deliverable; the best learning posture is to keep the audit trail legible on both sides.
- **HackerOne disclosure track** — vulnerability reports and coordinated disclosure for infrastructure under our scope route through [security@loust.pro](mailto:security@loust.pro). Triaged within 72 hours; reproducible PoCs and a minimum-scope patch suggestion move reports to the front of the queue. Out-of-scope signals (DMS, PipeWire hardening) and known-busy triage windows are documented so reporters don't spin.
- **Research collaborations** — formal proofs, deterministic systems, transport-layer hardening, sovereign AI infra. Best fit: university labs, independent PhD-track researchers, and private R&D teams working in applied-probability / IR / agent frameworks. Reach out at [research@loust.pro](mailto:research@loust.pro) with a 1-paragraph abstract and a concrete artifact (gist, paper draft, benchmark).
- **OSS upstream hardening** — if you maintain an OSS project where the runtime model is well-bounded (lifecycle contracts, allocator hot paths, compositor or daemon boundaries), I'd like to talk. I take scoped PRs against the runtime boundary; bring a reproducer + a minimum-scope patch, not a slide deck. Open invite — long-running contributor or co-maintainer track.
- **Communities and chat** — IRC, Discord, Matrix, and adjacent chat-based communities are my preferred channels over mainstream social networks. If you're active in OSS communities on those surfaces (Libera.Chat / OFTC, Matrix rooms, Discord OSS servers, project-specific channels), feel free to ping me. I read more than I write, but I value signal over volume.
- **B2B platform work / partnerships** — long-horizon engagements only. We build the substrate, the observability, and the audit trail before declaring anything shipped — capacity for staged rollouts is the constraint, not the calendar. Reach out at [partnership@loust.pro](mailto:partnership@loust.pro).
- **Reference policy** — I write public references for shipped work with measurable outcomes. Send the PR / artifact link and a 1-line outcome metric; I respond within a week.

### 🛠️ Services & Engineering Solutions Matrix

High-rigor technical services and consulting backed by 850K+ lines of production code across 50+ delivered systems:

| Service Category | Engineering Capabilities & Tech Stack | Value Proposition & Deliverable |
| :--- | :--- | :--- |
| **Systems & Kernel Hardening** | POSIX `prctl`, C/C++, Rust, IPC, Linux daemons, container isolation, eBPF / `tcp_diag` | Eliminates memory/CPU leaks, zombie process loops, and daemon IPC hangs under heavy production loads. |
| **Custom REST & GraphQL APIs** | TypeScript, Next.js, Apollo Server v4, Prisma, PostgreSQL, Redis Lua, APQ at scale | Sub-15ms p95 query latency, multi-tenant RBAC namespace isolation, and zero-downtime schema evolution. |
| **MarTech & AdTech Infrastructure** | Google Ads API, Meta CAPI, TikTok Ads API, X Ads API, Server-Side Tracking, CRM/ERP | Server-side conversion attribution, zero data-loss tracking, and CFDI 4.0 automated billing integrations. |
| **SaaS & Payment Gateway Integrations** | Stripe, PayPal, MercadoPago, Crypto (BTC/Solana), Webhooks, Microservices | Multi-currency, multi-gateway resilient billing pipelines with automated reconciliation and zero retry amplification. |
| **Sovereign AI & Agent Control Planes** | Model Context Protocol (MCP), Sovereign RAG, Local Vector Substrates, Zero-Egress Agents | Local-first agentic workflows with bounded latency, VRAM budgeting, and continuous contract verification. |
| **Security Audits & Zero-Trust Architecture** | SAST, CSP Level 3, Ed25519 identity transport, CA-pinning, HackerOne disclosure track | Hardened network transport, zero-egress sandboxing, and auditable vulnerability mitigation. |

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/section-selected-work.svg" width="100%" alt="Selected Work — section banner"/></p>

Production systems that have shipped to real users, merged into upstreams, or run as long-lived client platforms. Public artefacts link out; private platforms are referenced by name only — the boundary between public proof and client-confidential work is deliberate, reviewable, and unchanged across engagements.

**How we stay current.** Release notes get read before installs. Spec changelogs (MCP, Claude, OpenAI, Gemini, every model API we depend on) get watched continuously. Triage goes multi-layer-deep before anything ships — the goal is to understand the *vision*, *scope*, and *future steps* of anything we depend on, so the operator inherits a solid system instead of a house of cards.

| Focus | Operational Impact | Project |
| --- | --- | --- |
| Distributed data plane in Rust + Go: routing, cache control, and a hardened tool-call pipeline for autonomous agents. Backed by the [Sovereign RAG math gist](https://gist.github.com/louzt/d1ce71c05460c2c32bf31342cd0c6a3f) (English) / [Las Matemáticas del Sovereign RAG](https://gist.github.com/louzt/a75f9cf1a2f2edbd5af0e8d23526871d) (Español)<br/><br/><img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust"/> <img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white" alt="Go"/> <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/> <img src="https://img.shields.io/badge/Bayesian_Stream_Guard-8B5CF6?style=flat-square" alt="Bayesian Stream Guard"/> <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis"/> | Decouples agent control planes from provider volatility; 3-way semantic sync + Bayesian Stream Guard with <0.5s hallucination kill-switch. | **LZT SRE Harness** (private) |
| Closed-core agent runtime + secure gateway: a pruned Rust CLI (`h3ph`) talks to a multi-tenant k3s sidecar handling ephemeral SAST scans, BYOK inference, and zero-retention report delivery. Three access tiers (Researcher / Private Beta / Commercial) gated on signed digital contract<br/><br/><img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust"/> <img src="https://img.shields.io/badge/k3s-FFC61C?style=flat-square&logo=kubernetes&logoColor=black" alt="k3s"/> <img src="https://img.shields.io/badge/BYOK-7C3AED?style=flat-square" alt="BYOK"/> <img src="https://img.shields.io/badge/AGPLv3-3D4451?style=flat-square&logo=gnu&logoColor=white" alt="AGPLv3"/> <img src="https://img.shields.io/badge/Private_Repo-1F2937?style=flat-square" alt="Private Repo"/> | Operates with locked egress and isolated reasoning — client nodes never see the operator's reasoning loop, system prompts, or tool contracts. Adaptive VRAM/cache budgeting keeps long-running multi-agent fleets predictable across deep multi-turn runs. | **h3ph43st** (private repo, `h3ph` CLI · AGPLv3 · upcoming) |
| Multi-protocol transport optimized for autonomous agent control planes and other latency-sensitive use cases: Go + Rust proxy racing QUIC / Hysteria2 / direct TLS / SSH, promoting the first-healthy stream under 200ms. Public artefacts: [5-layer SSH fallback chain (Cadena de fallback SSH de 5 capas)](https://gist.github.com/louzt/e318d7e0ae1fd676d124311c80585f74) + [multi-protocol reverse proxy case study (SSH Reverse Proxy & 5-Tier Evasion Chain v1.0)](https://gist.github.com/louzt/3991f144c7d67726045af3cefc60f42a)<br/><br/><img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white" alt="Go"/> <img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust"/> <img src="https://img.shields.io/badge/QUIC-0093D0?style=flat-square" alt="QUIC"/> <img src="https://img.shields.io/badge/Multi--Protocol-7C3AED?style=flat-square" alt="Multi-Protocol"/> <img src="https://img.shields.io/badge/TLS-2C3E50?style=flat-square" alt="TLS"/> <img src="https://img.shields.io/badge/SSH-000000?style=flat-square" alt="SSH"/> <img src="https://img.shields.io/badge/Agent_Transport-1F2937?style=flat-square" alt="Agent Transport"/> | Sub-200ms first-healthy-stream promotion keeps agent tool-call round-trips within budget even when single-transport assumptions fail; CA-pinning blocks MITM and POSIX-atomic writes eliminate storage state drift. Designed for environments where transport-layer variability is the norm (mobile, captive portals, restrictive NATs, cross-region agent fleets) — not for any adversarial objective. | **Multi-protocol transport for agents** (private) |
| 3D fighting game engine informed by competitive-gaming netcode research: GGPO-style rollback (snapshot/restore + speculative execution) calibrated by Ishioka's repeat-last prediction (>70% accurate at 1-3 frame windows) for a 30-frame (~500 ms) rollback window with ~12-frame headroom over average VPN/high-latency play; Valve Source Engine patterns for interpolation buffer tuning + binary input codec; Claypool's prediction taxonomy (Prediction + TimeWarp + Interpolation); Age-of-Empires-style determinism discipline on the simulation path so both clients converge on identical state. Babylon.js 8 (WebGPU preferred, WebGL fallback), Bun + Vite + TypeScript strict, headless rollback simulation harness under synthetic lag/loss profiles<br/><br/><img src="https://img.shields.io/badge/Bun-000000?style=flat-square&logo=bun&logoColor=white" alt="Bun"/> <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/> <img src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white" alt="Vite"/> <img src="https://img.shields.io/badge/Babylon.js_8-000000?style=flat-square&logo=babylondotjs&logoColor=white" alt="Babylon.js 8"/> <img src="https://img.shields.io/badge/WebSocket-2C3E50?style=flat-square" alt="WebSocket"/> <img src="https://img.shields.io/badge/WebRTC-333333?style=flat-square&logo=webrtc&logoColor=white" alt="WebRTC"/> <img src="https://img.shields.io/badge/TURN%2FCOTURN-7C3AED?style=flat-square" alt="TURN/COTURN"/> <img src="https://img.shields.io/badge/GGPO--Rollback-FF6B35?style=flat-square" alt="GGPO Rollback"/> | Real-time matches stay playable on restrictive NATs and DPI: WebSocket (TCP, reliable/ordered) carries signaling and match lifecycle while WebRTC DataChannel (UDP, unordered) carries the binary input path; WebRTC upgrade happens in the background without interrupting gameplay, falls back to WebSocket transparently on failure. Diagnostic HUD exposes real-time ping, jitter, and rollback depth (toggleable in-match). | **h4kken** (private, deployed at h4kken.loust.pro) |
| Multi-tenant B2B engine: tenant-isolated Postgres/Redis namespaces, Apollo Persisted Queries (APQ) at the edge, Firefox Gecko + MDN-powered client-side translation fallback chain, cross-project indexed search across docs/frontends/dashboards, and spec-driven custom plugin development for ambitious needs — public case study on the 135k-line GraphQL schema deployment: [English gist](https://gist.github.com/louzt/64715cb9c6ec6ffdd98c5712b8fb7bac) / [caso de estudio en Español](https://gist.github.com/louzt/0c91771bf6370f0eb47e905934ab47e8)<br/><br/><img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/> <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis"/> <img src="https://img.shields.io/badge/Prisma-3982CE?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/> <img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/> <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"/> <img src="https://img.shields.io/badge/Astro-BC52EE?style=flat-square&logo=astro&logoColor=white" alt="Astro"/> <img src="https://img.shields.io/badge/Apollo_APQ-311C87?style=flat-square&logo=apollographql&logoColor=white" alt="Apollo APQ"/> | 7+ years operational stability without substrate resets; client-side translation chain (modular browser LLM → locale dictionaries → self-hosted LibreTranslate → Google Translate free tier → paid on-demand) keeps server-side token spend and DDoS amplification surface at zero. Locale autodetection + user-preference selectors. Data analysis from casual dashboards to business-specific algorithms. Custom plugins + spec-driven innovation posture. | **LOUST multi-tenant platform** (current, 7y6m) |
| Spec-driven code generators and platform scaffolding for multi-app TypeScript monorepos<br/><br/><img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/> <img src="https://img.shields.io/badge/Bun-000000?style=flat-square&logo=bun&logoColor=white" alt="Bun"/> <img src="https://img.shields.io/badge/esbuild-FFCF00?style=flat-square&logo=esbuild&logoColor=black" alt="esbuild"/> <img src="https://img.shields.io/badge/vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white" alt="Vitest"/> | Single source of truth across 9 packages and 391 TypeScript files, eliminating boilerplate duplication and type drift. | **Nexus Engine** (private) |
| Identity-anchored transport toolkit that solves the SSH/QUIC head-of-line blocking problem: when strict NATs, firewalls, captive campus networks, or carrier-grade mobile networks force transport to degrade toward TCP-ish behavior, rollback-sensitive real-time sessions become fragile. SnapPipe binds sessions to a cryptographic identity (Ed25519 public key) instead of an `ip:port` tuple — rebind/reconnect stays cheap, signed tickets gate the peer handshake before any data flows, and a self-hosted relay scaffolds the bootstrap path. v0.2.1 surfaces identity-gated handshake (`NonNullIssuer` rejects an empty trust store as default-allow), bounded `NonceStore` with TTL for replay protection, per-NodeId rate limiting, ALPN source-of-truth, sub-second mtime, and lock-free v0.3.0 trigger metrics on NonceStore/RateLimiter<br/><br/><img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust"/> <img src="https://img.shields.io/badge/QUIC-0093D0?style=flat-square" alt="QUIC"/> <img src="https://img.shields.io/badge/Ed25519-2C3E50?style=flat-square" alt="Ed25519"/> <img src="https://img.shields.io/badge/Identity--Anchored-7C3AED?style=flat-square" alt="Identity-Anchored"/> <img src="https://img.shields.io/badge/Self--Hosted-3D4451?style=flat-square" alt="Self-Hosted"/> | Library design + QUIC implementation choices that keep both client and server sides auditable: handshake decisions land before any peer sees an unauthenticated frame; the trust store is bounded and inspectable; rate-limit decisions trace to a NodeId, not to a transient socket. CI hardened with SHA-pinned actions, `persist-credentials: false`, and `cargo test --locked`. | [SnapPipe](https://github.com/LOUST-PRO/SnapPipe) |
| Cross-platform internet upgrade toolkit with three deployment shapes: Tauri v3.1 desktop GUI (Rust + SvelteKit, ~8 MB, glassmorphism UI, Windows production), Python v2.2 CLI legacy surface (CustomTkinter + headless CLI, ~25 MB Nuitka bundle), and headless systemd/Windows Service daemons. Windows side implements Linux BBR-equivalent TCP optimizations — HyStart++ slow-start, PRR loss recovery, ECN negotiation, TCP Fast Open, TCP Pacing, RSS/RSC receive-side coalescing. Linux headless binary delivers the same DNS Auto-Failover (11 servers across 6 tiers: Speed, Security, Privacy) as a systemd user service without GUI overhead. 4-Phase Diagnostics walks Adapter → Router → ISP → DNS with parallel 4-worker health checks (~3s cycle vs ~30s sequential) and live graphs + Event Log integration<br/><br/><img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust"/> <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=FFD43B" alt="Python"/> <img src="https://img.shields.io/badge/Tauri_v3.1-FFC131?style=flat-square&logo=tauri&logoColor=black" alt="Tauri v3.1"/> <img src="https://img.shields.io/badge/Windows-0078D6?style=flat-square&logo=windows&logoColor=white" alt="Windows"/> <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux"/> <img src="https://img.shields.io/badge/BBR-4285F4?style=flat-square" alt="BBR"/> <img src="https://img.shields.io/badge/DNS-1F2937?style=flat-square" alt="DNS"/> <img src="https://img.shields.io/badge/Apache_2.0-D22128?style=flat-square&logo=apache&logoColor=white" alt="Apache 2.0"/> | Real-world throughput gains of +15-20% on Windows via Linux kernel-default techniques (queueing discipline, congestion control, socket buffers) without paying for extra bandwidth; DNS failover across Speed/Security/Privacy tiers survives ISP DNS outages and captive-portal interference; three runtime modes (Tauri GUI, Python CLI, headless systemd/Service) cover desktop power users, remote shell operators, and unattended infrastructure with the same config grammar. Apache-2.0 (deliberate single-license since 2026-06-25). | [NetBoozt](https://github.com/LOUST-PRO/NetBoozt_InternetUpgrade) |
| Dual-binary GitHub automation: MCP server + webhook auto-tagger. Pulls metadata via JSON-RPC stdio surface and manages GitHub Projects triage<br/><br/><img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white" alt="Go"/> <img src="https://img.shields.io/badge/MCP-7C3AED?style=flat-square" alt="MCP"/> <img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub"/> | Single-binary infrastructure for GitHub Projects triage: automated PR slicing, batch label reconciliation, and webhook ingestion with zero outbound dependencies. | [TaxonRouter](https://github.com/LOUST-PRO/TaxonRouter) |
| TCP-level Linux OS watchdog in Go (`lzt-broker-stall-reaper`): enumerates ESTABLISHED sockets to `broker.actions.githubusercontent.com:443` via `ss -tnpi`, tracks per-socket `bytes_received` over time, and triggers POSIX `tcp_diag` kernel RST (`ss --kill`) on stalled long-polls (>5 min 0 bytes received while idle) with Prometheus textfile metrics<br/><br/><img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white" alt="Go"/> <img src="https://img.shields.io/badge/tcp__diag-000000?style=flat-square&logo=linux&logoColor=white" alt="tcp_diag"/> <img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white" alt="Prometheus"/> <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions"/> | Eliminates zombie runner hangs when GitHub's V2 broker holds long-poll HTTP sockets open indefinitely; auto-recovers runner fleets without manual intervention. | [lzt-broker-stall-reaper](https://github.com/LOUST-PRO/lzt-broker-stall-reaper) |
| Multi-path MCP server + CLI bridge for Outlook / Microsoft 365: Go 1.21 stdio MCP server wrapping 11 Microsoft Graph API endpoints (mail, folders, rules, user profile, attachments) with OAuth 2.0 Device Code Flow, zero external dependencies, and unified CLI dispatcher (`lzt-outlook`) v0.1.0<br/><br/><img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white" alt="Go"/> <img src="https://img.shields.io/badge/MCP-7C3AED?style=flat-square" alt="MCP"/> <img src="https://img.shields.io/badge/Microsoft_Graph-0078D4?style=flat-square&logo=microsoft&logoColor=white" alt="Microsoft Graph"/> <img src="https://img.shields.io/badge/OAuth_2.0-2C3E50?style=flat-square" alt="OAuth 2.0"/> <img src="https://img.shields.io/badge/Apache_2.0-D22128?style=flat-square&logo=apache&logoColor=white" alt="Apache 2.0"/> | Enables autonomous agent fleets to interact with Microsoft 365 mailboxes via clean stdio JSON-RPC without embedding client secrets; 25 MiB attachment safety caps prevent memory overflow during context injection. | [outlook-mcp-suite](https://github.com/LOUST-PRO/outlook-mcp-suite/releases/tag/v0.1.0) |
| Modular Rust workspace (`paperforge-core`, `paperforge-cli`, `paperforge-tui`) managing Wallpaper Engine Workshop scenes on Linux: process isolation over POSIX signals (`SIGUSR1`/`SIGUSR2` audio toggle) for clean MIT vs GPL-3.0 separation, `WallpaperBackend` abstraction (`linux-wallpaperengine`, `swww`, `hyprpaper`, `mpvpaper`), and per-monitor reusable playlists<br/><br/><img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust"/> <img src="https://img.shields.io/badge/IPC-7C3AED?style=flat-square" alt="IPC"/> <img src="https://img.shields.io/badge/Wayland-000000?style=flat-square" alt="Wayland"/> <img src="https://img.shields.io/badge/MIT-3D4451?style=flat-square" alt="MIT"/> | Reusable per-monitor playlist engine with instant GPU/CPU release via process pause/resume and zero-overhead POSIX IPC. | [paperforge](https://github.com/louzt/paperforge) |
| Single-binary local-first bookmark manager in Rust (`LinkMarks` v1.0.1): deterministic canonical URL deduplication, Chromium JSON / Netscape HTML bridges, and CRDT multi-device sync architecture under AGPLv3 + Commercial dual licensing | Replaces heavy containerized web tools with a 2.5 MB static binary; eliminates silent network crawling and un-gated AI costs while enforcing strict offline data ownership and zero-telemetry egress.<br/><br/><a href="https://github.com/LOUST-PRO/LinkMarks"><img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust"/></a> <a href="#"><img src="https://img.shields.io/badge/Local--First-064E3B?style=flat-square" alt="Local-First"/></a> <a href="#"><img src="https://img.shields.io/badge/AGPLv3-3D4451?style=flat-square&logo=gnu&logoColor=white" alt="AGPLv3"/></a> | [LinkMarks](https://github.com/LOUST-PRO/LinkMarks) |
| Visual identity, access hierarchy, and turnstile validation layout for regional mass-transit credentials (2025–2026 cycle) | Sustained high-density passenger throughput and multi-tier zoning enforcement under strict security constraints. | **Tren Maya smart-card credentials** (2025, 2mo contractor) |
| Content-addressed documentation scraper tracking corpora changes via BLAKE3 and git-tree manifests<br/><br/><img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=FFD43B" alt="Python"/> <img src="https://img.shields.io/badge/BLAKE3-2C3E50?style=flat-square" alt="BLAKE3"/> <img src="https://img.shields.io/badge/Git_Tree-181717?style=flat-square&logo=git&logoColor=white" alt="Git tree"/> <img src="https://img.shields.io/badge/Virtuoso_7.2.6-2C3E50?style=flat-square" alt="Virtuoso 7.2.6"/> | Grounded local corpora feed Sovereign RAG (DSVH) and Virtuoso 7.2.6 pipelines, replacing ungrounded web searches with reproducible local context. | [spec-snapshot-scraper](https://github.com/LOUST-PRO/spec-snapshot-scraper) |
| Linux kernel, graphics, compositor, and runtime contract enforcement across public upstreams: Valve/Fossilize ([PR #305](https://github.com/ValveSoftware/Fossilize/pull/305): `PR_SET_PDEATHSIG` child process reaper + `getppid` race mitigation, protecting millions of Steam Deck & SteamOS devices from orphan Vulkan shader replayer CPU/battery leaks; ranked #7 among only 12 contributors worldwide to `master` in 2024–2026 alongside DXVK/VKD3D/Mesa leads; catalyzing Valve's [PR #308](https://github.com/ValveSoftware/Fossilize/pull/308) bucket metadata system + authoring [PR #311](https://github.com/ValveSoftware/Fossilize/pull/311) `static_assert` compile-time type-safety guard that unblocked Valve's +7,913 LOC `fossilize-feature-sifter` Mesa CI silicon audit suite in [PR #310](https://github.com/ValveSoftware/Fossilize/pull/310)), spotify-player ([PR #1049](https://github.com/aome510/spotify-player/pull/1049): `is_active && is_playing` Connect device state-machine disambiguation preventing TUI audio engine starvation on standby speakers + [PR #1048](https://github.com/aome510/spotify-player/pull/1048): search request serialization eliminating HTTP 429 rate-limit storms), rspotify ([Issue #572](https://github.com/ramsayleung/rspotify/issues/572): non-breaking Serde `#[serde(default)]` resilience patch for omitted `available_markets` DTOs), Waypaper ([PR #286](https://github.com/anufrievroman/waypaper/pull/286): scaling filter matrix), PipeWire ([commit 2f747a7](https://github.com/louzt/pipewire/commit/2f747a7): connect timeout), Niri ([5 PRs](https://gist.github.com/louzt/1c5230a2e9471faf9ce4243314361fa1): typed IPC diagnostics), Bottles<br/><br/><img src="https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=c%2B%2B&logoColor=white" alt="C++"/> <img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust"/> <img src="https://img.shields.io/badge/Linux_prctl-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux prctl"/> <img src="https://img.shields.io/badge/Valve--Fossilize-171a21?style=flat-square&logo=steam&logoColor=white" alt="SteamOS"/> <img src="https://img.shields.io/badge/Wayland-000000?style=flat-square" alt="Wayland"/> | Solves multi-runtime edge cases: orphan Vulkan shader replayers on Steam/Proton crashes under container subreapers (`pressure-vessel`), TUI audio engine starvation on standby Spotify Connect devices, HTTP 429 quota exhaustion, GTK subprocess teardown, frame-callback races, and daemon IPC hangs. | **Public Upstream Hardening** — [Valve/Fossilize #305](https://github.com/ValveSoftware/Fossilize/pull/305) · [#308](https://github.com/ValveSoftware/Fossilize/pull/308) · [#311](https://github.com/ValveSoftware/Fossilize/pull/311) · [#310](https://github.com/ValveSoftware/Fossilize/pull/310) · [spotify-player #1049](https://github.com/aome510/spotify-player/pull/1049) · [#1048](https://github.com/aome510/spotify-player/pull/1048) · [rspotify #572](https://github.com/ramsayleung/rspotify/issues/572) · [Waypaper #286](https://github.com/anufrievroman/waypaper/pull/286) · [PipeWire](https://github.com/louzt/pipewire/commit/2f747a7) |
| Multi-tenant MCP broker with intent-filter (`read \| mutate \| admin`) + resource engine for VRAM/cache budgeting + spec-watch loop aligning annotation contracts before downstream tools adopt breaking changes<br/><br/><img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust"/> <img src="https://img.shields.io/badge/MCP-7C3AED?style=flat-square" alt="MCP"/> <img src="https://img.shields.io/badge/Annotation_Pruning-8B5CF6?style=flat-square" alt="Annotation Pruning"/> <img src="https://img.shields.io/badge/Resource_Engine-2C3E50?style=flat-square" alt="Resource Engine"/> | Deterministic tool-call surface survives provider churn, prevents prompt-injection-style annotation drift, and keeps cost + latency within bounded envelopes. | **LZT MCP infrastructure** (private: `lzt-mcp-broker` + resource engine + spec scanners) |
| VSCode-native agent loop integration: read-only MCP server wiring live editor state, the SPARQL corpus graph, the watchdog pressure sensor, and the update manifest (4 read-only tools) + a hardened CLI companion wrapping the VSCode Insiders editor CLI as 4 typed tools (`cli_open_file`, `cli_diff`, `cli_list_extensions`, `cli_install_extension`) with subcommand allowlist, hardcoded path blocklist (`/etc`, `/proc`, `/root/.ssh/`, `/root/.gnupg/`, etc.), workspace-prefix enforcement, and publisher allowlist for install operations<br/><br/><img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white" alt="Go"/> <img src="https://img.shields.io/badge/VSCode_API-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white" alt="VSCode API"/> <img src="https://img.shields.io/badge/MCP-7C3AED?style=flat-square" alt="MCP"/> <img src="https://img.shields.io/badge/SPARQL-2C3E50?style=flat-square" alt="SPARQL"/> <img src="https://img.shields.io/badge/Allowlist-1F2937?style=flat-square" alt="Allowlist"/> | Lets the agent reason about the operator's live editing context (active extensions, dev ports, LSP, bridge, watchdog events, update drift vs `update.code.visualstudio.com`) and act on it through a tightly-scoped CLI surface — never with full shell, never with the path blocklist, never with unsigned extension publishers. Closed-loop improvement workflow: detect problem via watchdog → query corpus for upstream doc → diff/cross-reference via the read-only tools → propose change via the mutate surface, with daily JSONL audit log. Both servers declare MCP `readOnlyHint`/`destructiveHint` per tool; the read-only pair rides broker intent `read`, the mutate pair requires `mutate`/`admin`. | **lzt-vscode-mcp + lzt-vscode-cli** (private: read-only editor state + hardened CLI companion) |
| arXiv preprint LaTeX source and companion verification suite for FNV-1a + L2 + cosine projection pipelines<br/><br/><img src="https://img.shields.io/badge/LaTeX-008080?style=flat-square&logo=latex&logoColor=white" alt="LaTeX"/> <img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust"/> <img src="https://img.shields.io/badge/FNV--1a_64bit-2C3E50?style=flat-square" alt="FNV-1a 64-bit"/> <img src="https://img.shields.io/badge/Virtuoso_7.2.6-2C3E50?style=flat-square" alt="Virtuoso 7.2.6"/> | Formally proves estimator unbiasedness and concentration bounds, validated empirically under 25/25 thread concurrency stress testing. | [deterministic-sovereign-rag](https://github.com/LOUST-PRO/deterministic-sovereign-rag) + [dsvh-verification-suite](https://github.com/LOUST-PRO/dsvh-verification-suite) |
| High-efficiency subagent fleet that activates ONLY when an upstream spec (MCP, model APIs, Claude/Gemini/OpenAI changelogs) releases a breaking change outside the LLM's training window. Patches the harness' contract types before downstream tools observe the drift<br/><br/><img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust"/> <img src="https://img.shields.io/badge/Change_Detection-2C3E50?style=flat-square" alt="Change Detection"/> <img src="https://img.shields.io/badge/Zero_Egress-1F2937?style=flat-square" alt="Zero Egress"/> | Closes the "stale spec" gap in long-running agent fleets — a model released 4 months ago doesn't know about a spec change from 3 weeks ago, but the harness auto-detects and re-validates contracts before production rollout. | **Spec-watch subagent fleet** (private: `lzt-mcp-version-scan`, `lzt-changelog-aggregate`) |
| iCal-to-CalDAV bridge daemon translating public ICS subscriptions into localized CalDAV streams for native desktop clients<br/><br/><img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust"/> <img src="https://img.shields.io/badge/CalDAV-4285F4?style=flat-square" alt="CalDAV"/> <img src="https://img.shields.io/badge/Apache_2.0-D22128?style=flat-square&logo=apache&logoColor=white" alt="Apache 2.0"/> | Lightweight Linux runtime daemon transforming remote web calendar subscriptions into local, standards-compliant CalDAV endpoints. | [ical-to-caldav](https://github.com/LOUST-PRO/ical-to-caldav) |
| Compiler translating noisy LLM export payloads (ChatGPT, Claude, Gemini) into canonical JSONL + Markdown records<br/><br/><img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/> <img src="https://img.shields.io/badge/JSONL-1F2937?style=flat-square" alt="JSONL"/> <img src="https://img.shields.io/badge/Claude-CC785C?style=flat-square&logo=anthropic&logoColor=white" alt="Claude"/> <img src="https://img.shields.io/badge/ChatGPT-74AA9C?style=flat-square&logo=openai&logoColor=white" alt="ChatGPT"/> | Normalizes fragmented vendor exports into a structured context stream, eliminating ~60% token bloat during prompt injection. | [LLMmempipe](https://github.com/LOUST-PRO/LLMmempipe) |

<details>
<summary>Representative build signals & internal observability metrics</summary>

- **850K+ lines of production code** shipped across 50+ delivered projects (2019–2026)
- **Knowledge Graph Compaction & Triage**: SPARQL/TriG corpus indexation digesting historical issues, PRs, and commit diffs vs local forks for zero-overhead token budgeting and multi-branch differential analysis
- **Custom SAST & OSINT Vulnerability Scanners**: Problem-tailored static analysis rules and public OSINT threat intelligence mapping documented regressions against local codebases before patch submission
- **Cross-Fork Differential Test Harnesses**: Multi-branch simulation suites measuring execution latency, memory footprint, and state invariance across candidate patches vs upstream forks
- **9 packages and 391 TypeScript files** in Nexus Engine monorepo
- **42 Prisma models and 600+ GraphQL endpoints** in production B2B multi-tenant engines
- **Enterprise multi-tenant RBAC isolation** & autonomous agentic workflows
- **FOSS community CLA, DMCA, and Acceptable Use (AUP)** legal governance framework
- **50K embeddings queried in 188 ms** in GPU-oriented RAG retrieval pipelines
- **15-20% throughput gains** in NetBoozt TCP optimization benchmarks on Windows
- **<2 minute lead-to-quote response latency** in SYPREME conversion-attribution pipeline
- **Atomic CFDI 4.0 invoicing pipeline** (multi-tenant e-commerce + Stripe / MercadoPago / Crypto)
- **Redis channel count reduced 59 → 18** via SCAN/COUNT migration over KEYS

</details>


<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/section-what-we-ship.svg" width="100%" alt="What we ship at loust.pro — Software company section banner"/></p>

The technology provider behind my work — multi-protocol transport, hardened Linux substrate, and B2B platforms that survive multi-year horizons. Public artefacts land in **Research & Publications** and **Investigations & Notes**; this section is the product surface I run day-to-day.

<p align="right"><sub><em>LOUST · Leverage Opportunities Unleashing Success and Transformation</em></sub></p>

<table>
  <tr>
    <td valign="top" width="50%">
      <strong>Enterprise CMS</strong><br/>
      <sub>Multi-tenant content + commerce + operations platform with isolated Postgres/Redis namespaces per tenant. Single codebase runs marketing, ERP-lite flows, bookings, and storefronts.</sub><br/>
      <sub>
        <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"/>
        <img src="https://img.shields.io/badge/Astro-BC52EE?style=flat-square&logo=astro&logoColor=white" alt="Astro"/>
        <img src="https://img.shields.io/badge/Prisma-3982CE?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/>
        <img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/>
        <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
        <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis"/>
        <img src="https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white" alt="Cloudflare"/>
      </sub>
    </td>
    <td valign="top" width="50%">
      <strong>Automations</strong><br/>
      <sub>Rule + webhook engine for client operations. Connects Meta Ads, Google Ads, Stripe, MercadoPago, and CFDI 4.0 invoicing into auditable workflows with run history and replay.</sub><br/>
      <sub>
        <img src="https://img.shields.io/badge/Bun-000000?style=flat-square&logo=bun&logoColor=white" alt="Bun"/>
        <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
        <img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/>
        <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
        <img src="https://img.shields.io/badge/Redis_Streams-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis Streams"/>
      </sub>
    </td>
  </tr>
  <tr>
    <td valign="top" width="50%">
      <strong>CRM Hub</strong><br/>
      <sub>Pipeline + contact + closing surfaces for sales teams. Sub-2-minute lead-to-quote latency under exhibition pressure. Native multi-tenant isolation.</sub><br/>
      <sub>
        <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"/>
        <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
        <img src="https://img.shields.io/badge/Prisma-3982CE?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/>
        <img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/>
        <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
      </sub>
    </td>
    <td valign="top" width="50%">
      <strong><a href="https://loust.pro/socialsphere">SocialSphere</a></strong><br/>
      <sub>PropTech + hospitality ERP. Multi-property booking, turnover calendars, and channel-manager hooks. CTO since Dec 2025.</sub><br/>
      <sub>
        <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"/>
        <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
        <img src="https://img.shields.io/badge/Prisma-3982CE?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/>
        <img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/>
        <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
        <img src="https://img.shields.io/badge/Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white" alt="Stripe"/>
        <img src="https://img.shields.io/badge/Tauri-FFC131?style=flat-square&logo=tauri&logoColor=black" alt="Tauri"/>
      </sub>
    </td>
  </tr>
  <tr>
    <td valign="top" width="50%">
      <strong>Nexus Apps</strong><br/>
      <sub>Spec-driven generators and platform scaffolding. 9 packages and 391 TypeScript files keep multi-app ecosystems consistent from one source of truth instead of copy-paste.</sub><br/>
      <sub>
        <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
        <img src="https://img.shields.io/badge/Bun-000000?style=flat-square&logo=bun&logoColor=white" alt="Bun"/>
        <img src="https://img.shields.io/badge/esbuild-FFCF00?style=flat-square&logo=esbuild&logoColor=black" alt="esbuild"/>
        <img src="https://img.shields.io/badge/tsc-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="tsc"/>
        <img src="https://img.shields.io/badge/vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white" alt="vitest"/>
      </sub>
    </td>
    <td valign="top" width="50%">
      <strong>Marketplace</strong><br/>
      <sub>Multi-vendor e-commerce with CFDI 4.0 invoicing, Stripe + MercadoPago splits, and a verified directory for sellers. Atomic invoicing pipeline keeps the trail auditable end-to-end.</sub><br/>
      <sub>
        <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"/>
        <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
        <img src="https://img.shields.io/badge/Prisma-3982CE?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/>
        <img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/>
        <img src="https://img.shields.io/badge/Stripe_Connect-635BFF?style=flat-square&logo=stripe&logoColor=white" alt="Stripe Connect"/>
        <img src="https://img.shields.io/badge/CFDI_4.0-2C3E50?style=flat-square" alt="CFDI 4.0"/>
      </sub>
    </td>
  </tr>
  <tr>
    <td valign="top" width="50%">
      <strong>AI Chatbot</strong><br/>
      <sub>Multi-tenant conversational surface for client ops. ReAct reasoning loop with provider-rotation across MiniMax M3, ChatGPT, Claude, DeepSeek, Gemini, Llama, and free-tier fallbacks; per-tenant retry budget keeps cost bounded. Routes to human handoff with full context, sessions in tenant-isolated Redis namespaces, exports to CRM Hub on close.</sub><br/>
      <sub>
        <img src="https://img.shields.io/badge/Bun-000000?style=flat-square&logo=bun&logoColor=white" alt="Bun"/>
        <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
        <img src="https://img.shields.io/badge/MiniMax_M3-FF6B6B?style=flat-square" alt="MiniMax M3"/>
        <img src="https://img.shields.io/badge/Pollinations-FF6B6B?style=flat-square" alt="Pollinations"/>
        <img src="https://img.shields.io/badge/ChatGPT-74AA9C?style=flat-square&logo=openai&logoColor=white" alt="ChatGPT"/>
        <img src="https://img.shields.io/badge/Claude-CC785C?style=flat-square&logo=anthropic&logoColor=white" alt="Claude"/>
        <img src="https://img.shields.io/badge/DeepSeek-1A4F8C?style=flat-square" alt="DeepSeek"/>
        <img src="https://img.shields.io/badge/Gemini-4285F4?style=flat-square&logo=google&logoColor=white" alt="Gemini"/>
        <img src="https://img.shields.io/badge/Llama-0467DF?style=flat-square&logo=meta&logoColor=white" alt="Llama"/>
        <img src="https://img.shields.io/badge/ReAct-7C3AED?style=flat-square" alt="ReAct"/>
        <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis"/>
        <img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/>
      </sub>
    </td>
    <td valign="top" width="50%">
      <strong>Public Research Notes</strong><br/>
      <sub>Long-form writeups on sovereign RAG, transport-layer hardening, kernel regressions, and infrastructure audits. Public-by-default where the abstraction boundary is legible.</sub><br/>
      <sub>
        <img src="https://img.shields.io/badge/Astro-BC52EE?style=flat-square&logo=astro&logoColor=white" alt="Astro"/>
        <img src="https://img.shields.io/badge/MDX-1B1F24?style=flat-square&logo=mdx&logoColor=white" alt="MDX"/>
        <img src="https://img.shields.io/badge/Gist-2C3E50?style=flat-square&logo=github&logoColor=white" alt="GitHub gist"/>
        <img src="https://img.shields.io/badge/ORCID-A6CE39?style=flat-square&logo=orcid&logoColor=white" alt="ORCID bridge"/>
      </sub>
    </td>
  </tr>
</table>


<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/section-research-and-publications.svg" width="100%" alt="Research and Publications — section banner"/></p>

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

### APQ at Scale on a 135k-Line GraphQL Schema (case study, 2026)

Empirical anchor for the theorems above: **90.9% cache hit rate, p95 12 ms latency, +125% throughput lift, $0/mo incremental infra cost** on the LOUST multi-tenant Next.js 16 + Apollo Server v4 stack against a 135k-line Prisma-derived GraphQL schema. The case study is the production evidence the formal results lean on — same $\lambda T \approx 389$ regime cited in Theorem A.1, same $r_1 \approx 0.25$ APQ compression ratio in Theorem B.1, and the same +125% throughput lift that compounds with Brotli q11 in the production measurements. Eight diagnostic anchors (cgroup v2 isolation, CB convergence, Zipf coverage, PSI pressure detection) and seven theorems ($H \leq 1 - \exp(-\lambda T)$, throughput gain $G = \frac{1 + \rho \cdot \frac{W_o}{W_r}}{1 + \rho \cdot \frac{W_o}{W_r'}}$, $R_{\text{total}} \approx 0.075$ end-to-end bandwidth) make the case study reviewable as a small formal dossier rather than a benchmark dump. Operator's diagnostic posture: if any of the seven anchors fire in production, the recipe (pre-warm + Redis Lua EVAL + cgroup v2 slice + persistent runner volume) is named and measurable in the document.

<p align="center">
  <a href="https://gist.github.com/louzt/64715cb9c6ec6ffdd98c5712b8fb7bac"><img src="https://img.shields.io/badge/Read_the_case_study-English-7C3AED?style=for-the-badge&logo=github&logoColor=white" alt="Read the APQ case study (English)"/></a>
  &nbsp;
  <a href="https://gist.github.com/louzt/0c91771bf6370f0eb47e905934ab47e8"><img src="https://img.shields.io/badge/Leer_el_caso_de_estudio-Español-D97706?style=for-the-badge&logo=github&logoColor=white" alt="Leer el caso de estudio APQ (Español)"/></a>
</p>

<sub>Stack: Next.js 16 `cacheComponents` + Apollo Server v4 + `ApolloAPQCache` + Redis 7 `ioredis` keyPrefix + Lua EVAL atomic + cgroup v2 `compile-runner.slice` + self-hosted GitHub Actions runner with persistent `/opt/build-cache` volume. Diagnostic anchors: §3.8 cgroup v2 runner isolation, Appendix F slice + hooks, Theorem E.8 throughput gain under cgroup contention. Public artefact, no host infra numbers exposed.</sub>

<p align="center"><img src="https://capsule-render.vercel.app/api?type=rect&color=0:0f172a,100:1e293b&height=2" width="100%"/></p>

### Zero-Prefill Keep-Alive Protocol & Multi-Region Clock Drift (operator stack paper draft, 2026)

Cost-benefit gate for cache-warming probes against upstream GPU clusters and multi-region agent control planes. Three-step procedure: **monitor** the upstream's TTL state via a single `max_tokens=1` probe (5-minute heartbeat cadence dynamically calibrated via Weibull survival analysis), **trigger** an asymmetric EMA update based on the boolean cache-hit response, and **fire** the next probe only when the gate fires. 

The protocol is **800× cheaper** than a cold start at `K=1` and **50× cheaper** than an evict-and-compress cycle at `K=16` under upstream rate limits (`5,000 req/hour`). Integrates **Marzullo's 1994 intersection algorithm** to bound multi-region clock drift ($\Delta t \le \epsilon_{\text{ntp}} + \delta_{\text{drift}}$), **Lamport happens-before ordering** (`CLOCK_MONOTONIC`), and a **Weibull survival distribution** ($\lambda(t) = \frac{k}{\lambda}\left(\frac{t}{\lambda}\right)^{k-1}$) modeling GPU VRAM cache eviction under non-stationary token loads.

<sub>Stack: Go (APG) + Rust (DSVH) + Lamport happens-before ordering + Marzullo 1994 intersection bound + CLOCK_MONOTONIC + Weibull survival bounds. Documented in §5 (clock drift), §8 (DET protocol), §9 (zero-prefill), and §12 (boundary conditions) of the Sovereign RAG operator paper.</sub>

<p align="center"><img src="https://capsule-render.vercel.app/api?type=rect&color=0:0f172a,100:1e293b&height=2" width="100%"/></p>

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/section-investigations-and-notes.svg" width="100%" alt="Investigations and Notes — section banner"/></p>

Public research notes, snapshots, and audit logs from ongoing work. Updated as findings stabilize.

| Topic | Type | Notes |
| --- | --- | --- |
| [lzt-* gist collection](https://gist.github.com/louzt) | Mixed · 9+ gists | Bash hardening snippets, systemd unit definitions, MCP surface designs, certificate chains, transport proxy configs |
| [Agent Provenance & Meta-Telemetry Detection](https://gist.github.com/louzt/d1ce71c05460c2c32bf31342cd0c6a3f) | Agent Architecture · Telemetry | `agent_id` provenance tagging, `lzt-branch-claim` verification, working-tree author classification, and automated PR-slicing gates for multi-agent fleets. |
| [APQ at Scale (135k-line GraphQL Schema)](https://gist.github.com/louzt/64715cb9c6ec6ffdd98c5712b8fb7bac) · [ES](https://gist.github.com/louzt/0c91771bf6370f0eb47e905934ab47e8) | GraphQL performance · Edge runtime · Self-hosted runners | 90.9% hit rate, p95 12 ms, +125% throughput, $0/mo. Seven diagnostic anchors + seven theorems; §3.8 cgroup v2 runner isolation (slice + Lua EVAL pre-warm + persistent `/opt/build-cache`). Companion to the APQ theorems in the Research and Publications section above. |
| [Resilient Transport vs Stateful DPI](https://gist.github.com/louzt/3991f144c7d67726045af3cefc60f42a) | Network engineering | 5-tier QUIC/Hysteria2/TLS/SSH fallback proxy; Happy Eyeballs racing in <200 ms; CA-pinned topology |
| [PipeWire handshake timeout (protocol-native)](https://github.com/louzt/pipewire/commit/2f747a7) | C / Linux core | 5s `spa timer` on `pw_protocol_native_connect_local_socket()`; prevents indefinite CLI hangs (`wpctl`/`pactl`) when daemon is alive but unresponsive. Published upstream on Freedesktop (PipeWire). |
| [Valve/Fossilize PR #305](https://github.com/ValveSoftware/Fossilize/pull/305) · [PR #308](https://github.com/ValveSoftware/Fossilize/pull/308) · [PR #311](https://github.com/ValveSoftware/Fossilize/pull/311) | C++ · Linux Systems · Vulkan | `PR_SET_PDEATHSIG` + `getppid()` race check in `fossilize_replay_linux` & `external_replayer`; terminates orphan Vulkan shader replayers immediately when Steam/Proton crashes, eliminating 100% CPU runaway worker leaks & battery drain across millions of Steam Deck, SteamOS, and Linux gaming devices. Ranked #7 among only 12 contributors worldwide to `ValveSoftware/Fossilize` master in 2024–2026 (alongside DXVK creator Philip Rebohle, Valve Vulkan lead Hans-Kristian Arntzen, and Intel/AMD Mesa driver leads). Merged in Valve's official repo. Catalyzed Valve's follow-up [PR #308](https://github.com/ValveSoftware/Fossilize/pull/308) (`bucket-json-system` metadata & FNV-1a de-hashing using vendor matrix) and authored [PR #311](https://github.com/ValveSoftware/Fossilize/pull/311) (`fossilize-list` `RESOURCE_BUCKET_INFO` enum alignment & `static_assert` compile-time safeguard preventing OOB array reads). |
| [Niri State Observability (Wayland typed-diagnostics)](https://gist.github.com/louzt/1c5230a2e9471faf9ce4243314361fa1) | Wayland compositor · Rust IPC | Pull-based typed diagnostics over Niri IPC; semantic asset labeling; per-output mutex; anchored 5 PRs upstream |
| [Waypaper image-filter PR #286](https://github.com/louzt/761e227ad8cfe55b29e79cf861214a62) | Upstream OSS | Scaling algorithms exposed across swww/awww backends; HiDPI + pixel-art artifact resolution |
| [Zero-overhead observability](https://gist.github.com/louzt/b8349629b602a782ac98d0cbfd0df0c0) | Linux runtime | PSI over polling; inotify fork-bomb mitigation; Redis KEYS → SCAN/COUNT migration |
| [Chromium 148 CSP regression audit](https://gist.github.com/louzt/77f0804ca11bad6636f0ac67928bd384) | Web security | Accepted upstream under Opera GB-80414; CSP Level 3 + srcdoc sandbox collision isolation |
| [spotify-player Connect State Disambiguation](https://github.com/aome510/spotify-player/pull/1049) | Async Rust · TUI Audio Engine | Disambiguated `is_active` Connect device presence from active playback (`is_playing`) in `new_session()`, preventing `librespot` audio engine starvation when standby smart speakers (e.g., Echo) report presence without audio streams. |
| [spotify-player Metadata Search Serialization](https://github.com/aome510/spotify-player/pull/1048) | Async Rust · Rate-Limiting | Serialized concurrent search requests to eliminate HTTP 429 QUOTA_EXCEEDED bursts during rapid TUI navigation. |
| [rspotify DTO Deserialization Resiliency](https://github.com/ramsayleung/rspotify/issues/572) | Rust · Serde DTOs | Identified API schema drift in `GET /v1/me/shows` where omitted `available_markets` broke Serde deserialization; proposed non-breaking `#[serde(default)]` fallback preserving `Vec<String>` public API stability. |
| [Self-scaling Minecraft Cluster on k3s](https://gist.github.com/louzt/b333b5601628a159630da13857834246) · [ES](https://gist.github.com/louzt/8e3b86c7398016964699e87d52222cf7) | Kubernetes · k3s · Automation | RCON-driven automated idle cluster teardown & auto-scaling for zero-cost standby game infrastructure on k3s. |
| [OpenAL Soft & ALSA Audio Container Resilience](https://gist.github.com/louzt/c175973d8e8bae8c8fef6af4d9d6aca7) · [ES](https://gist.github.com/louzt/dbc83b2ac0f7fa0f3938b7705c36c719) | Linux Subsystems · Containerization | Resolving OpenAL Soft & ALSA device mismatches and audio buffer overruns under Distrobox / LXC containerized environments. |
| [NVIDIA DKMS Kernel 7.0+ RFC](https://gist.github.com/louzt/1c85044d5090d19223c3f5edf426a19e) | Linux kernel · C | Forward-compat patch series for Kernel 7.0 API refactoring: VMA locking (`__is_vma_write_locked()` 2→1 args), DMA fence signal (`dma_fence_signal_locked()` int→void), `__vm_flags` removal in favor of `vm_flags_reset()`. 3-layer DKMS build-loop triage (`no-autoinstall` + `apt-mark hold` + unattended-upgrades blacklist). `NVreg_DynamicPowerManagement=0x02` modprobe rule for Optimus USB-C D3cold hotplug panics under hybrid GPUs. |

<p align="right"><sub><em>LOUST · Leverage Opportunities Unleashing Success and Transformation</em></sub></p>

> _Public gists are linked individually above as they ship. For private work-in-progress and operational forensics, see [LinkedIn](https://www.linkedin.com/in/davidmirelesll/?locale=es_ES) for the curated view._

<p align="center"><img src="https://capsule-render.vercel.app/api?type=rect&color=0:0f172a,100:1e293b&height=2" width="100%"/></p>

<!-- ============================================================ -->
<!-- FOOTER: animated squares grid + tagline (no operator name).  -->
<!-- Served from profile-public static/ alongside the section     -->
<!-- banners. Editor-only provenance; GitHub strips the comment.  -->
<!-- ============================================================ -->
<div align="center">
  <img alt="Animated footer tagline" src="https://raw.githubusercontent.com/louzt/louzt/main/static/profile-footer.svg" width="100%" style="display:block;margin:0 auto"/>
</div>
