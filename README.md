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

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider.svg" width="100%" alt="divider"/></p>

<h3 align="center"><b>SERVICES &amp; ENGINEERING SOLUTIONS MATRIX</b></h3>

<p align="center"><sub>High-rigor technical services and consulting backed by 850K+ lines of production code across 50+ delivered systems</sub></p>

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

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider.svg" width="100%" alt="divider"/></p>

<h3 align="center"><b>PUBLIC UPSTREAM HARDENING &amp; CORE SYSTEMS INVARIANTS</b></h3>

<p align="center"><sub>Direct C/C++, Rust, and Linux kernel contributions merged into primary upstream repositories</sub></p>

| Upstream Target | Technical Contribution & Verification | Role / Reach |
| :--- | :--- | :--- |
| **Valve Software**<br/>`ValveSoftware/Fossilize`<br/>([PR #305](https://github.com/ValveSoftware/Fossilize/pull/305) · [#308](https://github.com/ValveSoftware/Fossilize/pull/308) · [#311](https://github.com/ValveSoftware/Fossilize/pull/311) · [#310](https://github.com/ValveSoftware/Fossilize/pull/310)) | Eradicated Vulkan shader replayer zombie processes and background CPU/battery drain across Steam Deck / SteamOS devices via `PR_SET_PDEATHSIG` + `getppid` race mitigation (#305). Catalyzed the `RESOURCE_BUCKET_INFO = 10` multi-GPU manifest schema (#308) and authored the `static_assert` compile-time type-safety guard (#311) that unblocked Valve's +7,913 LOC `fossilize-feature-sifter` Mesa CI silicon audit suite (#310). | **Rank #7 of 12** worldwide contributors to `master` (2024–2026) alongside Valve, DXVK, and Mesa leads. |
| **Freedesktop PipeWire**<br/>`pipewire/pipewire`<br/>([commit 2f747a7](https://github.com/louzt/pipewire/commit/2f747a7)) | Implemented 5s `spa timer` protocol-native connection timeouts on `pw_protocol_native_connect_local_socket()`, preventing indefinite CLI hangs (`wpctl`/`pactl`) when daemon sockets lock up. | Upstream C / Linux Audio Subsystem Hardening. |
| **Niri Wayland Compositor**<br/>([5 PRs / Gist](https://gist.github.com/louzt/1c5230a2e9471faf9ce4243314361fa1)) | Engineered pull-based typed IPC diagnostics, semantic asset labeling, and per-output mutex thread isolation across Wayland display outputs. | Upstream Rust / Compositor IPC Diagnostics. |
| **spotify-player & rspotify**<br/>([PR #1049](https://github.com/aome510/spotify-player/pull/1049) · [#1048](https://github.com/aome510/spotify-player/pull/1048) · [Issue #572](https://github.com/ramsayleung/rspotify/issues/572)) | Disambiguated `is_active && is_playing` Connect device state-machines to prevent TUI audio engine starvation on standby speakers (#1049), serialized search requests to block HTTP 429 quota exhaustion (#1048), and applied Serde `#[serde(default)]` resilience to handle schema drift. | Upstream Async Rust & TUI Engine Resilience. |
| **Waypaper**<br/>([PR #286](https://github.com/anufrievroman/waypaper/pull/286)) | Exposed scaling filter matrix across swww/awww backends, resolving HiDPI and pixel-art rendering artifacts. | Upstream Wallpaper Manager Hardening. |
| **NVIDIA DKMS Kernel 7.0+ RFC**<br/>([Gist RFC](https://gist.github.com/louzt/1c85044d5090d19223c3f5edf426a19e)) | Forward-compat patch series for Kernel 7.0 API refactoring (VMA locking, DMA fence signals) and `NVreg_DynamicPowerManagement=0x02` modprobe rules for Optimus USB-C D3cold hotplug panics. | Linux Kernel 7.0+ API Refactoring & GPU Hardening. |
| **DankMaterialShell (DMS)**<br/>*(Upstream Patch Series)* | Engineered Quickshell / QML wayland shell component hardening, memory-leak fixes, and zero-leak state management. | Upstream Wayland Shell Hardening. |

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider.svg" width="100%" alt="divider"/></p>

<h3 align="center"><b>B2B MULTI-TENANT PLATFORMS &amp; SOVEREIGN SYSTEMS</b></h3>

<p align="center"><sub>Production platforms, enterprise engines, and standalone desktop software shipped to end-users</sub></p>

| System / Engine | Technical Focus & Architecture | Operational Impact |
| :--- | :--- | :--- |
| **LOUST Multi-Tenant Engine**<br/>*(Current, 7y 6m)* | Multi-tenant Next.js 16 + Apollo Server v4 + Redis 7 Lua EVAL + cgroup v2 isolation on a 135k-line GraphQL schema. Case study: [English](https://gist.github.com/louzt/64715cb9c6ec6ffdd98c5712b8fb7bac) / [Español](https://gist.github.com/louzt/0c91771bf6370f0eb47e905934ab47e8). | **90.9% APQ cache hit rate**, $p95 = 12\text{ ms}$, $+125\%$ throughput lift at $0/\text{mo}$ incremental infrastructure cost. |
| **h4kken 3D Rollback Engine**<br/>*(h4kken.loust.pro)* | GGPO-style rollback (30-frame window) + WebRTC/WebSocket dual transport + Babylon.js 8 WebGPU/WebGL rendering. | Sub-frame input prediction (>70% accurate) and seamless WebRTC DataChannel upgrades under restrictive NATs/DPI. |
| **SnapPipe**<br/>([GitHub](https://github.com/LOUST-PRO/SnapPipe)) | Identity-anchored transport toolkit binding sessions to Ed25519 public keys instead of `ip:port` tuples. | Solves SSH/QUIC head-of-line blocking under strict NATs/firewalls with zero unauthenticated frame exposure. |
| **NetBoozt**<br/>([GitHub](https://github.com/LOUST-PRO/NetBoozt_InternetUpgrade)) | Tauri v3.1 (Rust) + Python CLI + systemd daemon enforcing Linux BBR-equivalent TCP optimizations on Windows. | $+15\text{--}20\%$ real-world throughput gains via queueing discipline, ECN negotiation, and Fast Open tuning. |
| **LinkMarks**<br/>([GitHub](https://github.com/LOUST-PRO/LinkMarks)) | 2.5 MB single-binary bookmark engine in Rust with CRDT multi-device sync under AGPLv3 + Commercial dual license. | Replaces heavy containerized web tools with zero-telemetry egress and deterministic canonical URL deduplication. |
| **Tren Maya Smart Credentials**<br/>*(2025 Contractor)* | Visual identity, access hierarchy, and turnstile validation layout for regional mass-transit credentials. | Sustained high-density passenger throughput and multi-tier zoning enforcement under strict security constraints. |
| **TaxonRouter**<br/>([GitHub](https://github.com/LOUST-PRO/TaxonRouter)) | Dual-binary GitHub automation in Go: MCP stdio server + webhook auto-tagger. Listens to incoming issue/PR webhooks, auto-tags categories, reconciles labels, and manages GitHub Projects triage. | Automated GitHub issue/PR auto-tagging, label reconciliation, and zero-dependency webhook ingestion. |

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider.svg" width="100%" alt="divider"/></p>

<h3 align="center"><b>SOVEREIGN AI AGENT CONTROL PLANES &amp; SUBSTRATES</b></h3>

<p align="center"><sub>Autonomous agent fleets, local-first RAG substrates, and AI protocol bridges</sub></p>

| Substrate / Tooling | Architecture & Hardening | Value Proposition |
| :--- | :--- | :--- |
| **LZT SRE Harness**<br/>*(Private)* | Distributed data plane in Rust + Go: routing, cache control, and a hardened tool-call pipeline for autonomous agents. | Decouples agent reasoning from provider volatility; 3-way semantic sync + Bayesian Stream Guard (<0.5s kill-switch). |
| **h3ph43st Agent Runtime**<br/>*(Private, AGPLv3)* | Closed-core agent runtime: pruned Rust CLI (`h3ph`) talking to a multi-tenant k3s sidecar for ephemeral SAST scans. | Locked egress and isolated reasoning — client nodes never see system prompts, tool contracts, or reasoning loops. |
| **Multi-Protocol Agent Transport**<br/>*(Private)* | Go + Rust proxy racing QUIC / Hysteria2 / TLS / SSH, promoting the first-healthy stream under 200ms. | Keeps agent tool-call round-trips within budget even under captive portals, mobile NATs, or restrictive firewalls. |
| **lzt-broker-stall-reaper**<br/>([GitHub](https://github.com/LOUST-PRO/lzt-broker-stall-reaper)) | TCP-level Linux OS watchdog in Go enumerating sockets via `ss -tnpi` and firing `tcp_diag` kernel RST on stalled long-polls. | Auto-recovers GitHub Actions runner fleets when upstream broker sockets hang indefinitely without manual intervention. |
| **outlook-mcp-suite**<br/>([GitHub](https://github.com/LOUST-PRO/outlook-mcp-suite)) | Go 1.21 stdio MCP server wrapping 11 Microsoft Graph endpoints with OAuth 2.0 Device Code Flow and 25 MiB attachment caps. | Enables autonomous agent fleets to interact with Microsoft 365 mailboxes via clean stdio JSON-RPC without client secrets. |
| **Spec-Watch Subagent Fleet**<br/>*(Private)* | Event-driven Rust scanners detecting breaking spec changes across MCP, OpenAI, Claude, and Gemini changelogs. | Auto-patches agent contract types before downstream tools observe spec drift outside the LLM's training window. |

<p align="center">
  <a href="https://github.com/LOUST-PRO"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/banner-loust-pro-org.svg" width="100%" alt="LOUST-PRO Open Source &amp; Enterprise Substrates"/></a>
</p>

<p align="center">
  <a href="https://github.com/LOUST-PRO"><img src="https://img.shields.io/badge/Explore_LOUST--PRO_Organization-GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="Explore LOUST-PRO GitHub Organization"/></a>
  &nbsp;
  <a href="https://github.com/LOUST-PRO/SnapPipe"><img src="https://img.shields.io/badge/SnapPipe-Identity_Transport-0093D0?style=for-the-badge&logo=rust&logoColor=white" alt="SnapPipe Repo"/></a>
  &nbsp;
  <a href="https://github.com/LOUST-PRO/NetBoozt_InternetUpgrade"><img src="https://img.shields.io/badge/NetBoozt-TCP_Optimization-FFC131?style=for-the-badge&logo=tauri&logoColor=black" alt="NetBoozt Repo"/></a>
  &nbsp;
  <a href="https://github.com/LOUST-PRO/LinkMarks"><img src="https://img.shields.io/badge/LinkMarks-Local_CRDT-064E3B?style=for-the-badge&logo=rust&logoColor=white" alt="LinkMarks Repo"/></a>
</p>

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

<blockquote style="border-left: 3px solid #8b5cf6; background: #0f172a; padding: 16px; margin: 16px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
  <h4>🔬 Deterministic Sovereign RAG via Signed-Hash Projection (paper draft, 2026)</h4>
  <p>A four-formula operator stack for reproducible retrieval on sovereign cloud corpora: FNV-1a 64-bit feature hashing into a fixed <code>D = 128</code> vector, <code>L2</code> spherical normalization, cosine reduced to a dot product on the unit hypersphere, and a pagination throughput window for upstream API rate-limit optimization. <b>Seven theorems</b> bound estimator unbiasedness, variance via Weinberger 2009, exponential collision concentration via the non-asymptotic Hanson–Wright inequality, <code>O(D)</code> storage/matching, scale invariance under <code>L2</code> normalization, the cosine/dot equivalence, and the <code>R_throughput</code> operational bound.</p>
  <p>Validated empirically on a <b>4,458-document operator corpus</b> — indexed in 4.14 s (σ=0.18 s) with 640 ns match latency (σ=85 ns) and 0.78 top-5 recall. A 25/25 concurrency stress test on the production Rust implementation (<code>DSVH</code>) demonstrates stable operation under sustained workload.</p>
  <p align="center">
    <a href="https://gist.github.com/louzt/d1ce71c05460c2c32bf31342cd0c6a3f"><img src="https://img.shields.io/badge/Read_the_math_gist-English-7C3AED?style=for-the-badge&logo=github&logoColor=white" alt="Read the Sovereign RAG math gist (English)"/></a>
    &nbsp;
    <a href="https://gist.github.com/louzt/a75f9cf1a2f2edbd5af0e8d23526871d"><img src="https://img.shields.io/badge/Leer_las_matemáticas-Español-D97706?style=for-the-badge&logo=github&logoColor=white" alt="Leer las matemáticas del Sovereign RAG (Español)"/></a>
  </p>
  <sub>Stack: Rust (DSVH) + Go (APG) + Virtuoso 7.2.6 + FNV-1a 64-bit + L2 normalization. Open question: empirical head-to-head against dense embedders (BGE-M3, multilingual) — left for future work.</sub>
</blockquote>

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider.svg" width="100%" alt="divider"/></p>

<blockquote style="border-left: 3px solid #38bdf8; background: #0f172a; padding: 16px; margin: 16px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
  <h4>⚡ APQ at Scale on a 135k-Line GraphQL Schema (case study, 2026)</h4>
  <p>Empirical anchor for the theorems above: <b>90.9% cache hit rate, p95 12 ms latency, +125% throughput lift, $0/mo incremental infra cost</b> on the LOUST multi-tenant Next.js 16 + Apollo Server v4 stack against a 135k-line Prisma-derived GraphQL schema. The case study is the production evidence the formal results lean on — same $\lambda T \approx 389$ regime cited in Theorem A.1, same $r_1 \approx 0.25$ APQ compression ratio in Theorem B.1, and the same +125% throughput lift that compounds with Brotli q11 in the production measurements.</p>
  <p>Eight diagnostic anchors (cgroup v2 isolation, CB convergence, Zipf coverage, PSI pressure detection) and seven theorems make the case study reviewable as a small formal dossier rather than a benchmark dump.</p>
  <p align="center">
    <a href="https://gist.github.com/louzt/64715cb9c6ec6ffdd98c5712b8fb7bac"><img src="https://img.shields.io/badge/Read_the_case_study-English-7C3AED?style=for-the-badge&logo=github&logoColor=white" alt="Read the APQ case study (English)"/></a>
    &nbsp;
    <a href="https://gist.github.com/louzt/0c91771bf6370f0eb47e905934ab47e8"><img src="https://img.shields.io/badge/Leer_el_caso_de_estudio-Español-D97706?style=for-the-badge&logo=github&logoColor=white" alt="Leer el caso de estudio APQ (Español)"/></a>
  </p>
  <sub>Stack: Next.js 16 <code>cacheComponents</code> + Apollo Server v4 + <code>ApolloAPQCache</code> + Redis 7 <code>ioredis</code> keyPrefix + Lua EVAL atomic + cgroup v2 <code>compile-runner.slice</code> + self-hosted GitHub Actions runner with persistent <code>/opt/build-cache</code> volume.</sub>
</blockquote>

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider.svg" width="100%" alt="divider"/></p>

<blockquote style="border-left: 3px solid #10b981; background: #0f172a; padding: 16px; margin: 16px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
  <h4>📡 Zero-Prefill Keep-Alive Protocol &amp; Multi-Region Clock Drift (operator stack paper draft, 2026)</h4>
  <p>Cost-benefit gate for cache-warming probes against upstream GPU clusters and multi-region agent control planes. Three-step procedure: <b>monitor</b> the upstream's TTL state via a single <code>max_tokens=1</code> probe (5-minute heartbeat cadence dynamically calibrated via Weibull survival analysis), <b>trigger</b> an asymmetric EMA update based on the boolean cache-hit response, and <b>fire</b> the next probe only when the gate fires.</p>
  <p>The protocol is <b>800× cheaper</b> than a cold start at <code>K=1</code> and <b>50× cheaper</b> than an evict-and-compress cycle at <code>K=16</code> under upstream rate limits (<code>5,000 req/hour</code>). Integrates <b>Marzullo's 1994 intersection algorithm</b> to bound multi-region clock drift ($\Delta t \le \epsilon_{\text{ntp}} + \delta_{\text{drift}}$), <b>Lamport happens-before ordering</b> (<code>CLOCK_MONOTONIC</code>), and a <b>Weibull survival distribution</b> ($\lambda(t) = \frac{k}{\lambda}\left(\frac{t}{\lambda}\right)^{k-1}$) modeling GPU VRAM cache eviction under non-stationary token loads.</p>
  <sub>Stack: Go (APG) + Rust (DSVH) + Lamport happens-before ordering + Marzullo 1994 intersection bound + CLOCK_MONOTONIC + Weibull survival bounds. Documented in §5 (clock drift), §8 (DET protocol), §9 (zero-prefill), and §12 (boundary conditions) of the Sovereign RAG operator paper.</sub>
</blockquote>

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider.svg" width="100%" alt="divider"/></p>

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

<blockquote style="border-left: 3px solid #10b981; background: #0f172a; padding: 20px; margin: 24px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
  <h4 align="center">💡 <b>What This Systems Engineering Posture Means For Your Platform</b></h4>
  <p>The formal proofs, upstream PRs, and kernel investigations above reflect a single operational rule: <b>we fix substrate root causes before scaling</b>.</p>
  <ul>
    <li><b>Zero-Regression Production Safety:</b> Compile-time safeguards (<code>static_assert</code>), process reapers (<code>PR_SET_PDEATHSIG</code>), and deterministic RAG bounds ensure your systems remain memory-leak-free and resilient under heavy traffic.</li>
    <li><b>Substrate-First Cost Efficiency:</b> Edge-persisted GraphQL (90.9% APQ hit rate) and Linux kernel TCP tuning keep infrastructure costs at $0/mo incremental overhead while lifting throughput by +125%.</li>
    <li><b>Zero-Trust Security & IP Protection:</b> Locked-egress agent runtimes, CA-pinned transport proxies, and auditable 72-hour vulnerability disclosure protect your business data and user trust.</li>
  </ul>
  <p align="center">
    <a href="mailto:partnership@loust.pro"><img src="https://img.shields.io/badge/Architecture_Audit-partnership%40loust.pro-10B981?style=for-the-badge&logo=mail.ru&logoColor=white" alt="Schedule Architecture Audit"/></a>
    &nbsp;
    <a href="mailto:security@loust.pro"><img src="https://img.shields.io/badge/Security_Triage-security%40loust.pro-38BDF8?style=for-the-badge&logo=hackerone&logoColor=white" alt="Security Triage"/></a>
    &nbsp;
    <a href="mailto:research@loust.pro"><img src="https://img.shields.io/badge/R%26D_Collaboration-research%40loust.pro-8B5CF6?style=for-the-badge&logo=orcid&logoColor=white" alt="R&D Collaboration"/></a>
  </p>
</blockquote>

<p align="right"><sub><em>LOUST · Leverage Opportunities Unleashing Success and Transformation</em></sub></p>

> _Public gists are linked individually above as they ship. For private work-in-progress and operational forensics, see [LinkedIn](https://www.linkedin.com/in/davidmirelesll/?locale=es_ES) for the curated view._

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider.svg" width="100%" alt="divider"/></p>

<!-- ============================================================ -->
<!-- FOOTER: animated squares grid + tagline (no operator name).  -->
<!-- Served from profile-public static/ alongside the section     -->
<!-- banners. Editor-only provenance; GitHub strips the comment.  -->
<!-- ============================================================ -->
<div align="center">
  <img alt="Animated footer tagline" src="https://raw.githubusercontent.com/louzt/louzt/main/static/profile-footer.svg" width="100%" style="display:block;margin:0 auto"/>
</div>
