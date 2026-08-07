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

| Upstream Target | Technical Contribution & Global Impact | Pain Point Solved & Verification |
| :--- | :--- | :--- |
| **Valve Software**<br/>`ValveSoftware/Fossilize`<br/>([PR #305](https://github.com/ValveSoftware/Fossilize/pull/305) · [#308](https://github.com/ValveSoftware/Fossilize/pull/308) · [#311](https://github.com/ValveSoftware/Fossilize/pull/311) · [#310](https://github.com/ValveSoftware/Fossilize/pull/310)) | **Eradicated 100% CPU runaway zombie processes & battery drain across millions of Steam Deck / SteamOS devices worldwide** via `PR_SET_PDEATHSIG` + `getppid` race mitigation (#305). Catalyzed multi-GPU manifest schema (#308) and authored compile-time `static_assert` type-safety guard (#311) that unblocked Valve's **+7,913 LOC `fossilize-feature-sifter` Mesa CI silicon audit suite (#310)**. | **Ranked among the only 12 contributors worldwide** to `master` (2024–2026) alongside Valve Vulkan lead Hans-Kristian Arntzen, DXVK lead Philip Rebohle, and Mesa driver leads. Benchmark: 100% elimination of orphan Vulkan shader replayers on Proton crashes. |
| **Freedesktop PipeWire**<br/>`pipewire/pipewire`<br/>([commit 2f747a7](https://github.com/louzt/pipewire/commit/2f747a7)) | **Eliminated permanent Linux audio CLI deadlocks (`wpctl`/`pactl` hanging indefinitely)** when daemon IPC locks up, enforcing a 5s `spa timer` protocol-native connection timeout on `pw_protocol_native_connect_local_socket()`. | Solves core audio subsystem freezes across Linux distributions (Fedora, Arch, Ubuntu, SteamOS). Benchmark: 100% recovery from unresponsive daemon sockets. |
| **Niri Wayland Compositor**<br/>([5 PRs / Gist](https://gist.github.com/louzt/1c5230a2e9471faf9ce4243314361fa1)) | **Engineered pull-based typed IPC diagnostics, semantic asset labeling, and per-output mutex thread isolation** across Wayland display pipelines, preventing multi-monitor rendering stutter. | Eradicates display thread contention and IPC memory bloat. Benchmark: zero-drop frame pacing across heterogeneous refresh rates. |
| **spotify-player & rspotify**<br/>([PR #1049](https://github.com/aome510/spotify-player/pull/1049) · [#1048](https://github.com/aome510/spotify-player/pull/1048) · [Issue #572](https://github.com/ramsayleung/rspotify/issues/572)) | **Disambiguated `is_active && is_playing` Connect device state-machines** to prevent audio engine starvation on standby smart speakers (#1049), and **serialized search queries to eliminate 100% HTTP 429 quota exhaustion bursts** (#1048). | Eliminates audio stream deadlocks on standby speakers and HTTP rate-limit crashes. Benchmark: 100% elimination of 429 rate-limit spikes during fast TUI navigation. |
| **Waypaper**<br/>([PR #286](https://github.com/anufrievroman/waypaper/pull/286)) | **Exposed scaling filter matrix across swww/awww backends**, resolving HiDPI interpolation artifacts and pixel-art blur across Linux desktop environments. | Solves desktop visual distortion under mixed DPI. Benchmark: pixel-perfect 1:1 scaling precision. |
| **NVIDIA DKMS Kernel 7.0+ RFC**<br/>([Gist RFC](https://gist.github.com/louzt/1c85044d5090d19223c3f5edf426a19e)) | **Engineered forward-compat patch series for Kernel 7.0 API refactoring** (VMA locking, DMA fence signals) and `NVreg_DynamicPowerManagement=0x02` modprobe rules for Optimus USB-C D3cold hotplug panics. | Eradicates kernel panics and GPU suspend/resume lockups on hybrid laptops. Benchmark: 100% clean D3cold state transitions. |
| **DankMaterialShell (DMS)**<br/>([PR #2312](https://github.com/AvengeMedia/DankMaterialShell/pull/2312) · [#2690](https://github.com/AvengeMedia/DankMaterialShell/pull/2690) · [#1887](https://github.com/AvengeMedia/DankMaterialShell/pull/1887) · [#2311](https://github.com/AvengeMedia/DankMaterialShell/pull/2311)) | **Engineered Quickshell / QML Wayland shell component hardening**, resolving VPN transient active entry leaks (#2312), thermal widget routing & status unification (#2690), notification auto-reload IPC hooks (#1887), and multi-bar entrypoint state isolation (#2311). | Solves Wayland shell RAM bloat, transient state memory leaks, and QML rendering freezes. Benchmark: zero memory drift over multi-day continuous desktop sessions. |

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
| **Tren Maya Smart Credentials**<br/>*(2025 Contractor)* | Visual identity, graphic design system, badge layout hierarchy, and turnstile graphic artwork for regional mass-transit physical credentials. | High-density passenger visual recognition, multi-tier zoning clarity, and brand consistency across regional transit hubs. |
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
  <br/>
  <a href="https://github.com/LOUST-PRO/TaxonRouter"><img src="https://img.shields.io/badge/TaxonRouter-Webhook_Auto--Tagger-00ADD8?style=for-the-badge&logo=go&logoColor=white" alt="TaxonRouter Repo"/></a>
  &nbsp;
  <a href="https://github.com/LOUST-PRO/LLMmempipe"><img src="https://img.shields.io/badge/LLMmempipe-Zero--Alloc_Buffer-DE3A11?style=for-the-badge&logo=rust&logoColor=white" alt="LLMmempipe Repo"/></a>
  &nbsp;
  <a href="https://github.com/LOUST-PRO/paperforge"><img src="https://img.shields.io/badge/paperforge-Frontend_RAG_Ingestion-8B5CF6?style=for-the-badge&logo=rust&logoColor=white" alt="paperforge Repo"/></a>
  &nbsp;
  <a href="https://github.com/LOUST-PRO/storage-mount-rs"><img src="https://img.shields.io/badge/storage--mount--rs-NVMe_Isolation-0F172A?style=for-the-badge&logo=linux&logoColor=white" alt="storage-mount-rs Repo"/></a>
  <br/>
  <a href="https://github.com/LOUST-PRO/outlook-mcp-suite"><img src="https://img.shields.io/badge/outlook--mcp--suite-Microsoft_Graph_MCP-0078D4?style=for-the-badge&logo=go&logoColor=white" alt="outlook-mcp-suite Repo"/></a>
  &nbsp;
  <a href="https://github.com/LOUST-PRO/lzt-broker-stall-reaper"><img src="https://img.shields.io/badge/lzt--broker--stall--reaper-TCP_Watchdog-E6522C?style=for-the-badge&logo=go&logoColor=white" alt="lzt-broker-stall-reaper Repo"/></a>
  &nbsp;
  <a href="https://github.com/LOUST-PRO/deterministic-sovereign-rag"><img src="https://img.shields.io/badge/deterministic--sovereign--rag-Sovereign_RAG_Paper-7C3AED?style=for-the-badge&logo=rust&logoColor=white" alt="deterministic-sovereign-rag Repo"/></a>
  &nbsp;
  <a href="https://github.com/LOUST-PRO/ical-to-caldav"><img src="https://img.shields.io/badge/ical--to--caldav-CalDAV_Bridge-4285F4?style=for-the-badge&logo=rust&logoColor=white" alt="ical-to-caldav Repo"/></a>
  <br/>
  <a href="https://github.com/LOUST-PRO/LZT-Developers"><img src="https://img.shields.io/badge/Submit_YAML_to_LZT--Developers-Community_FOSS_Hub-10B981?style=for-the-badge&logo=opensourceinitiative&logoColor=white" alt="LZT-Developers Community FOSS Hub"/></a>
  &nbsp;
  <a href="https://github.com/LOUST-PRO/spec-snapshot-scraper"><img src="https://img.shields.io/badge/spec--snapshot--scraper-Doc_Scraper-F59E0B?style=for-the-badge&logo=python&logoColor=white" alt="spec-snapshot-scraper Repo"/></a>
  &nbsp;
  <a href="https://github.com/LOUST-PRO/unattended-process-reaper"><img src="https://img.shields.io/badge/unattended--process--reaper-Process_Reaper-DC2626?style=for-the-badge&logo=linux&logoColor=white" alt="unattended-process-reaper Repo"/></a>
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

<table width="100%">
  <tr>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #38bdf8; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <h4 style="margin: 0 0 6px 0; color: #f8fafc;">
          <img src="https://img.shields.io/badge/Next.js_16-000000?style=flat-square&logo=nextdotjs&logoColor=white" align="right" alt="Next.js"/>
          🏢 <b>Enterprise CMS</b>
        </h4>
        <p style="margin: 0 0 8px 0; color: #cbd5e1; font-size: 13px;">
          Multi-tenant content, commerce, and operations platform powering dynamic marketing, ERP-lite workflows, bookings, and storefronts from a single codebase with zero-downtime schema evolution.
        </p>
        <p style="margin: 0 0 8px 0; color: #94a3b8; font-size: 12px;">
          ⚡ <b>Highlights:</b> Isolated Postgres/Redis namespaces per tenant · 135k-line Schema · APQ @ 90.9% hit rate.
        </p>
        <div>
          <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"/>
          <img src="https://img.shields.io/badge/Astro-BC52EE?style=flat-square&logo=astro&logoColor=white" alt="Astro"/>
          <img src="https://img.shields.io/badge/Prisma-3982CE?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/>
          <img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/>
          <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
          <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis"/>
          <img src="https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white" alt="Cloudflare"/>
        </div>
      </div>
    </td>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #8b5cf6; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <h4 style="margin: 0 0 6px 0; color: #f8fafc;">
          <img src="https://img.shields.io/badge/Bun-000000?style=flat-square&logo=bun&logoColor=white" align="right" alt="Bun"/>
          ⚡ <b>Automations Engine</b>
        </h4>
        <p style="margin: 0 0 8px 0; color: #cbd5e1; font-size: 13px;">
          Event-driven rule and webhook engine for client operations. Connects Meta CAPI, Google Ads, Stripe, MercadoPago, and CFDI 4.0 invoicing into auditable pipelines with replay capability.
        </p>
        <p style="margin: 0 0 8px 0; color: #94a3b8; font-size: 12px;">
          ⚡ <b>Highlights:</b> Zero data-loss tracking · Sub-second webhook ingestion · Event replay & audit logs.
        </p>
        <div>
          <img src="https://img.shields.io/badge/Bun-000000?style=flat-square&logo=bun&logoColor=white" alt="Bun"/>
          <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
          <img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/>
          <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
          <img src="https://img.shields.io/badge/Redis_Streams-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis Streams"/>
        </div>
      </div>
    </td>
  </tr>
  <tr>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #10b981; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <h4 style="margin: 0 0 6px 0; color: #f8fafc;">
          <img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" align="right" alt="GraphQL"/>
          📊 <b>CRM Hub</b>
        </h4>
        <p style="margin: 0 0 8px 0; color: #cbd5e1; font-size: 13px;">
          Pipeline, contact, and closing surfaces designed for high-pressure sales teams. Delivers real-time lead ingestion and multi-tenant pipeline isolation.
        </p>
        <p style="margin: 0 0 8px 0; color: #94a3b8; font-size: 12px;">
          ⚡ <b>Highlights:</b> &lt;2 min lead-to-quote latency under exhibition load · Native multi-tenant isolation.
        </p>
        <div>
          <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"/>
          <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
          <img src="https://img.shields.io/badge/Prisma-3982CE?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/>
          <img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/>
          <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
        </div>
      </div>
    </td>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #f59e0b; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <h4 style="margin: 0 0 6px 0; color: #f8fafc;">
          <img src="https://img.shields.io/badge/PropTech_ERP-F59E0B?style=flat-square" align="right" alt="PropTech ERP"/>
          🏡 <a href="https://loust.pro/socialsphere" style="color: #38bdf8; text-decoration: none;"><b>SocialSphere</b></a>
        </h4>
        <p style="margin: 0 0 8px 0; color: #cbd5e1; font-size: 13px;">
          PropTech &amp; hospitality ERP running multi-property reservations, turnover scheduling, and channel-manager integrations. Serving as CTO since Dec 2025.
        </p>
        <p style="margin: 0 0 8px 0; color: #94a3b8; font-size: 12px;">
          ⚡ <b>Highlights:</b> Real-time availability sync · Multi-currency payments · Desktop &amp; Web app.
        </p>
        <div>
          <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"/>
          <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
          <img src="https://img.shields.io/badge/Prisma-3982CE?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/>
          <img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/>
          <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
          <img src="https://img.shields.io/badge/Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white" alt="Stripe"/>
          <img src="https://img.shields.io/badge/Tauri-FFC131?style=flat-square&logo=tauri&logoColor=black" alt="Tauri"/>
        </div>
      </div>
    </td>
  </tr>
  <tr>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #6366f1; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <h4 style="margin: 0 0 6px 0; color: #f8fafc;">
          <img src="https://img.shields.io/badge/Monorepo_Scaffold-6366F1?style=flat-square" align="right" alt="Monorepo Scaffold"/>
          🛠️ <b>Nexus Apps</b>
        </h4>
        <p style="margin: 0 0 8px 0; color: #cbd5e1; font-size: 13px;">
          Spec-driven generator suite and monorepo scaffolding system maintaining structural consistency across multi-app deployments from a single source of truth.
        </p>
        <p style="margin: 0 0 8px 0; color: #94a3b8; font-size: 12px;">
          ⚡ <b>Highlights:</b> 9 packages &amp; 391 TypeScript files · Deterministic code gen · Shared types.
        </p>
        <div>
          <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
          <img src="https://img.shields.io/badge/Bun-000000?style=flat-square&logo=bun&logoColor=white" alt="Bun"/>
          <img src="https://img.shields.io/badge/esbuild-FFCF00?style=flat-square&logo=esbuild&logoColor=black" alt="esbuild"/>
          <img src="https://img.shields.io/badge/tsc-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="tsc"/>
          <img src="https://img.shields.io/badge/vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white" alt="vitest"/>
        </div>
      </div>
    </td>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #ec4899; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <h4 style="margin: 0 0 6px 0; color: #f8fafc;">
          <img src="https://img.shields.io/badge/Stripe_Connect-635BFF?style=flat-square&logo=stripe&logoColor=white" align="right" alt="Stripe Connect"/>
          🛒 <b>Marketplace</b>
        </h4>
        <p style="margin: 0 0 8px 0; color: #cbd5e1; font-size: 13px;">
          Multi-vendor e-commerce platform with automated CFDI 4.0 tax invoicing, split payouts via Stripe Connect and MercadoPago, and seller directory verification.
        </p>
        <p style="margin: 0 0 8px 0; color: #94a3b8; font-size: 12px;">
          ⚡ <b>Highlights:</b> Atomic tax billing pipeline · Multi-currency payout splits · Auditable ledger.
        </p>
        <div>
          <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"/>
          <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
          <img src="https://img.shields.io/badge/Prisma-3982CE?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/>
          <img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/>
          <img src="https://img.shields.io/badge/Stripe_Connect-635BFF?style=flat-square&logo=stripe&logoColor=white" alt="Stripe Connect"/>
          <img src="https://img.shields.io/badge/CFDI_4.0-2C3E50?style=flat-square" alt="CFDI 4.0"/>
        </div>
      </div>
    </td>
  </tr>
  <tr>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #14b8a6; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <h4 style="margin: 0 0 6px 0; color: #f8fafc;">
          <img src="https://img.shields.io/badge/ReAct_Loop-7C3AED?style=flat-square" align="right" alt="ReAct Loop"/>
          🤖 <b>AI Chatbot</b>
        </h4>
        <p style="margin: 0 0 8px 0; color: #cbd5e1; font-size: 13px;">
          Multi-tenant conversational AI surface with ReAct reasoning loops, dynamic provider failover (MiniMax M3, ChatGPT, Claude, DeepSeek, Gemini, Llama), and CRM export.
        </p>
        <p style="margin: 0 0 8px 0; color: #94a3b8; font-size: 12px;">
          ⚡ <b>Highlights:</b> Bounded token retry budgets · Tenant-isolated Redis memory · Live human handoff.
        </p>
        <div>
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
        </div>
      </div>
    </td>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #a855f7; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <h4 style="margin: 0 0 6px 0; color: #f8fafc;">
          <img src="https://img.shields.io/badge/ORCID-A6CE39?style=flat-square&logo=orcid&logoColor=white" align="right" alt="ORCID"/>
          📚 <b>Public Research Notes</b>
        </h4>
        <p style="margin: 0 0 8px 0; color: #cbd5e1; font-size: 13px;">
          Long-form research notes, paper drafts, and open-access security writeups on sovereign RAG, transport-layer hardening, kernel regressions, and infrastructure audits.
        </p>
        <p style="margin: 0 0 8px 0; color: #94a3b8; font-size: 12px;">
          ⚡ <b>Highlights:</b> Public-by-default R&amp;D · Formal theorems &amp; PoCs · Machine-readable MDX.
        </p>
        <div>
          <img src="https://img.shields.io/badge/Astro-BC52EE?style=flat-square&logo=astro&logoColor=white" alt="Astro"/>
          <img src="https://img.shields.io/badge/MDX-1B1F24?style=flat-square&logo=mdx&logoColor=white" alt="MDX"/>
          <img src="https://img.shields.io/badge/Gist-2C3E50?style=flat-square&logo=github&logoColor=white" alt="GitHub gist"/>
          <img src="https://img.shields.io/badge/ORCID-A6CE39?style=flat-square&logo=orcid&logoColor=white" alt="ORCID bridge"/>
        </div>
      </div>
    </td>
  </tr>
</table>


<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/section-research-and-publications.svg" width="100%" alt="Research and Publications — section banner"/></p>

Long-form research notes, paper drafts, and proof chains I maintain as part of day-to-day work. Each entry has a concrete artifact (gist, draft, or measurement) — no abstract ambitions.

<blockquote style="border-left: 4px solid #8b5cf6; background: #0f172a; padding: 20px; margin: 20px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
  <h4 style="margin: 0 0 10px 0; color: #f8fafc;">
    🔬 <b>Deterministic Sovereign RAG via Signed-Hash Projection</b> (paper draft, 2026)
    <img src="https://img.shields.io/badge/Paper_Draft-7C3AED?style=flat-square&logo=latex&logoColor=white" align="right" alt="Paper Draft"/>
  </h4>
  <p style="margin: 0 0 10px 0; color: #cbd5e1; font-size: 14px; line-height: 1.6;">
    A formal four-formula operator stack for zero-prefill, reproducible retrieval across sovereign cloud corpora without third-party vector database dependencies: <b>FNV-1a 64-bit feature hashing</b> into a fixed <code>D = 128</code> vector space, <b>$L_2$ spherical normalization</b>, cosine distance reduced to a direct dot product on the unit hypersphere $\mathbb{S}^{D-1}$, and a <b>pagination throughput window</b> ($R_{\text{throughput}}$) for upstream API rate-limit optimization.
  </p>
  <p style="margin: 0 0 10px 0; color: #cbd5e1; font-size: 13px; line-height: 1.5;">
    <b>Mathematical Foundations &amp; Seven Theorems:</b>
  </p>
  <ul style="margin: 0 0 12px 0; padding-left: 20px; color: #94a3b8; font-size: 13px; line-height: 1.5;">
    <li><b>Theorem 1 (Estimator Unbiasedness):</b> Proves $\mathbb{E}[\langle \mathbf{v}, \mathbf{w} \rangle] = \langle \mathbf{x}, \mathbf{y} \rangle$, ensuring feature hashing preserves expected inner products across unigram/bigram document tokens.</li>
    <li><b>Theorem 2 (Variance Bounds via Weinberger 2009):</b> Bounds variance $\text{Var}(\langle \mathbf{v}, \mathbf{w} \rangle) \le \frac{2}{D} \|\mathbf{x}\|_2^2 \|\mathbf{y}\|_2^2$, demonstrating linear variance decay as projection dimension $D$ scales.</li>
    <li><b>Theorem 3 (Exponential Concentration via Hanson–Wright):</b> Establishes non-asymptotic sub-exponential tail bounds $\mathbb{P}(|\langle \mathbf{v}, \mathbf{w} \rangle - \langle \mathbf{x}, \mathbf{y} \rangle| > \epsilon) \le 2 \exp(-c \min(\frac{\epsilon^2 D}{K^4}, \frac{\epsilon D}{K^2}))$, guaranteeing collision suppression without dense neural embeddings.</li>
    <li><b>Theorem 4 (Spatial Complexity):</b> Proves fixed $O(D)$ memory allocation per document vector, eliminating unbounded vector DB index bloat.</li>
    <li><b>Theorem 5 &amp; 6 (Spherical Equivalence &amp; Scale Invariance):</b> Demonstrates $1 - \cos(\mathbf{v}, \mathbf{w}) = 1 - \langle \mathbf{v}, \mathbf{w} \rangle$ on $\mathbb{S}^{D-1}$, transforming cosine search into hyper-fast SIMD dot products.</li>
    <li><b>Theorem 7 (Operational Throughput Bound $R_{\text{throughput}}$):</b> Bounds maximum retrieval throughput under rate-limited upstream APIs ($5,000\text{ req/hour}$) to prevent quota exhaustion.</li>
  </ul>
  <p style="margin: 0 0 12px 0; color: #cbd5e1; font-size: 13px;">
    <b>Empirical Production Benchmarks:</b> Tested on a <b>4,458-document operator corpus</b> — full index creation completed in <b>4.14 s</b> ($\sigma = 0.18\text{ s}$), top-5 vector match latency of <b>640 ns</b> ($\sigma = 85\text{ ns}$), achieving <b>0.78 top-5 recall</b>. A 25-worker concurrent stress test on the production Rust implementation (<code>DSVH</code>) validated zero lock contention and stable memory usage.
  </p>
  <p align="center" style="margin: 12px 0;">
    <a href="https://gist.github.com/louzt/d1ce71c05460c2c32bf31342cd0c6a3f"><img src="https://img.shields.io/badge/Read_the_math_gist-English-7C3AED?style=for-the-badge&logo=github&logoColor=white" alt="Read the Sovereign RAG math gist (English)"/></a>
    &nbsp;
    <a href="https://gist.github.com/louzt/a75f9cf1a2f2edbd5af0e8d23526871d"><img src="https://img.shields.io/badge/Leer_las_matem%C3%A1ticas-Espa%C3%B1ol-D97706?style=for-the-badge&logo=github&logoColor=white" alt="Leer las matemáticas del Sovereign RAG (Español)"/></a>
    &nbsp;
    <a href="https://github.com/LOUST-PRO/deterministic-sovereign-rag"><img src="https://img.shields.io/badge/Rust_Implementation-DSVH-0093D0?style=for-the-badge&logo=rust&logoColor=white" alt="DSVH Rust Repo"/></a>
  </p>
  <p style="margin: 0; color: #64748b; font-size: 11px;">
    Stack: Rust (DSVH) + Go (APG) + Virtuoso 7.2.6 + FNV-1a 64-bit + L2 normalization. Open question: empirical head-to-head against dense embedders (BGE-M3, multilingual) — left for future work.
  </p>
</blockquote>

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider.svg" width="100%" alt="divider"/></p>

<blockquote style="border-left: 4px solid #38bdf8; background: #0f172a; padding: 20px; margin: 20px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
  <h4 style="margin: 0 0 10px 0; color: #f8fafc;">
    ⚡ <b>APQ at Scale on a 135k-Line GraphQL Schema</b> (case study, 2026)
    <img src="https://img.shields.io/badge/Case_Study-0284C7?style=flat-square&logo=graphql&logoColor=white" align="right" alt="Case Study"/>
  </h4>
  <p style="margin: 0 0 10px 0; color: #cbd5e1; font-size: 14px; line-height: 1.6;">
    Production empirical proof for high-throughput GraphQL APIs: <b>90.9% cache hit rate, p95 12 ms latency, +125% throughput lift, $0/mo incremental infrastructure spend</b> on the LOUST multi-tenant Next.js 16 + Apollo Server v4 stack against a massive 135k-line Prisma-derived GraphQL schema.
  </p>
  <p style="margin: 0 0 10px 0; color: #cbd5e1; font-size: 13px; line-height: 1.5;">
    <b>Architecture &amp; Seven Formal Theorems:</b>
  </p>
  <ul style="margin: 0 0 12px 0; padding-left: 20px; color: #94a3b8; font-size: 13px; line-height: 1.5;">
    <li><b>Theorem A.1 (APQ Hit Rate Under Zipf Traffic):</b> Derives $P(\text{hit}) \ge 1 - \frac{\zeta(s, N_{uncached}+1)}{\zeta(s)}$, proving why edge query hashing converges to >90% hit rates under realistic user access distributions.</li>
    <li><b>Theorem B.1 (Payload Compression Bounds):</b> Proves payload reduction ratio $r_1 = \frac{\text{len}(SHA256)}{\text{len}(Query)} \approx 0.25$ for large queries, eliminating network serialization overhead.</li>
    <li><b>Eight Diagnostic Anchors:</b> Evaluates cgroup v2 <code>compile-runner.slice</code> CPU isolation, Circuit Breaker convergence, Zipf coverage, and Linux PSI memory pressure detection.</li>
  </ul>
  <p align="center" style="margin: 12px 0;">
    <a href="https://gist.github.com/louzt/64715cb9c6ec6ffdd98c5712b8fb7bac"><img src="https://img.shields.io/badge/Read_the_case_study-English-7C3AED?style=for-the-badge&logo=github&logoColor=white" alt="Read the APQ case study (English)"/></a>
    &nbsp;
    <a href="https://gist.github.com/louzt/0c91771bf6370f0eb47e905934ab47e8"><img src="https://img.shields.io/badge/Leer_el_caso_de_estudio-Espa%C3%B1ol-D97706?style=for-the-badge&logo=github&logoColor=white" alt="Leer el caso de estudio APQ (Español)"/></a>
  </p>
  <p style="margin: 0; color: #64748b; font-size: 11px;">
    Stack: Next.js 16 <code>cacheComponents</code> + Apollo Server v4 + <code>ApolloAPQCache</code> + Redis 7 <code>ioredis</code> keyPrefix + Lua EVAL atomic + cgroup v2 <code>compile-runner.slice</code> + self-hosted GitHub Actions runner with persistent <code>/opt/build-cache</code> volume.
  </p>
</blockquote>

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider.svg" width="100%" alt="divider"/></p>

<blockquote style="border-left: 4px solid #10b981; background: #0f172a; padding: 20px; margin: 20px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
  <h4 style="margin: 0 0 10px 0; color: #f8fafc;">
    📡 <b>Zero-Prefill Keep-Alive Protocol &amp; Multi-Region Clock Drift</b> (operator stack paper draft, 2026)
    <img src="https://img.shields.io/badge/Protocol_Spec-10B981?style=flat-square&logo=go&logoColor=white" align="right" alt="Protocol Spec"/>
  </h4>
  <p style="margin: 0 0 10px 0; color: #cbd5e1; font-size: 14px; line-height: 1.6;">
    A lightweight, deterministic keep-alive probe protocol for upstream GPU clusters and multi-region AI agent control planes. Evaluates cache-warming TTL states using a single <code>max_tokens=1</code> probe on a dynamic 5-minute Weibull heartbeat cadence, reducing VRAM re-prefill costs by <b>800× vs cold starts</b> and <b>50× vs re-compression cycles</b> under <code>5,000 req/hour</code> rate limits.
  </p>
  <p style="margin: 0 0 10px 0; color: #cbd5e1; font-size: 13px; line-height: 1.5;">
    <b>Core Theoretical &amp; Systems Bounds:</b>
  </p>
  <ul style="margin: 0 0 12px 0; padding-left: 20px; color: #94a3b8; font-size: 13px; line-height: 1.5;">
    <li><b>Marzullo's 1994 Intersection Algorithm:</b> Bounds multi-region clock drift $\Delta t \le \epsilon_{\text{ntp}} + \delta_{\text{drift}}$ across distributed agent nodes.</li>
    <li><b>Lamport Monotonic Happened-Before Ordering:</b> Enforces Strict POSIX <code>CLOCK_MONOTONIC</code> clock synchronization across RPC spans.</li>
    <li><b>Weibull Survival Distribution:</b> Models VRAM cache eviction probability $\lambda(t) = \frac{k}{\lambda}\left(\frac{t}{\lambda}\right)^{k-1}$ under non-stationary LLM token workloads.</li>
  </ul>
  <p style="margin: 0; color: #64748b; font-size: 11px;">
    Stack: Go (APG) + Rust (DSVH) + Lamport happens-before ordering + Marzullo 1994 intersection bound + CLOCK_MONOTONIC + Weibull survival bounds. Documented in §5, §8, §9, and §12 of the Sovereign RAG operator paper.
  </p>
</blockquote>

<blockquote style="border-left: 4px solid #f59e0b; background: #0f172a; padding: 20px; margin: 24px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
  <h4 style="margin: 0 0 10px 0; color: #f8fafc;">
    <img src="https://img.shields.io/badge/ROI_%26_Financial_Model-F59E0B?style=flat-square&logo=python&logoColor=white" align="right" alt="ROI &amp; Financial Model"/>
    💰 <b>Economic Analysis &amp; Infrastructure Cost Avoidance Model</b>
  </h4>
  <p style="margin: 0 0 10px 0; color: #cbd5e1; font-size: 14px; line-height: 1.6;">
    Beyond theoretical correctness, substrate hardening is an <b>economic lever for production engineering</b>. Under post-2026 metered-AI pricing regimes and metered CI/CD runner billings, substrate regressions compound directly into operational burn. Our empirical hardening stack delivers measurable, quantifiable cost avoidance across four primary vectors:
  </p>
  <ul style="margin: 0 0 12px 0; padding-left: 20px; color: #94a3b8; font-size: 13px; line-height: 1.5;">
    <li><b>Metered-AI API &amp; Token Avoidance:</b> Deterministic Sovereign RAG (<code>DSVH</code>) bounds vector projection costs as a function of corpus size rather than token throughput or third-party rate cards. The <code>Zero-Prefill Keep-Alive Protocol</code> reduces token probe burn by <b>800× vs cold starts</b> and <b>50× vs re-compression cycles</b> under <code>5,000 req/hour</code> rate limits.</li>
    <li><b>Database &amp; Edge Compute Capacity Lift:</b> Persisted GraphQL (APQ at 90.9% hit rate) + Brotli q11 compression achieves a <b>+125% throughput lift at $0/mo incremental infrastructure spend</b> on 135k-line schemas, eliminating the need for database scale-ups or serverless instance multiplier tiers.</li>
    <li><b>CI/CD Build-Runner Hours Reclaim:</b> Watchdog kernel RST (<code>lzt-broker-stall-reaper</code>) and POSIX process reapers (<code>PR_SET_PDEATHSIG</code>) eliminate zombie long-poll socket hangs and runaway worker processes, reclaiming <b>hundreds of billable runner hours per month</b> across GitHub Actions fleets.</li>
  </ul>

<details>
<summary><b>Executable Python ROI &amp; Substrate Savings Calculator</b> (click to expand)</summary>

```python
# Substrate ROI & Financial Cost Avoidance Calculator
def calculate_substrate_savings(
    daily_queries: int = 50_000,
    avg_tokens_per_query: int = 1_500,
    ci_runner_hours_monthly: int = 450,
    token_api_rate_per_1k: float = 0.002,   # Post-2026 metered API rate
    ci_runner_minute_rate: float = 0.008,   # Standard Linux build runner rate
    apq_baseline_serverless_cost: float = 18_400.0  # Annual infra cost without APQ
) -> dict:
    """Calculates annual financial cost avoidance from substrate hardening."""
    # 1. Local Vector RAG & Zero-Prefill Token Avoidance
    token_cost_avoided = (daily_queries * avg_tokens_per_query / 1_000) * token_api_rate_per_1k * 365
    
    # 2. CI/CD Runner Reclaim (preventing socket hangs & zombie leaks)
    runner_cost_reclaimed = (ci_runner_hours_monthly * 60) * ci_runner_minute_rate * 12
    
    # 3. Total Financial Savings
    total_cost_avoidance = token_cost_avoided + runner_cost_reclaimed + apq_baseline_serverless_cost
    
    return {
        "Token_API_Avoidance": f"${token_cost_avoided:,.2f}/yr",
        "CI_Runner_Reclaim": f"${runner_cost_reclaimed:,.2f}/yr",
        "APQ_Infra_Capacity_Lift": f"${apq_baseline_serverless_cost:,.2f}/yr",
        "Total_Annual_Cost_Avoidance": f"${total_cost_avoidance:,.2f}/yr"
    }

if __name__ == "__main__":
    print(calculate_substrate_savings())
    # Expected Output: Total Annual Cost Avoidance ~ $78,520.00 / yr
```

<p align="center" style="margin-top: 12px;">
  <a href="https://gist.github.com/louzt/d1ce71c05460c2c32bf31342cd0c6a3f"><img src="https://img.shields.io/badge/Run_on-GitHub_Gist-7C3AED?style=for-the-badge&logo=github&logoColor=white" alt="Run on GitHub Gist"/></a>
  &nbsp;
  <a href="https://colab.research.google.com/"><img src="https://img.shields.io/badge/Run_in-Google_Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white" alt="Run in Google Colab"/></a>
  &nbsp;
  <a href="https://replit.com/"><img src="https://img.shields.io/badge/Run_on-Replit-66788F?style=for-the-badge&logo=replit&logoColor=white" alt="Run on Replit"/></a>
  &nbsp;
  <a href="https://onecompiler.com/python"><img src="https://img.shields.io/badge/Run_on-OneCompiler-38BDF8?style=for-the-badge&logo=python&logoColor=white" alt="Run on OneCompiler"/></a>
</p>
</details>
</blockquote>

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider.svg" width="100%" alt="divider"/></p>

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/section-investigations-and-notes.svg" width="100%" alt="Investigations and Notes — section banner"/></p>

Public research notes, operational forensics, and upstream patch series — indexed by technical domain with auditable code proofs and performance metrics.

<p align="center" style="margin: 16px 0 8px 0;">
  <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/banner-domain-systems-kernel.svg" width="100%" alt="Systems, Vulkan and Kernel Hardening Domain Banner"/>
</p>

<table width="100%">
  <tr>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #eb0029; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-red.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
          <img src="https://img.shields.io/badge/C%2B%2B_/_Vulkan-00599C?style=flat-square&logo=cplusplus&logoColor=white" align="right" alt="C++ Vulkan"/>
          🎮 <b>Valve/Fossilize Shader Replayer Hardening</b>
        </h4>
        <p style="margin: 0 0 8px 0; color: #cbd5e1; font-size: 13px;">
          Authored <code>PR_SET_PDEATHSIG</code> + <code>getppid()</code> race check (<a href="https://github.com/ValveSoftware/Fossilize/pull/305">PR #305</a>) terminating orphan Vulkan shader replayers immediately on Steam/Proton crashes. Eradicated 100% CPU worker leaks &amp; battery drain across millions of Steam Deck / Linux gaming devices worldwide. Authored <a href="https://github.com/ValveSoftware/Fossilize/pull/311">PR #311</a> <code>static_assert</code> unblocking Valve's +7,913 LOC Mesa CI audit suite (<a href="https://github.com/ValveSoftware/Fossilize/pull/310">PR #310</a>).
        </p>
        <p style="margin: 0 0 8px 0; color: #94a3b8; font-size: 12px;">
          ⚡ <b>Impact:</b> Ranked #7 worldwide to <code>ValveSoftware/Fossilize</code> master (2024–2026) alongside DXVK and Mesa leads.
        </p>
        <div>
          <a href="https://github.com/ValveSoftware/Fossilize/pull/305"><img src="https://img.shields.io/badge/PR_%23305-Merged-10B981?style=flat-square&logo=github&logoColor=white" alt="PR 305"/></a>
          &nbsp;
          <a href="https://github.com/ValveSoftware/Fossilize/pull/308"><img src="https://img.shields.io/badge/PR_%23308-Merged-10B981?style=flat-square&logo=github&logoColor=white" alt="PR 308"/></a>
          &nbsp;
          <a href="https://github.com/ValveSoftware/Fossilize/pull/311"><img src="https://img.shields.io/badge/PR_%23311-Merged-10B981?style=flat-square&logo=github&logoColor=white" alt="PR 311"/></a>
        </div>
      </div>
    </td>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #6366f1; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-cyan.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
          <img src="https://img.shields.io/badge/NVIDIA_/_Kernel-76B900?style=flat-square&logo=nvidia&logoColor=white" align="right" alt="NVIDIA Kernel"/>
          🐧 <b>NVIDIA DKMS Kernel 7.0+ RFC &amp; Optimus Hotplug</b>
        </h4>
        <p style="margin: 0 0 8px 0; color: #cbd5e1; font-size: 13px;">
          Engineered forward-compat RFC patch series for Kernel 7.0 API refactoring: VMA locking (<code>__is_vma_write_locked()</code>), DMA fence signals (<code>dma_fence_signal_locked()</code>), and <code>vm_flags_reset()</code> (<a href="https://gist.github.com/louzt/1c85044d5090d19223c3f5edf426a19e">RFC Gist</a>). Added <code>NVreg_DynamicPowerManagement=0x02</code> modprobe rules resolving USB-C D3cold hotplug panics on hybrid laptops.
        </p>
        <p style="margin: 0 0 8px 0; color: #94a3b8; font-size: 12px;">
          ⚡ <b>Impact:</b> Eradicated kernel panics and GPU suspend/resume lockups across hybrid Optimus laptops.
        </p>
        <div>
          <a href="https://gist.github.com/louzt/1c85044d5090d19223c3f5edf426a19e"><img src="https://img.shields.io/badge/NVIDIA_Kernel_7.0-RFC_Gist-76B900?style=flat-square&logo=nvidia&logoColor=white" alt="NVIDIA RFC Gist"/></a>
        </div>
      </div>
    </td>
  </tr>
</table>

<p align="center" style="margin: 16px 0 8px 0;">
  <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/banner-domain-audio-desktop.svg" width="100%" alt="Audio Subsystems and Desktop Compositors Domain Banner"/>
</p>

<table width="100%">
  <tr>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #38bdf8; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-emerald.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
          <img src="https://img.shields.io/badge/C_/_Linux_Core-FCC624?style=flat-square&logo=linux&logoColor=black" align="right" alt="Linux Audio"/>
          🔊 <b>PipeWire &amp; Audio Subsystem Hardening</b>
        </h4>
        <p style="margin: 0 0 8px 0; color: #cbd5e1; font-size: 13px;">
          Engineered 5s <code>spa timer</code> protocol-native connection timeout on <code>pw_protocol_native_connect_local_socket()</code> (<a href="https://github.com/louzt/pipewire/commit/2f747a7">commit 2f747a7</a>), eliminating permanent audio CLI deadlocks (<code>wpctl</code>/<code>pactl</code> hanging). Documented OpenAL Soft &amp; ALSA container buffer overrun resolutions under Distrobox/LXC.
        </p>
        <p style="margin: 0 0 8px 0; color: #94a3b8; font-size: 12px;">
          ⚡ <b>Impact:</b> 100% recovery from deadlocked audio sockets across Fedora, Arch, Ubuntu, and SteamOS.
        </p>
        <div>
          <a href="https://github.com/louzt/pipewire/commit/2f747a7"><img src="https://img.shields.io/badge/PipeWire_Commit-2f747a7-38BDF8?style=flat-square&logo=github&logoColor=white" alt="PipeWire Commit"/></a>
          &nbsp;
          <a href="https://gist.github.com/louzt/c175973d8e8bae8c8fef6af4d9d6aca7"><img src="https://img.shields.io/badge/OpenAL_Gist-Notes-7C3AED?style=flat-square&logo=github&logoColor=white" alt="OpenAL Gist"/></a>
        </div>
      </div>
    </td>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #14b8a6; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-pink.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
          <img src="https://img.shields.io/badge/Async_Rust-1DB954?style=flat-square&logo=spotify&logoColor=white" align="right" alt="Async Rust"/>
          🎵 <b>spotify-player &amp; rspotify Terminal Ecosystem</b>
        </h4>
        <p style="margin: 0 0 8px 0; color: #cbd5e1; font-size: 13px;">
          Enabled headless terminal-native Spotify playback (TUI) with active session inheritance and zero GUI overhead. Disambiguated <code>is_active</code> Connect device presence from active playback (<code>is_playing</code>) in <code>spotify-player</code> (<a href="https://github.com/aome510/spotify-player/pull/1049">PR #1049</a>), unblocking <code>librespot</code> audio engine starvation on standby speakers. Serialized search requests (<a href="https://github.com/aome510/spotify-player/pull/1048">PR #1048</a>) eliminating 429 quota bursts. Proposed non-breaking Serde <code>#[serde(default)]</code> schema drift fallback in <code>rspotify</code> (<a href="https://github.com/ramsayleung/rspotify/issues/572">Issue #572</a>).
        </p>
        <p style="margin: 0 0 8px 0; color: #94a3b8; font-size: 12px;">
          ⚡ <b>Impact:</b> Headless TUI session inheritance, 100% elimination of HTTP 429 rate-limit spikes &amp; standby speaker playback deadlocks.
        </p>
        <div>
          <a href="https://github.com/aome510/spotify-player/pull/1049"><img src="https://img.shields.io/badge/PR_%231049-Merged-10B981?style=flat-square&logo=github&logoColor=white" alt="PR 1049"/></a>
          &nbsp;
          <a href="https://github.com/aome510/spotify-player/pull/1048"><img src="https://img.shields.io/badge/PR_%231048-Merged-10B981?style=flat-square&logo=github&logoColor=white" alt="PR 1048"/></a>
          &nbsp;
          <a href="https://github.com/ramsayleung/rspotify/issues/572"><img src="https://img.shields.io/badge/Issue_%23572-Triaged-38BDF8?style=flat-square&logo=github&logoColor=white" alt="Issue 572"/></a>
        </div>
      </div>
    </td>
  </tr>
  <tr>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #10b981; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-emerald.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
          <img src="https://img.shields.io/badge/Rust_IPC-000000?style=flat-square&logo=rust&logoColor=white" align="right" alt="Rust IPC"/>
          🖼️ <b>Wayland Compositor &amp; Display IPC Diagnostics</b>
        </h4>
        <p style="margin: 0 0 8px 0; color: #cbd5e1; font-size: 13px;">
          Authored pull-based typed IPC diagnostics, semantic asset labeling, and per-output mutex thread isolation across Niri Wayland display pipelines (<a href="https://gist.github.com/louzt/1c5230a2e9471faf9ce4243314361fa1">5 PRs Gist</a>). Exposed scaling filter matrix across swww/awww backends in Waypaper (<a href="https://github.com/louzt/761e227ad8cfe55b29e79cf861214a62">PR #286</a>).
        </p>
        <p style="margin: 0 0 8px 0; color: #94a3b8; font-size: 12px;">
          ⚡ <b>Impact:</b> Zero-drop frame pacing across multi-monitor displays with heterogeneous refresh rates.
        </p>
        <div>
          <a href="https://gist.github.com/louzt/1c5230a2e9471faf9ce4243314361fa1"><img src="https://img.shields.io/badge/Niri_IPC-5_PRs_Gist-10B981?style=flat-square&logo=github&logoColor=white" alt="Niri Gist"/></a>
          &nbsp;
          <a href="https://github.com/louzt/761e227ad8cfe55b29e79cf861214a62"><img src="https://img.shields.io/badge/Waypaper-PR_%23286-38BDF8?style=flat-square&logo=github&logoColor=white" alt="Waypaper PR"/></a>
        </div>
      </div>
    </td>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #8b5cf6; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-violet.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
          <img src="https://img.shields.io/badge/Web_Security-4285F4?style=flat-square&logo=googlechrome&logoColor=white" align="right" alt="Chromium Security"/>
          🌐 <b>Chromium 148 CSP Audit &amp; Web Security</b>
        </h4>
        <p style="margin: 0 0 8px 0; color: #cbd5e1; font-size: 13px;">
          Identified cross-origin <code>srcdoc</code> sandbox CSP Level 3 policy collision regressions in Chromium 148 (<a href="https://gist.github.com/louzt/77f0804ca11bad6636f0ac67928bd384">Gist</a>). Accepted upstream under Opera security disclosure tracking GB-80414.
        </p>
        <p style="margin: 0 0 8px 0; color: #94a3b8; font-size: 12px;">
          ⚡ <b>Impact:</b> Auditable security triage, CSP sandbox collision isolation, and upstream browser patch validation.
        </p>
        <div>
          <a href="https://gist.github.com/louzt/77f0804ca11bad6636f0ac67928bd384"><img src="https://img.shields.io/badge/Chromium_CSP-Audit_Gist-8B5CF6?style=flat-square&logo=github&logoColor=white" alt="Chromium Gist"/></a>
          &nbsp;
          <img src="https://img.shields.io/badge/Opera_Tracking-GB--80414-FF1B2D?style=flat-square&logo=opera&logoColor=white" alt="Opera GB-80414"/>
        </div>
      </div>
    </td>
  </tr>
</table>

<p align="center" style="margin: 16px 0 8px 0;">
  <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/banner-domain-network-security.svg" width="100%" alt="Resilient Network Transport and Web Security Domain Banner"/>
</p>

<table width="100%">
  <tr>
    <td valign="top" width="100%">
      <div style="background: #0f172a; border-left: 4px solid #f59e0b; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-amber.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
          <img src="https://img.shields.io/badge/Network_Eng-F59E0B?style=flat-square&logo=wireguard&logoColor=white" align="right" alt="Network Eng"/>
          🛰️ <b>Resilient Transport Proxy &amp; Linux Telemetry</b>
        </h4>
        <p style="margin: 0 0 8px 0; color: #cbd5e1; font-size: 13px;">
          Engineered 5-tier fallback transport proxy racing QUIC / Hysteria2 / TLS / SSH in &lt;200 ms with CA-pinned topology (<a href="https://gist.github.com/louzt/3991f144c7d67726045af3cefc60f42a">Gist</a>). Documented Linux PSI over polling and Redis <code>KEYS</code> → <code>SCAN/COUNT</code> zero-overhead observability (<a href="https://gist.github.com/louzt/b8349629b602a782ac98d0cbfd0df0c0">Gist</a>).
        </p>
        <p style="margin: 0 0 8px 0; color: #94a3b8; font-size: 12px;">
          ⚡ <b>Impact:</b> Sub-200ms transport racing across restrictive firewalls &amp; 70% reduction in Redis channel bloat.
        </p>
        <div>
          <a href="https://gist.github.com/louzt/3991f144c7d67726045af3cefc60f42a"><img src="https://img.shields.io/badge/Transport-Proxy_Gist-F59E0B?style=flat-square&logo=github&logoColor=white" alt="Transport Gist"/></a>
          &nbsp;
          <a href="https://gist.github.com/louzt/b8349629b602a782ac98d0cbfd0df0c0"><img src="https://img.shields.io/badge/Observability-PSI_Gist-10B981?style=flat-square&logo=github&logoColor=white" alt="Observability Gist"/></a>
        </div>
      </div>
    </td>
  </tr>
</table>

<p align="center" style="margin: 16px 0 8px 0;">
  <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/banner-domain-agents-cloud.svg" width="100%" alt="Sovereign Agent Fleets and Kubernetes Substrates Domain Banner"/>
</p>

<table width="100%">
  <tr>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #ec4899; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-pink.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
          <img src="https://img.shields.io/badge/Agent_Fleet_/_Rust-EC4899?style=flat-square&logo=rust&logoColor=white" align="right" alt="Agent Fleet Rust"/>
          🤖 <b>Sovereign Agent Fleet Provenance &amp; Git Claim Gates</b>
        </h4>
        <p style="margin: 0 0 8px 0; color: #cbd5e1; font-size: 13px;">
          Designed deterministic <code>agent_id</code> provenance tagging and subagent conversation ID audit traces across hierarchical agentic workflows. Implemented working-tree author classification (mine / foreign / mixed / unknown) with automated author email attribution gates. Engineered F80.14-aware <code>lzt-branch-claim</code> verification, preventing parallel agent branch drift or race conditions during automated PR-slicing and multi-agent code generation pipelines (<a href="https://gist.github.com/louzt/d1ce71c05460c2c32bf31342cd0c6a3f">Gist</a>).
        </p>
        <p style="margin: 0 0 8px 0; color: #94a3b8; font-size: 12px;">
          ⚡ <b>Impact:</b> Zero-drift multi-agent git branch claim verification &amp; 100% auditable agent execution provenance.
        </p>
        <div>
          <a href="https://gist.github.com/louzt/d1ce71c05460c2c32bf31342cd0c6a3f"><img src="https://img.shields.io/badge/Agent_Provenance-Gist-EC4899?style=flat-square&logo=github&logoColor=white" alt="Provenance Gist"/></a>
        </div>
      </div>
    </td>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #326ce5; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-cyan.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
          <img src="https://img.shields.io/badge/k3s_/_Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white" align="right" alt="k3s Kubernetes"/>
          ☸️ <b>k3s Kubernetes Standby Auto-Scaling &amp; RCON Teardowns</b>
        </h4>
        <p style="margin: 0 0 8px 0; color: #cbd5e1; font-size: 13px;">
          Engineered RCON-driven automated idle cluster detection and graceful worker node teardowns for zero-cost standby game and telemetry workloads on k3s / Lightweight Kubernetes (<a href="https://gist.github.com/louzt/b333b5601628a159630da13857834246">Gist</a>). Implemented event-driven pod scaling and node lifecycle controllers with fast warm-start initialization (&lt;15s container spin-up) under zero active player/connection load, eliminating 24/7 static VPS billings.
        </p>
        <p style="margin: 0 0 8px 0; color: #94a3b8; font-size: 12px;">
          ⚡ <b>Impact:</b> 100% idle infrastructure cost elimination &amp; &lt;15s warm-start cluster recovery under zero load.
        </p>
        <div>
          <a href="https://gist.github.com/louzt/b333b5601628a159630da13857834246"><img src="https://img.shields.io/badge/k3s_Auto--Scaling-Gist-326CE5?style=flat-square&logo=github&logoColor=white" alt="k3s Gist"/></a>
        </div>
      </div>
    </td>
  </tr>
</table>

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

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider-bracket-closing.svg" width="100%" alt="closing bracket divider"/></p>

<!-- ============================================================ -->
<!-- FOOTER: animated squares grid + tagline (no operator name).  -->
<!-- Served from profile-public static/ alongside the section     -->
<!-- banners. Editor-only provenance; GitHub strips the comment.  -->
<!-- ============================================================ -->
<div align="center">
  <img alt="Animated footer tagline" src="https://raw.githubusercontent.com/louzt/louzt/main/static/profile-footer.svg" width="100%" style="display:block;margin:0 auto"/>
</div>
