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

<p align="center" style="margin: 8px 0 12px 0;">
  <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-violet.svg" width="100%" height="4" alt="Lava Lamp Glow Divider"/>
</p>

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
    <!-- Row 1: Language Switcher Row (Active: English) -->
    <td align="left" valign="middle">
      <img src="https://img.shields.io/badge/%E9%96%B1%E8%AE%80%E7%B9%81%E9%AB%94%E4%B8%AD%E6%96%87-(%E5%8F%B0%E7%81%A3)-D97706?style=flat-square&logo=readme&logoColor=white" alt="閱讀繁體中文 (台灣)"/>
      <a href="https://github.com/louzt/louzt/blob/main/README.md"><img src="https://img.shields.io/badge/Read_in-English-0093D0?style=flat-square&logo=readme&logoColor=white" alt="Read in English"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.es.md"><img src="https://img.shields.io/badge/Leer_en-Espa%C3%B1ol-D97706?style=flat-square&logo=readme&logoColor=white" alt="Leer en Español"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.it.md"><img src="https://img.shields.io/badge/Leggi_in-Italiano-009246?style=flat-square&logo=readme&logoColor=white" alt="Leggi in Italiano"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.pt.md"><img src="https://img.shields.io/badge/Ler_em-Portugu%C3%AAs-009B3A?style=flat-square&logo=readme&logoColor=white" alt="Ler em Português"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.de.md"><img src="https://img.shields.io/badge/Auf-Deutsch_lesen-DD0000?style=flat-square&logo=readme&logoColor=white" alt="Auf Deutsch lesen"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.ja.md"><img src="https://img.shields.io/badge/%E6%97%A5%E6%9C%AC%E8%AA%9E%E3%81%A7-%E8%AA%AD%E3%82%80-BC002D?style=flat-square&logo=readme&logoColor=white" alt="日本語で読む"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.ko.md"><img src="https://img.shields.io/badge/%ED%95%9C%EA%B5%AD%EC%96%B4%EB%A1%9C-%EC%9D%BD%EA%B8%B0-0047A0?style=flat-square&logo=readme&logoColor=white" alt="한국어로 읽기"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.fr.md"><img src="https://img.shields.io/badge/Lire_en-Fran%C3%A7ais-0055A5?style=flat-square&logo=readme&logoColor=white" alt="Lire en Français"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.nl.md"><img src="https://img.shields.io/badge/In_het_Nederlands-lezen-21468B?style=flat-square&logo=readme&logoColor=white" alt="In het Nederlands lesen"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.sv.md"><img src="https://img.shields.io/badge/L%C3%A4s_p%C3%A5-Svenska-006AA7?style=flat-square&logo=readme&logoColor=white" alt="Läs på Svenska"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.pl.md"><img src="https://img.shields.io/badge/Czytaj_po-Polsku-DC143C?style=flat-square&logo=readme&logoColor=white" alt="Czytaj po Polsku"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.tr.md"><img src="https://img.shields.io/badge/T%C3%BCrk%C3%A7e-okuyun-E30A17?style=flat-square&logo=readme&logoColor=white" alt="Türkçe okuyun"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.hi.md"><img src="https://img.shields.io/badge/%E0%A4%A8%E0%A5%80%E0%A4%9A%E0%A5%87_%E0%A4%A5%E0%A5%80-%E0%A4%B9%E0%A4%BF%E0%A4%A8%E0%A5%8D%E0%A4%A6%E0%A5%80-%E0%A4%B9%E0%A4%BF%E0%A4%A8%E0%A5%8D%E0%A4%A6%E0%A5%80-FF9933?style=flat-square&logo=readme&logoColor=white" alt="हिन्दी में पढ़ें"/></a>
    </td>
  </tr>
    <!-- Row 2: Contact channels & Schedule a meeting & Spoken Languages -->
    <td align="left" valign="middle">
    <td align="left" valign="middle">
      <a href="https://calendar.app.google/XR7FkZXWVwfmZ57x6"><img src="https://img.shields.io/badge/%E9%A0%90%E7%B4%84%E6 me2%9B%E8 me2%AE-34A853?style=flat-square&logo=googlecalendar&logoColor=white" alt="預約會議 (Google Calendar)"/></a>
      <a href="https://www.linkedin.com/in/davidmirelesll/?locale=es_ES"><img src="https://img.shields.io/badge/Write_me_%26_Connect-LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="Write me & Connect on LinkedIn"/></a>
      <img src="https://img.shields.io/badge/GitLab-FC6D26?style=flat-square&logo=gitlab&logoColor=white" alt="GitLab"/>
      <img src="https://img.shields.io/badge/X-000000?style=flat-square&logo=x&logoColor=white" alt="X.com"/>
      <img src="https://img.shields.io/badge/Matrix-000000?style=flat-square&logo=matrix&logoColor=white" alt="Matrix"/>
      <img src="https://img.shields.io/badge/%7C-1e293b?style=flat-square" alt="|"/>
      <img src="https://img.shields.io/badge/Languages-1e293b?style=flat-square&logo=translate&logoColor=white" alt="Spoken Languages"/>
      <img src="https://img.shields.io/badge/Espa%C3%B1ol-Nativo-D97706?style=flat-square" alt="Español (Nativo)"/>
      <img src="https://img.shields.io/badge/English-Full_Professional-0093D0?style=flat-square" alt="English (Full Professional)"/>
      <img src="https://img.shields.io/badge/Portugu%C3%AAs-Working_Knowledge-009B3A?style=flat-square" alt="Português (Working Knowledge)"/>
    </td>
  </tr>
  <tr>
    <td align="left" valign="middle">
      <a href="https://komarev.com/ghpvc/?username=louzt&label=profile+views&color=1e293b&style=flat-square"><img src="https://komarev.com/ghpvc/?username=louzt&label=profile+views&color=1e293b&style=flat-square" alt="Profile Views"/></a>
      <a href="https://orcid.org/0009-0008-4374-2254"><img src="https://img.shields.io/badge/ORCID-0009--0008--4374--2254-A6CE39?style=flat-square&logo=orcid&logoColor=white" alt="ORCID iD 0009-0008-4374-2254"/></a>
      <a href="https://gist.github.com/louzt"><img src="https://img.shields.io/badge/Gists-181717?style=flat-square&logo=github&logoColor=white" alt="Gists"/></a>
      <a href="mailto:research@loust.pro"><img src="https://img.shields.io/badge/research%40loust.pro-7C3AED?style=flat-square&logo=protonmail&logoColor=white" alt="research@loust.pro"/></a>
      <a href="https://opensource.org/"><img src="https://img.shields.io/badge/OSI-%E4%BC%9A%E5%93%A1-3DA639?style=flat-square&logo=opensourceinitiative&logoColor=white" alt="OSI Member"/></a>
      <a href="https://github.com/django-commons"><img src="https://img.shields.io/badge/Django_Commons-0C4B33?style=flat-square&logo=django&logoColor=white" alt="Django Commons Member"/></a>
      <a href="https://kernel.org/"><img src="https://img.shields.io/badge/Linux_Kernel-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux Kernel"/></a>
      <a href="https://crates.io/users/louzt"><img src="https://img.shields.io/badge/crates.io-000000?style=flat-square&logo=rust&logoColor=e43717" alt="crates.io packages"/></a>
      <img src="https://img.shields.io/badge/%2b_%E5%85%B6%E4%BB%96%E8%A8%B1%E5%A4%9A-1E293B?style=flat-square" alt="+ many more communities"/>
    </td>
  </tr>
    <!-- Row 3: Core Programming Languages & Core Engine Technologies -->
    <td align="left" valign="middle">
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
      <img src="https://img.shields.io/badge/%E7%B4%94%E7%B2 me2%B7%E5%B0%8D%E5%85%B6%E4%BB%96%E6%8A%80%E8%A1%93%E7%96 me2%B3%E8%AA%BF%E8 me2%A6%E4%BF%9D%E6 me2%81%E5 me2%BD%E8%B6%A3-8b5cf6?style=flat-square&logoColor=white" alt="Always curious to debug in another tech stack"/>
    </td>
  </tr>
    <!-- Row 4: MarTech, AdTech, PropTech, Hospitality & Commercial Tech Infrastructure -->
    <td align="left" valign="middle">
    <td align="left" valign="middle">
      <img src="https://img.shields.io/badge/MarTech_%26_AdTech-FF5722?style=flat-square&logo=googleanalytics&logoColor=white" alt="MarTech & AdTech"/>
      <img src="https://img.shields.io/badge/PropTech_%26_Real_Estate-00897B?style=flat-square&logo=homeassistant&logoColor=white" alt="PropTech & Real Estate Tech"/>
      <img src="https://img.shields.io/badge/Restaurant_%26_Hospitality_Tech-D81B60?style=flat-square&logo=ubereats&logoColor=white" alt="Restaurant & Hospitality Tech"/>
      <img src="https://img.shields.io/badge/Google_Ads_API-4285F4?style=flat-square&logo=googleads&logoColor=white" alt="Google Ads API"/>
      <img src="https://img.shields.io/badge/Meta_CAPI-1877F2?style=flat-square&logo=meta&logoColor=white" alt="Meta Conversions API"/>
      <img src="https://img.shields.io/badge/TikTok_Ads_API-000000?style=flat-square&logo=tiktok&logoColor=white" alt="TikTok Ads API"/>
      <img src="https://img.shields.io/badge/X_Ads_API-000000?style=flat-square&logo=x&logoColor=white" alt="X Ads API"/>
      <img src="https://img.shields.io/badge/Stripe_API-635BFF?style=flat-square&logo=stripe&logoColor=white" alt="Stripe API"/>
      <img src="https://img.shields.io/badge/PayPal_API-003087?style=flat-square&logo=paypal&logoColor=white" alt="PayPal API"/>
      <img src="https://img.shields.io/badge/MercadoPago_API-009EE3?style=flat-square&logo=mercadopago&logoColor=white" alt="MercadoPago API"/>
      <img src="https://img.shields.io/badge/%E5%8A%A0%E5%AF%86%E8%B2%A8%E5%B9%A3%E6%94%AF%E4%BB%98_(BTC%2fSOL)-121D33?style=flat-square&logo=solana&logoColor=white" alt="Crypto Payments"/>
      <img src="https://img.shields.io/badge/%E8 me2%AA%E5%AE%9A_REST_%26_GraphQL_APIs-00A1E0?style=flat-square" alt="Custom REST & GraphQL APIs"/>
      <img src="https://img.shields.io/badge/%E4%BC%BA%E6%9C%8D%E7%AB%AF%E8%BF%BD%E8%B9%A4-00A1E0?style=flat-square&logo=salesforce&logoColor=white" alt="Server-Side Tracking"/>
      <img src="https://img.shields.io/badge/CRM-00A1E0?style=flat-square&logo=salesforce&logoColor=white" alt="CRM"/>
      <img src="https://img.shields.io/badge/ERP-714B67?style=flat-square" alt="ERP"/>
      <img src="https://img.shields.io/badge/SaaS--to--SaaS-2C3E50?style=flat-square" alt="SaaS-to-SaaS"/>
    </td>
  </tr>
    <!-- Row 5: Web3 & Decentralized Infrastructure -->
    <td align="left" valign="middle">
    <td align="left" valign="middle">
      <img src="https://img.shields.io/badge/Blockchain_%26_Web3-121D33?style=flat-square&logo=blockchaindotcom&logoColor=white" alt="Blockchain & Web3"/>
      <img src="https://img.shields.io/badge/MCP_%26_%E4%BB%A3%E7%90%86%E5%8D%9F%E8%AD%B0-000000?style=flat-square&logo=github&logoColor=white" alt="MCP & Agent Protocols"/>
      <img src="https://img.shields.io/badge/%E4%BB%A3%E7%90%86%E5%B7%A5%E4%BD%9C%E6%B5 me2%E7%A8%8B-7c3aed?style=flat-square" alt="Agentic Workflows"/>
      <img src="https://img.shields.io/badge/RBAC_%26_%E5%A4%9A%E7%A7%9F me2%B6%E9%9A%94%E9%9B me2-0f172a?style=flat-square" alt="RBAC & Multi-Tenant Isolation"/>
      <img src="https://img.shields.io/badge/Ed25519_%E8%BA%AB%E4%BB%BD-2C3E50?style=flat-square" alt="Ed25519 Identity"/>
      <img src="https://img.shields.io/badge/Virtuoso_Triples_%2f_SPARQL-2C3E50?style=flat-square" alt="Virtuoso Triples / SPARQL"/>
      <img src="https://img.shields.io/badge/%E7%9F%A5%E8%AD%98%E5%9C%96%E8%AD me2-0f172a?style=flat-square" alt="Knowledge Graphs"/>
      <img src="https://img.shields.io/badge/Local--First_%26_CRDT-064E3B?style=flat-square" alt="Local-First & CRDT"/>
    </td>
  </tr>
    <!-- Row 6: Research Specializations, Engineering Categories & Community Call -->
    <td align="left" valign="middle">
    <td align="left" valign="middle">
      <a href="https://gist.github.com/louzt/376f48c722d4a15d7e78f940818cbade"><img src="https://img.shields.io/badge/%E7%A2%BA%E5%AE%9A%E6%80%A7%E6%B8%AC%E8%A9 me2%E5%A5%97%E4%BB%B6-8b5cf6?style=flat-square" alt="Deterministic Harnesses"/></a>
      <a href="https://gist.github.com/louzt/d1ce71c05460c2c32bf31342cd0c6a3f"><img src="https://img.shields.io/badge/Sovereign_RAG-7c3aed?style=flat-square" alt="Sovereign RAG"/></a>
      <img src="https://img.shields.io/badge/%E8%A6%8F%E6%A0%BC%E9 me2%B1%E5%B0 me2%E5%B7%A5%E7%A8%8B-0284c7?style=flat-square" alt="Spec-Driven Engineering"/>
      <img src="https://img.shields.io/badge/Zero--Egress_%E5%AE%89%E5%85%A8-1F2937?style=flat-square" alt="Zero-Egress Security"/>
      <img src="https://img.shields.io/badge/%E6%A0%B8%E5%BF%83%E8%88%87%E5%9F%B7%E8%A1%8C%E9%9A me2%E5%98 me2%E5%8C%96-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Kernel & Runtime Hardening"/>
      <img src="https://img.shields.io/badge/CLA_%26_FOSS_%E6%B2%BB%E7%90%86-004D40?style=flat-square" alt="CLA & FOSS Governance"/>
      <a href="mailto:partnership@loust.pro"><img src="https://img.shields.io/badge/partnership%40loust.pro-0A66C2?style=flat-square&logo=minutemailer&logoColor=white" alt="partnership@loust.pro"/></a>
      <a href="mailto:partnership@loust.pro?subject=FOSS%20Community%20Collaboration"><img src="https://img.shields.io/badge/Open_to_contribute_to_FOSS%2FOSS_Communities-34A853?style=flat-square&logo=opensourceinitiative&logoColor=white" alt="Open to contribute to FOSS/OSS Communities"/></a>
      <a href="mailto:partnership@loust.pro?subject=Peer%20Collaboration"><img src="https://img.shields.io/badge/%E5%B0%8B%E6 me2%82%E5%90%8C%E4%BC%B4%E8%88%87%E4%BB%A4%E4%BA%BA%E8%88%B4%E5%A5 me2%E7%9A%84%E5%B0%88%E6%A1%88-0284c7?style=flat-square" alt="Looking for peers & exciting projects"/></a>
    </td>
  </tr>
    <!-- Row 7: Roles, Infrastructure & Mindset -->
    <td align="left" valign="middle">
    <td align="left" valign="middle">
      <img src="https://img.shields.io/badge/%E7%B3%BB%E7%B5%B1%E6 me2%B6%E8%A8%88%E5%B8%AB-0f172a?style=flat-square" alt="Systems Architect"/>
      <img src="https://img.shields.io/badge/DevOps_%26_SRE-2563eb?style=flat-square&logo=kubernetes&logoColor=white" alt="DevOps & SRE"/>
      <img src="https://img.shields.io/badge/%E5%B9 me2%E8%87%BA%E5%B7%A5%E7%A8%8B-0891b2?style=flat-square" alt="Platform Engineering"/>
      <img src="https://img.shields.io/badge/%E5%AE%89%E5%85%A8%E7%A0%94%E7%A9%B6%E5%93%A1-eb0029?style=flat-square&logo=hackerone&logoColor=white" alt="Security Researcher"/>
      <img src="https://img.shields.io/badge/%E7%AC%AC%E4%B8%80%E5%8E%9F%E5%89%87%E5%B7%A5%E7%A8%8B-6366f1?style=flat-square" alt="First-Principles Engineering"/>
      <img src="https://img.shields.io/badge/Zero--Trust_%E5%9F%BA%E7%A4%8D%E8%A8%AD%E6%96%BD-1e293b?style=flat-square" alt="Zero-Trust Infrastructure"/>
      <img src="https://img.shields.io/badge/%E6%A0%B8%E5%BF%83%E8%88%87%E7%B3%BB%E7%B5%B1%E7%A0%94%E7%A9%B6-0f172a?style=flat-square&logo=linux&logoColor=white" alt="Kernel & Systems Research"/>
      <img src="https://img.shields.io/badge/%E7 me2%9F%E8%BA%AB%E5%AD%B8%E7%BF%92%E8%80%85-7c3aed?style=flat-square" alt="Lifelong Student"/>
    </td>
  </tr>

<div align="center">
<div align="center">
  <img alt="Systems Architecture &amp; Operational Posture — section banner" src="https://raw.githubusercontent.com/louzt/louzt/main/static/section-tactical-posture.svg" width="100%" />

我維持一種預防性、嚴謹且確定性的工程姿態——持續根據實證資料校準推理過程、傳輸層與作業流程。我設計並交付生產系統，其中應用程式交付與系統工程的邊界必須成立。我大部分的工作是研究導向的工程：抽象化是可複用的，證明在必要時是形式化的，操作證據可端到端審計。

<blockquote style="border-left: 3px solid #10b981; background: #0f172a; padding: 12px 16px; margin: 16px 0; border-radius: 0 6px 6px 0; color: #e2e8f0;">
<blockquote style="border-left: 3px solid #10b981; background: #0f172a; padding: 12px 16px; margin: 16px 0; border-radius: 0 6px 6px 0; color: #e2e8f0;">
  <b>Confucius</b> <i>(Philosopher)</i>: <i>"Choose a job you love, and you will never have to work a day in your life."</i>

<blockquote style="border-left: 3px solid #38bdf8; background: #0f172a; padding: 12px 16px; margin: 16px 0; border-radius: 0 6px 6px 0; color: #e2e8f0;">
<blockquote style="border-left: 3px solid #38bdf8; background: #0f172a; padding: 12px 16px; margin: 16px 0; border-radius: 0 6px 6px 0; color: #e2e8f0;">
  <b>Rob Pike</b> <i>(Co-creator of Go &amp; UTF-8)</i>: <i>"Data dominates. If you've chosen the right data structures and organized things well, the algorithms will almost always be self-evident."</i>

<blockquote style="border-left: 3px solid #8b5cf6; background: #0f172a; padding: 12px 16px; margin: 16px 0; border-radius: 0 6px 6px 0; color: #e2e8f0;">
<blockquote style="border-left: 3px solid #8b5cf6; background: #0f172a; padding: 12px 16px; margin: 16px 0; border-radius: 0 6px 6px 0; color: #e2e8f0;">
  <b>Rich Hickey</b> <i>(Creator of Clojure &amp; Datomic)</i>: <i>"Simplicity is a prerequisite for reliability."</i>

<blockquote style="border-left: 3px solid #ec4899; background: #0f172a; padding: 12px 16px; margin: 16px 0; border-radius: 0 6px 6px 0; color: #e2e8f0;">
<blockquote style="border-left: 3px solid #ec4899; background: #0f172a; padding: 12px 16px; margin: 16px 0; border-radius: 0 6px 6px 0; color: #e2e8f0;">
  <b>Fred Brooks</b> <i>(Turing Award Winner &amp; Author of The Mythical Man-Month)</i>: <i>"Conceptual integrity is the most important consideration in system design. Good judgment comes from experience, and experience comes from bad judgment."</i>

<blockquote style="border-left: 3px solid #f59e0b; background: #0f172a; padding: 12px 16px; margin: 16px 0; border-radius: 0 6px 6px 0; color: #e2e8f0;">
<blockquote style="border-left: 3px solid #f59e0b; background: #0f172a; padding: 12px 16px; margin: 16px 0; border-radius: 0 6px 6px 0; color: #e2e8f0;">
  <b>Werner Vogels</b> <i>(CTO of Amazon)</i>: <i>"Everything fails, all the time. Design for recovery, not perfection."</i>

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/section-how-i-work.svg" width="100%" alt="How I work — section banner"/></p>

- 我以類似工匠在 workshop 的方式來處理系統工程——在撰寫程式或提出重構方案之前，先研究產品架構、傳輸瓶頸，以及從頭到尾的遙測資料。
- 我以專注且有條不紊的耐心來提取確定性遙測資料，精確到最後一個資料點——每當現有工具留下模糊空間時，就會建構自訂測試工具、

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/section-working-with-me.svg" width="100%" alt="Working with me — section banner"/></p>

### 與我合作

- **回饋與學習** — 如果您在哪裡看到我學習如何更好地在軟體團隊中工作，我會很感興趣。資深審查者、工程主管或同事如果有任何具體的技術觀察——程式碼審查討論、共享程式庫、流程摩擦——都歡迎與我聯繫。我認為您的意見很有價值，並將回饋視為雙向循環，而非單向交付物；最好的學習姿態是讓雙方的稽核軌跡都保持清晰可讀。
- **HackerOne 回報管道** — 在我們範圍內的基礎設施漏洞回報與協調披露請透過 [security@loust.pro](mailto:security@loust.pro) 處理。72 小時內完成分類；可重現的 PoC 加上最小範圍的修補建議會讓回報優先處理。超出範圍的訊號（DMS、PipeWire 強化）以及忙碌的分類時段都會記錄在案，以免回報者徒勞無功。
- **研究合作** — 形式化證明、決定性系統、傳輸層強化、主權 AI 基礎設施。最適合的合作對象：大學實驗室、獨立博士級研究人員，以及在應用機率 / IR / 代理框架領域工作的私人研發團隊。請透過 [research@loust.pro](mailto:research@loust.pro) 聯繫，附上 1 段摘要與具體成果（gist、論文草稿、基準測試）。
- **開放原始碼上游強化** — 如果您維護的開放原始碼專案具有明確界限的執行期模型（生命週期合約、配置器熱路徑、合成器或守護行程邊界），我很樂意聊聊。我會針對執行期邊界提出範圍明確的 PR；帶來可重現的問題與最小範圍的修補程式即可，不需要簡報。公開邀請——長期貢獻者或共同維護者路線。
- **社群與聊天** — IRC、Discord、Matrix 以及相關的聊天社群是我偏好的頻道，勝過主流社交網路。如果您在這些平台上活跃於開放原始碼社群（Libera.Chat / OFTC、Matrix 聊天室、Discord 開放原始碼伺服器、專案專屬頻道），歡迎 ping 我。我讀的多、寫的少，但我重視訊號品質勝過數量。
- **B2B 平台業務 / 合作夥伴** — 只接受長期承諾的合作。我們會在宣布任何東西已交付之前，先建構好基底、可觀測性與稽核軌跡——分階段推出的能力才是限制，而非日曆上的日期。請透過 [partnership@loust.pro](mailto:partnership@loust.pro) 聯繫。
- **推薦信政策** — 我會為有可衡量成果的已交付工作撰寫公開推薦信。請發送 PR / 成果連結以及 1 行成果指標；我會在一週內回覆。

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider.svg" width="100%" alt="divider"/></p>

<h3 align="center"><b>SERVICES &amp; ENGINEERING SOLUTIONS MATRIX</b></h3>

<p align="center"><sub>High-rigor technical services and consulting backed by 850K+ lines of production code across 50+ delivered systems</sub></p>

| Service Category | Engineering Capabilities & Tech Stack | Value Proposition & Deliverable |
| Service Category | Engineering Capabilities & Tech Stack | Value Proposition & Deliverable |
| :--- | :--- | :--- |
| **Systems & Kernel Hardening** | POSIX `prctl`, C/C++, Rust, IPC, Linux daemons, container isolation, eBPF / `tcp_diag` | Eliminates memory/CPU leaks, zombie process loops, and daemon IPC hangs under heavy production loads. |
| **Custom REST & GraphQL APIs** | TypeScript, Next.js, Apollo Server v4, Prisma, PostgreSQL, Redis Lua, APQ at scale | Sub-15ms p95 query latency, multi-tenant RBAC namespace isolation, and zero-downtime schema evolution. |
| **MarTech & AdTech Infrastructure** | Google Ads API, Meta CAPI, TikTok Ads API, X Ads API, Server-Side Tracking, CRM/ERP | Server-side conversion attribution, zero data-loss tracking, and CFDI 4.0 automated billing integrations. |
| **SaaS & Payment Gateway Integrations** | Stripe, PayPal, MercadoPago, Crypto (BTC/Solana), Webhooks, Microservices | Multi-currency, multi-gateway resilient billing pipelines with automated reconciliation and zero retry amplification. |
| **Sovereign AI & Agent Control Planes** | Model Context Protocol (MCP), Sovereign RAG, Local Vector Substrates, Zero-Egress Agents | Local-first agentic workflows with bounded latency, VRAM budgeting, and continuous contract verification. |

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/section-selected-work.svg" width="100%" alt="Selected Work — section banner"/></p>

已部署至實際使用者、合併至上游程式碼，或作為長期用戶端平台的正式作業系統。公開成果會連結出去；私人平台僅以名稱提及——公開驗證與客戶機密工作之間的界線是刻意設定、可審查，且在各項合作中保持不變。

**我們如何保持最新。** 在安裝前會先閱讀發布說明。規格變更日誌（MCP、Claude、OpenAI、Gemini、我們依賴的每個模型 API）會持續監控。在任何東西交付之前，優先排序會深入多層——目標是理解我們依賴的任何事物的*願景*、*範圍*和*未來步驟*，這樣操作者接手的是穩固的系統，而非紙牌屋。

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider.svg" width="100%" alt="divider"/></p>

<h3 align="center"><b>PUBLIC UPSTREAM HARDENING &amp; CORE SYSTEMS INVARIANTS</b></h3>

<p align="center"><sub>Direct C/C++, Rust, and Linux kernel contributions merged into primary upstream repositories</sub></p>

| Upstream Target | Technical Contribution & Global Impact | Pain Point Solved & Verification |
| Upstream Target | Technical Contribution & Global Impact | Pain Point Solved & Verification |
| :--- | :--- | :--- |
| **Valve Software**<br/>`ValveSoftware/Fossilize`<br/>([PR #305](https://github.com/ValveSoftware/Fossilize/pull/305) · [#308](https://github.com/ValveSoftware/Fossilize/pull/308) · [#311](https://github.com/ValveSoftware/Fossilize/pull/311) · [#310](https://github.com/ValveSoftware/Fossilize/pull/310)) | **Eradicated 100% CPU runaway zombie processes & battery drain across millions of Steam Deck / SteamOS devices worldwide** via `PR_SET_PDEATHSIG` + `getppid` race mitigation (#305). Catalyzed multi-GPU manifest schema (#308) and authored compile-time `static_assert` type-safety guard (#311) that unblocked Valve's **+7,913 LOC `fossilize-feature-sifter` Mesa CI silicon audit suite (#310)**. | **Ranked among the only 12 contributors worldwide** to `master` (2024–2026) alongside Valve Vulkan lead Hans-Kristian Arntzen, DXVK lead Philip Rebohle, and Mesa driver leads. Benchmark: 100% elimination of orphan Vulkan shader replayers on Proton crashes. |
| **Freedesktop PipeWire**<br/>`pipewire/pipewire`<br/>([commit 2f747a7](https://github.com/louzt/pipewire/commit/2f747a7)) | **Eliminated permanent Linux audio CLI deadlocks (`wpctl`/`pactl` hanging indefinitely)** when daemon IPC locks up, enforcing a 5s `spa timer` protocol-native connection timeout on `pw_protocol_native_connect_local_socket()`. | Solves core audio subsystem freezes across Linux distributions (Fedora, Arch, Ubuntu, SteamOS). Benchmark: 100% recovery from unresponsive daemon sockets. |
| **Niri Wayland Compositor**<br/>([5 PRs / Gist](https://gist.github.com/louzt/1c5230a2e9471faf9ce4243314361fa1)) | **Engineered pull-based typed IPC diagnostics, semantic asset labeling, and per-output mutex thread isolation** across Wayland display pipelines, preventing multi-monitor rendering stutter. | Eradicates display thread contention and IPC memory bloat. Benchmark: zero-drop frame pacing across heterogeneous refresh rates. |
| **spotify-player & rspotify**<br/>([PR #1049](https://github.com/aome510/spotify-player/pull/1049) · [#1048](https://github.com/aome510/spotify-player/pull/1048) · [Issue #572](https://github.com/ramsayleung/rspotify/issues/572)) | **Disambiguated `is_active && is_playing` Connect device state-machines** to prevent audio engine starvation on standby smart speakers (#1049), and **serialized search queries to eliminate 100% HTTP 429 quota exhaustion bursts** (#1048). | Eliminates audio stream deadlocks on standby speakers and HTTP rate-limit crashes. Benchmark: 100% elimination of 429 rate-limit spikes during fast TUI navigation. |
| **Waypaper**<br/>([PR #286](https://github.com/anufrievroman/waypaper/pull/286)) | **Exposed scaling filter matrix across swww/awww backends**, resolving HiDPI interpolation artifacts and pixel-art blur across Linux desktop environments. | Solves desktop visual distortion under mixed DPI. Benchmark: pixel-perfect 1:1 scaling precision. |
| **NVIDIA DKMS Kernel 7.0+ RFC**<br/>([Gist RFC](https://gist.github.com/louzt/1c85044d5090d19223c3f5edf426a19e)) | **Engineered forward-compat patch series for Kernel 7.0 API refactoring** (VMA locking, DMA fence signals) and `NVreg_DynamicPowerManagement=0x02` modprobe rules for Optimus USB-C D3cold hotplug panics. | Eradicates kernel panics and GPU suspend/resume lockups on hybrid laptops. Benchmark: 100% clean D3cold state transitions. |
| **DankMaterialShell (DMS)**<br/>([PR #2972](https://github.com/AvengeMedia/DankMaterialShell/pull/2972) · [#2312](https://github.com/AvengeMedia/DankMaterialShell/pull/2312) · [#2690](https://github.com/AvengeMedia/DankMaterialShell/pull/2690) · [#1887](https://github.com/AvengeMedia/DankMaterialShell/pull/1887) · [#2311](https://github.com/AvengeMedia/DankMaterialShell/pull/2311)) | **Redesigned the plugin & theme registry subsystem** enabling user-configurable multi-source aggregation with ID-based deduplication & declaration-order priority (#2972 — adopted by maintainer for CLI, IPC server & QML UI). **Engineered Quickshell / QML Wayland shell component hardening** — VPN transient active entry leak resolution (#2312), thermal widget routing & status unification (#2690), notification auto-reload IPC hooks (#1887), multi-bar entrypoint state isolation (#2311). | Solves plugin source isolation & legacy cache migration, Wayland shell RAM bloat, transient state memory leaks, and QML rendering freezes. Benchmark: zero memory drift over multi-day continuous desktop sessions. |
| **NGINX**<br/>([Evidence &amp; branch-split Gist](https://gist.github.com/louzt/7bdf370a28126718e7e7b69d53b0ae86)) | **Documented runtime CRLF injection vector** in NGINX via `$uri` propagation through `proxy_pass`, `proxy_set_header`, `add_header`, and `add_trailer` directives — enabling arbitrary HTTP header injection through malformed upstream variables ([nginx#590](https://github.com/nginx/nginx/pull/590) · [#1414](https://github.com/nginx/nginx/pull/1414) · [nginx-tests#55](https://github.com/nginx/nginx-tests/pull/55) · [#58](https://github.com/nginx/nginx-tests/pull/58)). | Hardens `ngx_http_proxy_module.c` + `ngx_http_headers_filter_module.c` against header smuggling. Benchmark: 4.6k–4.9k req/s on ApacheBench for valid requests with sanitization active. |

<details>
<details>

<table width="100%">
<table width="100%">
<tr>
<td valign="top" width="50%">
<div style="background: #0f172a; border-left: 4px solid #38bdf8; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
<h4 style="margin: 8px 0 6px 0; color: #f8fafc;">🎯 Env-var-first, config-file-later</h4>
當發布覆寫旗標時，從環境變數（<code>DMS_PLUGIN_REGISTRIES</code>）開始，而非設定檔。為指令碼撰寫、容器化部署和 CI 提供零阻力。只有在狀態必須持續或 UI 必須編輯它時，才遷移到設定檔。
</p>
</p>
⚠️ <b>權衡取捨：</b>在持久化到來之前沒有驗證層。<br>
🚫 <b>何時不應套用：</b>狀態繁重的設定，具有多個關聯欄位。
</p>
</p>
</div>
</td>
<td valign="top" width="50%">
<div style="background: #0f172a; border-left: 4px solid #f472b6; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
<h4 style="margin: 8px 0 6px 0; color: #f8fafc;">🪜 Third-caller applies</h4>
重複的程式碼在 2 個套件中是可以接受的。僅當 ≥3 個呼叫者需要相同的形式時，才萃取共享的抽象層（例如：外掛程式 + 佈景主題 + 網路處理常式 + CLI = 4 → 是時候萃取 <code>core/internal/registries</code>）。強迫誠實的命名以及共享的驗證，延後過度抽象化。
</p>
</p>
⚠️ <b>權衡：</b>短期重複程式碼成本；消除過早的抽象化。
</p>
</p>
</div>
</td>
</tr>
<tr>
<td valign="top" width="50%">
<div style="background: #0f172a; border-left: 4px solid #34d399; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
<h4 style="margin: 8px 0 6px 0; color: #f8fafc;">🔁 Idempotent cache migration by signature</h4>
當重組磁碟上的狀態時，透過<b>外觀</b>來偵測舊版（例如，存在 <code>&lt;cache&gt;/.git</code>，或扁平的 <code>&lt;cache&gt;/plugins/</code> 目錄）— 而非版本號碼。當新佈局已存在時，遷移必須是空作業，因此重新執行是安全的，且併發程式不會損壞狀態。
</p>
</p>
⚠️ <b>權衡取捨：</b> 啟發式偵測需要防禦性 <code>os.IsNotExist</code> 處理。
</p>
</p>
</div>
</td>
<td valign="top" width="50%">
<div style="background: #0f172a; border-left: 4px solid #facc15; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
<h4 style="margin: 8px 0 6px 0; color: #f8fafc;">⚖️ Declaration order = priority</h4>
當組合多個來源時，「首次命中即勝出」透過有序迭代達成。避免新增 <code>priority: int</code> 或 <code>disabled: bool</code> 欄位 — 列表順序 <i>即</i> 是優先級契約。進階使用者可以自然地分層註冊表：<code>official → personal → experimental</code>。
</p>
</p>
⚠️ <b>Tradeoff：</b>沒有辦法「跳過」登錄檔而不將其從列表中移除。
</p>
</p>
</div>
</td>
</tr>
<tr>
<td valign="top" width="50%">
<div style="background: #0f172a; border-left: 4px solid #a78bfa; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
<h4 style="margin: 8px 0 6px 0; color: #f8fafc;">🧩 Errors.Join for partial-failure aggregation</h4>
從 N 個來源匯聚時，改為回傳 <code>errors.Join(errs...)</code> 而非在首個錯誤時中止。一個損壞的登錄檔不應封鎖其他登錄檔。呈現部分狀態比無聲失敗更誠實，比完全中止更有用。直接追溯自維護者的重寫之 <a href="https://github.com/AvengeMedia/DankMaterialShell/pull/2972">DMS #2972</a>，在我的首次迭代於首次失敗後中止之後。
</p>
</p>
⚠️ <b>取捨：</b>呼叫端必須檢查合併的錯誤，才能知道哪些來源失敗。
</p>
</p>
</div>
</td>
<td valign="top" width="50%">
<div style="background: #0f172a; border-left: 4px solid #fb7185; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
<h4 style="margin: 8px 0 6px 0; color: #f8fafc;">🛡️ Reserved name + validation regex</h4>
任何「預設 + 自訂列表」功能（登錄檔、主題、設定檔、代理程式 fleet）都需要一個保留名稱作為官方預設值（<code>"official"</code>），以及一個嚴格的驗證正規表示式（<code>^[a-z0-9][a-z0-9-]{0,31}$</code>）。這可防止欺騙、路徑遍歷，以及當設定檔覆寫環境變數預設值時，預設值被靜默覆蓋的情況。
</p>
</p>
⚠️ <b>Tradeoff:</b> 更多前期驗證成本；消除整個類別的「why is my default gone」臭蟲。
</p>
</p>
</div>
</td>
</tr>

</details>

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider.svg" width="100%" alt="divider"/></p>

<h3 align="center"><b>B2B MULTI-TENANT PLATFORMS &amp; SOVEREIGN SYSTEMS</b></h3>

<p align="center"><sub>Production platforms, enterprise engines, autonomous agent control planes, and netcode substrates</sub></p>

| System / Engine / Substrate | Technical Focus & Architecture | Operational Impact & ROI |
| System / Engine / Substrate | Technical Focus & Architecture | Operational Impact & ROI |
| **LOUST Multi-Tenant Engine**<br/>*(Current, 7y 6m)* | Multi-tenant Next.js 16 + Apollo Server v4 + Redis 7 Lua EVAL + cgroup v2 isolation on a 135k-line GraphQL schema. Case study: [English](https://gist.github.com/louzt/64715cb9c6ec6ffdd98c5712b8fb7bac) / [Español](https://gist.github.com/louzt/0c91771bf6370f0eb47e905934ab47e8). | **90.9% APQ cache hit rate**, $p95 = 12\text{ ms}$, $+125\%$ throughput lift at $0/\text{mo}$ incremental infrastructure cost. |
| **SocialSphereMX Multi-Tenant SaaS**<br/>([socialspheremx.loust.pro](https://socialspheremx.loust.pro)) | Multi-tenant SaaS fabric for creators, ERP for restaurants with QR menus/KDS, real-time PropTech inventory, and live Spotify/YouTube metadata streams. | **99.9% real uptime**, live API metadata ingestion, zero legacy PDF overhead, and sub-2 min lead workflows. |
| **SocialSphereMX Multi-Tenant SaaS**<br/>([socialspheremx.loust.pro](https://socialspheremx.loust.pro)) | Multi-tenant SaaS fabric for creators, ERP for restaurants with QR menus/KDS, real-time PropTech inventory, and live Spotify/YouTube metadata streams. | **99.9% real uptime**, live API metadata ingestion, zero legacy PDF overhead, and sub-2 min lead workflows. |
| **LZT SRE Harness**<br/>*(Private)* | Distributed data plane in Rust + Go: asymmetric cognitive routing, 3-way semantic sync + Bayesian Stream Guard (<0.5s kill-switch). | Decouples agent reasoning from provider volatility; **99.5% effective cache rate** and drastically reduced token burn-rate. |
| **H4KKEN Fighting Game Engine**<br/>([h4kken.loust.pro](https://h4kken.loust.pro)) | GGPO-style 30-frame rollback netcode + WebRTC/WebSocket dual transport + Babylon.js 8 WebGPU rendering. Deployed on a private VPS. | **Sub-frame input prediction (>70% accurate)**, seamless WebRTC DataChannel upgrades, and zero unauthenticated frame exposure at the transport layer. |
| **NetBoozt**<br/>([Releases](https://github.com/LOUST-PRO/NetBoozt_InternetUpgrade/releases) · [Repo](https://github.com/LOUST-PRO/NetBoozt_InternetUpgrade)) | Tauri v3.1 (Rust) + native C netcode + Fallback DNS module for Windows/Linux: ISP & modem DNS stall recovery, TCP window autotuning, BBR/Cubic selection, `TCP_NODELAY`, QoS DSCP, and MTU/MSS discovery. | **$+15\text{--}20\%$ real-world throughput gains** via queueing discipline, fallback DNS resilience, and zero packet loss. |
| **h3ph43st Agent Runtime**<br/>*(Private, AGPLv3)* | Closed-core agent runtime: pruned Rust CLI (`h3ph`) talking to a multi-tenant k3s sidecar for ephemeral SAST scans. | Locked egress and isolated reasoning — client nodes never see system prompts, tool contracts, or reasoning loops. |
| **h3ph43st Agent Runtime**<br/>*(Private, AGPLv3)* | Closed-core agent runtime: pruned Rust CLI (`h3ph`) talking to a multi-tenant k3s sidecar for ephemeral SAST scans. | Locked egress and isolated reasoning — client nodes never see system prompts, tool contracts, or reasoning loops. |
| **Multi-Protocol Agent Transport**<br/>*(Private)* | Go + Rust proxy racing QUIC / Hysteria2 / TLS / SSH, promoting the first-healthy stream under 200ms. | Keeps agent tool-call round-trips within budget even under captive portals, mobile NATs, or restrictive firewalls. |
| **lzt-broker-stall-reaper**<br/>([Releases](https://github.com/LOUST-PRO/lzt-broker-stall-reaper/releases) · [Repo](https://github.com/LOUST-PRO/lzt-broker-stall-reaper)) | TCP-level Linux OS watchdog in Go enumerating sockets via `ss -tnpi` and firing `tcp_diag` kernel RST on stalled long-polls. | Auto-recovers GitHub Actions runner fleets when upstream broker sockets hang indefinitely without manual intervention. |
| **LinkMarks**<br/>([Releases](https://github.com/LOUST-PRO/LinkMarks/releases) · [Repo](https://github.com/LOUST-PRO/LinkMarks)) | 2.5 MB single-binary bookmark engine in Rust with CRDT multi-device sync under AGPLv3 + Commercial dual license. | Replaces heavy containerized web tools with zero-telemetry egress and deterministic canonical URL deduplication. |
| **outlook-mcp-suite**<br/>([Repo](https://github.com/LOUST-PRO/outlook-mcp-suite)) | Go 1.21 stdio MCP server with **22 tools** spanning Path A (Microsoft Graph API + OAuth 2.0 Device Code Flow) and Path C (web.outlook.com Playwright automation, ToS-sensitive), plus a defense-in-depth hook chain. | Multi-path agent access to Microsoft 365 mailboxes via clean stdio JSON-RPC — no client secrets required in Path A. |
| **TaxonRouter**<br/>([Releases](https://github.com/LOUST-PRO/TaxonRouter/releases) · [Repo](https://github.com/LOUST-PRO/TaxonRouter)) | Dual-binary GitHub automation in Go: MCP stdio server + webhook auto-tagger microservice managing issue/PR triage. | Automated GitHub issue/PR auto-tagging, label reconciliation, and zero-dependency webhook ingestion. |
| **nexus-engine**<br/>*(Private, multi-tenant recovery)* | Single-tenant recovery plane and backend orchestrator backing the LOUST multi-tenant SaaS — handles tenant snapshots, schema migrations, and rollback drills. | Self-healing infrastructure substrate for client-facing SaaS deployments (not a public artifact). |

<p align="center">
<p align="center">
  <a href="https://github.com/LOUST-PRO"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/banner-loust-pro-org.svg" width="100%" alt="LOUST-PRO Open Source &amp; Enterprise Substrates"/></a>

<table width="100%">
<table width="100%">
  <tr>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #f59e0b; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-amber.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
⚡ <a href="https://github.com/LOUST-PRO/NetBoozt_InternetUpgrade/releases" style="color: #38bdf8; text-decoration: none;"><b>NetBoozt — 網路效能、DNS 備援與通訊端調整</b></a>
        </h4>
        </h4>
跨平台網路效能升級及插槽調整引擎，採用 Rust、Tauri 與原生 C 網路程式碼打造。特色包括專為 Windows 和 Linux 設計的實驗性<b>備援 DNS 模組</b>，可繞過不穩定的 ISP DNS 伺服器與電信數據機解析停滯，並具備 TCP 視窗自動調整、BBR/Cubic 壅塞控制選擇、<code>TCP_NODELAY</code>、QoS DSCP 優先排序及 MTU/MSS 探索功能。
        </p>
        </p>
⚡ <b>重點功能：</b> +15-20% 吞吐量提升 · ISP/數據機 Fallback DNS 模組 · Windows & Linux 版本 · BBR/Cubic 調校
        </p>
        </p>
        <div>
          &nbsp;
          <a href="https://github.com/LOUST-PRO/NetBoozt_InternetUpgrade"><img src="https://img.shields.io/badge/NetBoozt_Repo-Explore-1E293B?style=flat-square&logo=github&logoColor=white" alt="NetBoozt Repo"/></a>
          <a href="https://github.com/LOUST-PRO/NetBoozt_InternetUpgrade"><img src="https://img.shields.io/badge/NetBoozt_Repo-Explore-1E293B?style=flat-square&logo=github&logoColor=white" alt="NetBoozt Repo"/></a>
        </div>
      </div>
    </td>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #0093d0; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-cyan.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
🔐 <a href="https://github.com/LOUST-PRO/SnapPipe" style="color: #38bdf8; text-decoration: none;"><b>SnapPipe — 身份識別與加密傳輸</b></a>
        </h4>
        </h4>
以 Rust 編寫的高效能身份傳輸與金鑰交換協定。強制執行零信任密碼學交握、點對點工作階段隔離，以及跨越非受管邊緣節點的零出口狀態同步。
        </p>
        </p>
⚡ <b>亮點：</b>零信任密碼學交握 · P2P 連線階段隔離 · 純 Rust 核心。
        </p>
        </p>
        <div>
          <a href="https://github.com/LOUST-PRO/SnapPipe"><img src="https://img.shields.io/badge/SnapPipe_Repo-Explore-0093D0?style=flat-square&logo=github&logoColor=white" alt="SnapPipe Repo"/></a>
        </div>
      </div>
    </td>
  </tr>
  <tr>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #00add8; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-emerald.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
🏷️ <a href="https://github.com/LOUST-PRO/TaxonRouter" style="color: #38bdf8; text-decoration: none;"><b>TaxonRouter — Webhook 自動標記微服務</b></a>
        </h4>
        </h4>
用於高吞吐量 B2B 事件驅動管道中即時負載分類、正則表達式路由和自動化 webhook 標記的並發 Go 微型服務，具有零記憶體配置。
        </p>
        </p>
⚡ <b>亮點：</b>零配置 Go 解析器 · 即時酬載分類 · 高並發
        </p>
        </p>
        <div>
          <a href="https://github.com/LOUST-PRO/TaxonRouter"><img src="https://img.shields.io/badge/TaxonRouter_Repo-Explore-00ADD8?style=flat-square&logo=github&logoColor=white" alt="TaxonRouter Repo"/></a>
        </div>
      </div>
    </td>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #de3a11; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-red.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
🧹 <a href="https://github.com/LOUST-PRO/LLMmempipe" style="color: #38bdf8; text-decoration: none;"><b>LLMmempipe — LLM 匯出清理工具 & 代幣效率優化 Markdown</b></a>
        </h4>
        </h4>
將雜訊 LLM 匯出資料（ChatGPT、Claude、Gemini）編譯成專為 Claude Code、Claude Projects 以及下游代理程式執行環境量身打造的權杖高效 JSONL 與 Markdown。跨多供應商語料庫的確定性結構描述、冪等重新攝取以及可重現重建。
        </p>
        </p>
⚡ <b>重點功能：</b>語法元高效化的 JSONL/Markdown · 多供應商正規化 · 適用於代理程式管道的等冪重新擷取
        </p>
        </p>
        <div>
          <a href="https://github.com/LOUST-PRO/LLMmempipe"><img src="https://img.shields.io/badge/LLMmempipe_Repo-Explore-DE3A11?style=flat-square&logo=github&logoColor=white" alt="LLMmempipe Repo"/></a>
        </div>
      </div>
    </td>
  </tr>
  <tr>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #8b5cf6; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-violet.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
🖼️ <a href="https://github.com/LOUST-PRO/paperforge" style="color: #38bdf8; text-decoration: none;"><b>paperforge — Linux 桌布引擎前端</b></a>
        </h4>
        </h4>
MIT 授權的 Rust 前端，專為 <b>linux-wallpaperengine 工作坊</b>設計。將 Steam 網路工作坊素材包裝成原生 Linux 渲染介面，具備確定性著色器播放、離線場景快取，以及 Vulkan 支援的合成器整合功能。獨立桌面應用程式 — 不是 RAG 管線。
        </p>
        </p>
⚡ <b>重點:</b> Steam Workshop 資源擷取 · Rust GTK4 原生 UI · 確定性著色器播放 &amp; 離線快取。
        </p>
        </p>
        <div>
          <a href="https://github.com/LOUST-PRO/paperforge"><img src="https://img.shields.io/badge/paperforge-Explore-8B5CF6?style=flat-square&logo=github&logoColor=white" alt="paperforge Repo"/></a>
        </div>
      </div>
    </td>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #10b981; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-emerald.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
🤝 <a href="https://github.com/LOUST-PRO/LZT-Developers" style="color: #38bdf8; text-decoration: none;"><b>LZT-Developers — YAML 開發目錄</b></a>
        </h4>
        </h4>
宣告式開發者名錄，位於 <a href="https://devs-github.loust.pro">devs-github.loust.pro</a>。貢獻者在 <code>/members</code> 下新增單一 YAML 檔案並提交 PR — 零衝突地整合至公開社群花名冊。在尋找開源專案、內部 CRM 及 B2B 契約人才時進行審閱。
        </p>
        </p>
⚡ <b>亮點：</b> YAML <code>/members</code> 目錄 · 零衝突入職流程 · devs-github.loust.pro 公開介面。
        </p>
        </p>
        <p style="margin: 0 0 6px 0; color: #cbd5e1; font-size: 12px; line-height: 1.4;">
          <b>How to join:</b>
        </p>
        <ol style="margin: 0 0 8px 0; padding-left: 18px; color: #94a3b8; font-size: 12px; line-height: 1.4;">
          <li>Fork the repo and create <code>members/&lt;your-github-username&gt;.yml</code> with <code>username</code>, <code>name</code>, <code>role</code>, <code>skills</code>, <code>github</code>.</li>
          <li>Open a Pull Request — CI validates the YAML schema.</li>
          <li>Once merged, your profile surfaces on <a href="https://devs-github.loust.pro">devs-github.loust.pro</a> within the next sync window.</li>
        </ol>
        <div>
          &nbsp;
          <a href="https://github.com/LOUST-PRO/LZT-Developers"><img src="https://img.shields.io/badge/Submit_YAML-PR-181717?style=flat-square&logo=github&logoColor=white" alt="Submit YAML PR"/></a>
          <a href="https://github.com/LOUST-PRO/LZT-Developers"><img src="https://img.shields.io/badge/Submit_YAML-PR-181717?style=flat-square&logo=github&logoColor=white" alt="Submit YAML PR"/></a>
        </div>
      </div>
    </td>
  </tr>
  <tr>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #0093d0; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-cyan.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
📅 <a href="https://github.com/LOUST-PRO/ical-to-caldav" style="color: #38bdf8; text-decoration: none;"><b>ical-to-caldav — iCal → CalDAV 橋接程式</b></a>
        </h4>
        </h4>
輕量級 Apache-2.0 程式，可將公開的 iCal（`.ics`）訂閱網址轉換為功能完整的 CalDAV 伺服器。支援與 khal、DankCalendar、Evolution、Thunderbird、GNOME Calendar 以及任何符合標準的 CalDAV 用戶端整合——無供應商鎖定，無 SaaS 來回傳輸。
        </p>
        </p>
⚡ <b>亮點：</b> 採用 Go 標準函式庫 · Apache-2.0 · 隨插即用 CalDAV 橋接器，適用於任何 <code>.ics</code> URL。
        </p>
        </p>
        <div>
          <a href="https://github.com/LOUST-PRO/ical-to-caldav"><img src="https://img.shields.io/badge/ical--to--caldav-Repo-0093D0?style=flat-square&logo=github&logoColor=white" alt="ical-to-caldav Repo"/></a>
        </div>
      </div>
    </td>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #7c3aed; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-violet.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
📚 <a href="https://github.com/LOUST-PRO/spec-snapshot-scraper" style="color: #38bdf8; text-decoration: none;"><b>spec-snapshot-scraper — AI就緒型文件語料庫</b></a>
        </h4>
        </h4>
用於建立 AI 就緒文件語料庫的快照工具。支援網路爬蟲、GitHub 樹狀結構和網址列表，並具有確定性版本控制、變更追蹤和 YAML 中繼資料標頭。設計為 Sovereign RAG 攝取管線和離線規格鏡像的上游基底。
        </p>
        </p>
⚡ <b>亮點：</b> Web/GitHub/URL 擷取 · YAML 中繼資料標頭 · 離線 RAG 的版本化快照。
        </p>
        </p>
        <div>
          <a href="https://github.com/LOUST-PRO/spec-snapshot-scraper"><img src="https://img.shields.io/badge/spec--snapshot--scraper-Repo-7C3AED?style=flat-square&logo=github&logoColor=white" alt="spec-snapshot-scraper Repo"/></a>
        </div>
      </div>
    </td>
  </tr>
  <tr>
    <td valign="top" width="100%">
      <div style="background: #0f172a; border-left: 4px solid #e91e63; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-pink.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
🔎 <a href="https://github.com/louzt/serpapi-mcp" style="color: #38bdf8; text-decoration: none;"><b>serpapi-mcp — 多引擎搜尋 MCP 伺服器</b></a>
        </h4>
        </h4>
Go stdio MCP 程式提供<b>SerpApi 多引擎搜尋</b>（Google + 20+ 個引擎）的存取，並透過 OAuth 2.0 + JWT 驗證管道、依據 RFC 6570 的動態<code>ResourceTemplate</code>具現化，以及 Anthropic Research 協定遵循。包含設計的 OIDC 代理、密碼學狀態對應用於探索驗證、決定性垃圾回收規則，以及記憶體優先權限制以優化活躍內容阈值。
        </p>
        </p>
⚡ <b>亮點：</b> 透過 <code>ResourceTemplate</code> 延遲展開，握手酬載縮減約 97.5% · OAuth 2.0 + JWT · Anthropic Research 協定 · 多引擎扇出。
        </p>
        </p>
        <div>
          <a href="https://github.com/louzt/serpapi-mcp"><img src="https://img.shields.io/badge/serpapi--mcp-Repo-E91E63?style=flat-square&logo=github&logoColor=white" alt="serpapi-mcp Repo"/></a>
        </div>
      </div>
    </td>
  </tr>

<details>
<details>

- **已交付超過 85 萬行程式碼**，橫跨 50 個以上專案（2019–2026）
- **知識圖譜緊縮與分類**：SPARQL/TriG 語料庫索引，消化歷史議題、PR 和提交差異與本機分支的對比，實現零開銷 token 預算及多分支差異分析
- **自訂 SAST 與 OSINT 弱點掃描工具**：問題導向的靜態分析規則及公開 OSINT 威脅情報對應，在修補程式提交前針對本機程式碼庫記錄回歸問題
- **跨分支差異測試工具**：多分支模擬套件，測量候選修補程式與上游分支間的執行延遲、記憶體佔用及狀態不變性
- **Nexus Engine 單體倉庫中 9 個套件和 391 個 TypeScript 檔案**
- **生產環境 B2B 多租戶引擎中 42 個 Prisma 模型和 600 多個 GraphQL 端點**
- **企業級多租戶 RBAC 隔離**與自主代理工作流程
- **FOSS 社群 CLA、DMCA 及可接受使用政策（AUP）** 法律治理框架
- **GPU 導向 RAG 檢索管線中 50K 嵌入向量在 188 毫秒內完成查詢**
- **NetBoozt TCP 最佳化基準測試在 Windows 上提升 15-20% 吞吐量**
- **SYPREME 轉換歸屬管線中從詢價到報價的回應延遲低於 2 分鐘**
- **原子性 CFDI 4.0 開票管線**（多租戶電子商務 + Stripe / MercadoPago / 加密貨幣）
- **Redis 頻道數從 59 降至 18**，透過 KEYS 遷移至 SCAN/COUNT

</details>


<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/section-what-we-ship.svg" width="100%" alt="What we ship at loust.pro — Software company section banner"/></p>

我工作的技術供應商——多協定向傳輸、強化 Linux 底層，以及能撐過多年期的 B2B 平台。公開產出物放在 **Research & Publications** 和 **Investigations & Notes**；這個區塊是我日常運作的產品面向。

<p align="right"><sub><em>LOUST · Leverage Opportunities Unleashing Success and Transformation</em></sub></p>

<table width="100%">
<table width="100%">
  <tr>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #38bdf8; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <h4 style="margin: 0 0 6px 0; color: #f8fafc;">
🏢 <b>企業內容管理系統</b>
        </h4>
        </h4>
多租戶內容、電子商務及營運平台，從單一程式碼庫驅動動態行銷、輕量級 ERP 工作流程、預訂系統及店面，支援零停機結構演進。
        </p>
        </p>
⚡ <b>亮點：</b> 每個租戶的獨立 Postgres/Redis 命名空間 · 13.5 萬行 Schema · APQ 命中率 90.9%
        </p>
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
⚡ <b>自動化引擎</b>
        </h4>
        </h4>
用於客戶操作的イベント驅動規則與網路鉤子引擎。將 Meta CAPI、Google Ads、Stripe、MercadoPago 和 CFDI 4.0 發票整合至具有重播功能且可稽核的管線中。
        </p>
        </p>
⚡ <b>亮點：</b>零資料遺失追蹤 · 亞秒級 webhook 擷取 · 事件重播與稽核日誌。
        </p>
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
📊 <b>CRM Hub</b>
        </h4>
        </h4>
為高壓銷售團隊設計的管線、聯絡人及成交介面。提供即時潛在客戶擷取及多租戶管線隔離。
        </p>
        </p>
⚡ <b>亮點：</b> 在展覽負載下從商機到報價延遲少於 2 分鐘 · 原生多租戶隔離。
        </p>
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
🌐 <a href="https://socialspheremx.loust.pro" style="color: #38bdf8; text-decoration: none;"><b>SocialSphereMX — 多租用戶 SaaS、ERP 與 MarTech 架構</b></a>
        </h4>
        </h4>
多租戶 SaaS 架構與 MarTech 生態系統，為代理商、內容創作者、PropTech 房地產及飯店旅遊企業打造。特色功能包括互動式數位媒體工具包，具備即時 API 中繼資料串流（Spotify/YouTube）、雲端原生餐廳 ERP（QR 菜單、即時廚房顯示系統、服務生介面）、即時房產庫存追蹤，以及低延遲潛在客戶工作流程。現任技術長與主要 SaaS 架構師。
        </p>
        </p>
⚡ <b>亮點：</b>多租戶 SaaS 核心 · 即時 Spotify/YouTube 攝取 · 餐廳 KDS 與 QR ERP · PropTech 庫存管理 · 99.9% 正常運作時間。
        </p>
        </p>
        <div>
          <img src="https://img.shields.io/badge/Next.js_16-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js 16"/>
          <img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React"/>
          <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
          <img src="https://img.shields.io/badge/Prisma-3982CE?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/>
          <img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL"/>
          <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
          <img src="https://img.shields.io/badge/Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white" alt="Stripe"/>
          <img src="https://img.shields.io/badge/Cloudflare_Edge-F38020?style=flat-square&logo=cloudflare&logoColor=white" alt="Cloudflare Edge"/>
        </div>
      </div>
    </td>
  </tr>
  <tr>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #6366f1; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <h4 style="margin: 0 0 6px 0; color: #f8fafc;">
🛠️ <b>Nexus Apps</b>
        </h4>
        </h4>
規格驅動產生器套件與單一倉儲架構系統，從單一事實來源維持跨多應用程式部署的結構一致性。
        </p>
        </p>
⚡ <b>亮點：</b> 9 個套件 &amp; 391 個 TypeScript 檔案 · 確定性程式生成 · 共用類型
        </p>
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
🛒 <b>市集</b>
        </h4>
        </h4>
多供應商電子商務平台，具備自動化 CFDI 4.0 稅務發票開立功能、透過 Stripe Connect 和 MercadoPago 的分潤分帳，以及賣家目錄驗證機制。
        </p>
        </p>
⚡ <b>亮點：</b>原子稅務帳單處理管線 · 多幣別支付分潤 · 可稽核帳本
        </p>
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
🤖 <b>AI 聊天機器人</b>
        </h4>
        </h4>
具備 ReAct 推理迴圈與動態供應商容錯移轉（M3、MiniMax M3、ChatGPT、Claude、DeepSeek、Gemini、Llama）的多租戶對話式 AI 介面，以及 CRM 匯出功能。
        </p>
        </p>
⚡ <b>亮點：</b>限制的權杖重試預算 · 租用戶隔離的 Redis 記憶體 · 即時人工接管
        </p>
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
📚 <b>公開研究筆記</b>
        </h4>
        </h4>
長篇研究筆記、論文草稿，以及關於主權式 RAG、傳輸層強化、核心回歸問題和基礎設施稽核的開放取用安全性報告。
        </p>
        </p>
⚡ <b>亮點：</b>預設公開的研發 · 形式定理與概念驗證 · 機器可讀取的 MDX
        </p>
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


<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/section-research-and-publications.svg" width="100%" alt="Research and Publications — section banner"/></p>

我在日常工作中維護的長篇研究筆記、論文草稿及證明鏈。每個條目都包含具體的產出（摘要、草稿或量測）——而非抽象的抱負。

<blockquote style="border-left: 4px solid #8b5cf6; background: #0f172a; padding: 20px; margin: 20px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
<blockquote style="border-left: 4px solid #8b5cf6; background: #0f172a; padding: 20px; margin: 20px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
🔬 <b>透過簽章雜湊投影的決定論式主權 RAG</b>（論文草稿，2026）
    <img src="https://img.shields.io/badge/Paper_Draft-7C3AED?style=flat-square&logo=latex&logoColor=white" align="right" alt="Paper Draft"/>
    <img src="https://img.shields.io/badge/Paper_Draft-7C3AED?style=flat-square&logo=latex&logoColor=white" align="right" alt="Paper Draft"/>
  </h4>
    A formal four-formula operator stack for zero-prefill, reproducible retrieval across sovereign cloud corpora without third-party vector database dependencies: <b>FNV-1a 64-bit feature hashing</b> into a fixed <code>D = 128</code> vector space, <b>$L_2$ spherical normalization</b>, cosine distance reduced to a direct dot product on the unit hypersphere $\mathbb{S}^{D-1}$, and a <b>pagination throughput window</b> ($R_{\text{throughput}}$) for upstream API rate-limit optimization.
  </p>
  </p>
  <p style="margin: 0 0 10px 0; color: #cbd5e1; font-size: 13px; line-height: 1.5;">
    <b>Mathematical Foundations &amp; Seven Theorems:</b>
  </p>
    <li><b>Theorem 1 (Estimator Unbiasedness):</b> Proves $\mathbb{E}[\langle \mathbf{v}, \mathbf{w} \rangle] = \langle \mathbf{x}, \mathbf{y} \rangle$, ensuring feature hashing preserves expected inner products across unigram/bigram document tokens.</li>
    <li><b>Theorem 1 (Estimator Unbiasedness):</b> Proves $\mathbb{E}[\langle \mathbf{v}, \mathbf{w} \rangle] = \langle \mathbf{x}, \mathbf{y} \rangle$, ensuring feature hashing preserves expected inner products across unigram/bigram document tokens.</li>
    <li><b>Theorem 2 (Variance Bounds via Weinberger 2009):</b> Bounds variance $\text{Var}(\langle \mathbf{v}, \mathbf{w} \rangle) \le \frac{2}{D} \|\mathbf{x}\|_2^2 \|\mathbf{y}\|_2^2$, demonstrating linear variance decay as projection dimension $D$ scales.</li>
    <li><b>Theorem 3 (Exponential Concentration via Hanson–Wright):</b> Establishes non-asymptotic sub-exponential tail bounds $\mathbb{P}(|\langle \mathbf{v}, \mathbf{w} \rangle - \langle \mathbf{x}, \mathbf{y} \rangle| > \epsilon) \le 2 \exp(-c \min(\frac{\epsilon^2 D}{K^4}, \frac{\epsilon D}{K^2}))$, guaranteeing collision suppression without dense neural embeddings.</li>
    <li><b>Theorem 4 (Spatial Complexity):</b> Proves fixed $O(D)$ memory allocation per document vector, eliminating unbounded vector DB index bloat.</li>
    <li><b>Theorem 5 &amp; 6 (Spherical Equivalence &amp; Scale Invariance):</b> Demonstrates $1 - \cos(\mathbf{v}, \mathbf{w}) = 1 - \langle \mathbf{v}, \mathbf{w} \rangle$ on $\mathbb{S}^{D-1}$, transforming cosine search into hyper-fast SIMD dot products.</li>
  </ul>
  </ul>
💡 <b>執行摘要與財務影響翻譯：</b><br/>
    <i>Why this matters for your organization:</i> This mathematical stack enables your platform to query millions of internal enterprise documents locally with <b>zero third-party vector database bills</b> (saving $2K–$10K/mo on Pinecone/Weaviate) and sub-microsecond retrieval (<b>640 nanoseconds</b>). For engineering leadership, it proves an ability to architect mathematical, zero-cost, model-free AI systems that never crash under traffic bursts and keep 100% of proprietary enterprise data strictly sovereign within your infrastructure.
  </p>
  </p>
    <b>Empirical Production Benchmarks:</b> Tested on a <b>4,458-document operator corpus</b> — full index creation completed in <b>4.14 s</b> ($\sigma = 0.18\text{ s}$), top-5 vector match latency of <b>640 ns</b> ($\sigma = 85\text{ ns}$), achieving <b>0.78 top-5 recall</b>. A 25-worker concurrent stress test on the production Rust implementation (<code>DSVH</code>) validated zero lock contention and stable memory usage.
  </p>
  </p>
  <p align="center" style="margin: 12px 0;">
    <a href="https://gist.github.com/louzt/3063245e9e42b2a5b100e0f72bc4387a"><img src="https://img.shields.io/badge/HexCortex-Edge_Deployment_Kit-7C3AED?style=for-the-badge&logo=c&logoColor=white" alt="HexCortex Edge Deployment Kit"/></a>
    &nbsp;
    <a href="https://gist.github.com/louzt/a75f9cf1a2f2edbd5af0e8d23526871d"><img src="https://img.shields.io/badge/Leer_las_matem%C3%A1ticas-Espa%C3%B1ol-D97706?style=for-the-badge&logo=github&logoColor=white" alt="Leer las matemáticas del Sovereign RAG (Español)"/></a>
    &nbsp;
    <a href="https://github.com/LOUST-PRO/deterministic-sovereign-rag"><img src="https://img.shields.io/badge/Rust_Implementation-DSVH-0093D0?style=for-the-badge&logo=rust&logoColor=white" alt="DSVH Rust Repo"/></a>
    <a href="https://github.com/LOUST-PRO/deterministic-sovereign-rag"><img src="https://img.shields.io/badge/Rust_Implementation-DSVH-0093D0?style=for-the-badge&logo=rust&logoColor=white" alt="DSVH Rust Repo"/></a>
  </p>
技術堆疊：Rust（DSVH）+ Go（APG）+ Virtuoso 7.2.6 + FNV-1a 64 位元 + L2 正規化。
待解問題：針對稠密嵌入器（BGE-M3、多語言）進行的實證比較——留待後續研究。
  </p>
  </p>

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider.svg" width="100%" alt="divider"/></p>

<blockquote style="border-left: 4px solid #38bdf8; background: #0f172a; padding: 20px; margin: 20px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
<blockquote style="border-left: 4px solid #38bdf8; background: #0f172a; padding: 20px; margin: 20px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
⚡ <b>135k 行 GraphQL 結構描述上的大規模 APQ</b>（案例研究，2026）
    <img src="https://img.shields.io/badge/Case_Study-0284C7?style=flat-square&logo=graphql&logoColor=white" align="right" alt="Case Study"/>
    <img src="https://img.shields.io/badge/Case_Study-0284C7?style=flat-square&logo=graphql&logoColor=white" align="right" alt="Case Study"/>
  </h4>
用於高吞吐量 GraphQL API 的生產環境實證數據：<b>90.9% 快取命中率、p95 延遲時間 12 毫秒、+125% 吞吐量提升、每月 $0 的額外基礎設施支出</b>，此乃 LOUST 多租戶 Next.js 16 + Apollo Server v4 技術堆疊在處理龐大的 13.5 萬行 Prisma 衍生的 GraphQL 結構描述時所達成。
  </p>
  </p>
  <p style="margin: 0 0 10px 0; color: #cbd5e1; font-size: 13px; line-height: 1.5;">
    <b>Architecture &amp; Seven Formal Theorems:</b>
  </p>
    <li><b>Theorem A.1 (APQ Hit Rate Under Zipf Traffic):</b> Derives $P(\text{hit}) \ge 1 - \frac{\zeta(s, N_{uncached}+1)}{\zeta(s)}$, proving why edge query hashing converges to >90% hit rates under realistic user access distributions.</li>
    <li><b>Theorem A.1 (APQ Hit Rate Under Zipf Traffic):</b> Derives $P(\text{hit}) \ge 1 - \frac{\zeta(s, N_{uncached}+1)}{\zeta(s)}$, proving why edge query hashing converges to >90% hit rates under realistic user access distributions.</li>
    <li><b>Eight Diagnostic Anchors:</b> Evaluates cgroup v2 <code>compile-runner.slice</code> CPU isolation, Circuit Breaker convergence, Zipf coverage, and Linux PSI memory pressure detection.</li>
    <li><b>Eight Diagnostic Anchors:</b> Evaluates cgroup v2 <code>compile-runner.slice</code> CPU isolation, Circuit Breaker convergence, Zipf coverage, and Linux PSI memory pressure detection.</li>
  </ul>
💡 <b>執行摘要與財務影響翻譯：</b><br/>
    <i>Why this matters for your organization:</i> Large enterprise schemas (700+ models, 2,000+ endpoints) typically require forced multi-server database upgrades ($15K–$50K/yr) due to server-side query parsing overhead and massive JSON payloads. By persist-hashing queries at the edge (90.9% hit rate) and applying cgroup v2 build isolation, we achieved a <b>+125% capacity increase at $0/mo incremental cloud spend</b>. For engineering directors and CTOs, this demonstrates elite systems mastery that directly protects company profit margins.
  </p>
  </p>
  <p align="center" style="margin: 12px 0;">
    &nbsp;
    <a href="https://gist.github.com/louzt/0c91771bf6370f0eb47e905934ab47e8"><img src="https://img.shields.io/badge/Leer_el_caso_de_estudio-Espa%C3%B1ol-D97706?style=for-the-badge&logo=github&logoColor=white" alt="Leer el caso de estudio APQ (Español)"/></a>
    <a href="https://gist.github.com/louzt/0c91771bf6370f0eb47e905934ab47e8"><img src="https://img.shields.io/badge/Leer_el_caso_de_estudio-Espa%C3%B1ol-D97706?style=for-the-badge&logo=github&logoColor=white" alt="Leer el caso de estudio APQ (Español)"/></a>
  </p>
堆疊：Next.js 16 <code>cacheComponents</code> + Apollo Server v4 + <code>ApolloAPQCache</code> + Redis 7 <code>ioredis</code> keyPrefix + Lua EVAL atomic + cgroup v2 <code>compile-runner.slice</code> + 自架 GitHub Actions runner 搭配持久性 <code>/opt/build-cache</code> 磁碟區。
  </p>
  </p>

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider.svg" width="100%" alt="divider"/></p>

<blockquote style="border-left: 4px solid #10b981; background: #0f172a; padding: 20px; margin: 20px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
<blockquote style="border-left: 4px solid #10b981; background: #0f172a; padding: 20px; margin: 20px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
📡 <b>零預填充保持連線協定與多區域時脈漂移</b>（運算子堆疊論文草稿，2026）
    <img src="https://img.shields.io/badge/Protocol_Spec-10B981?style=flat-square&logo=go&logoColor=white" align="right" alt="Protocol Spec"/>
    <img src="https://img.shields.io/badge/Protocol_Spec-10B981?style=flat-square&logo=go&logoColor=white" align="right" alt="Protocol Spec"/>
  </h4>
一個輕量級、確定性的 keep-alive 探測協定，用於上游 GPU 叢集和多區域 AI 代理程式控制平面。使用單一 <code>max_tokens=1</code> 探測，透過動態 5 分鐘 Weibull 心跳節奏評估快取預熱 TTL 狀態，在 <code>5,000 req/hour</code> 速率限制下，將 VRAM 重新預填充成本降低<b>800× 相較於冷啟動</b>，並<b>50× 相較於重新壓縮週期</b>。
  </p>
  </p>
  <p style="margin: 0 0 10px 0; color: #cbd5e1; font-size: 13px; line-height: 1.5;">
    <b>Core Theoretical &amp; Systems Bounds:</b>
  </p>
    <li><b>Marzullo's 1994 Intersection Algorithm:</b> Bounds multi-region clock drift $\Delta t \le \epsilon_{\text{ntp}} + \delta_{\text{drift}}$ across distributed agent nodes.</li>
    <li><b>Lamport Monotonic Happened-Before Ordering:</b> Enforces Strict POSIX <code>CLOCK_MONOTONIC</code> clock synchronization across RPC spans.</li>
    <li><b>Weibull Survival Distribution:</b> Models VRAM cache eviction probability $\lambda(t) = \frac{k}{\lambda}\left(\frac{t}{\lambda}\right)^{k-1}$ under non-stationary LLM token workloads.</li>
  </ul>
  </ul>
💡 <b>執行摘要與財務影響翻譯：</b><br/>
    <i>Why this matters for your organization:</i> Upstream LLM APIs and GPU clusters suffer from high "cold start" latency and expensive context re-prefilling when idle. By running a 5-minute Weibull heartbeat probe (<code>max_tokens=1</code>), we keep GPU VRAM context hot for <b>800× cheaper than cold starts</b> and <b>50× cheaper than re-compression cycles</b>. For VPs of Engineering and HR leadership, this proves rare operational maturity: zero wasted token burn, sub-second AI response times, and clock-drift-immune multi-region deployments.
    <i>Why this matters for your organization:</i> Upstream LLM APIs and GPU clusters suffer from high "cold start" latency and expensive context re-prefilling when idle. By running a 5-minute Weibull heartbeat probe (<code>max_tokens=1</code>), we keep GPU VRAM context hot for <b>800× cheaper than cold starts</b> and <b>50× cheaper than re-compression cycles</b>. For VPs of Engineering and HR leadership, this proves rare operational maturity: zero wasted token burn, sub-second AI response times, and clock-drift-immune multi-region deployments.
  </p>
堆疊：Go (APG) + Rust (DSVH) + Lamport happens-before 排序 + Marzullo 1994 交集邊界 + CLOCK_MONOTONIC + Weibull 存活邊界。記錄於 Sovereign RAG 操作員論文的 §5、§8、§9 及 §12。
  </p>
  </p>

<blockquote style="border-left: 4px solid #f59e0b; background: #0f172a; padding: 20px; margin: 24px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
<blockquote style="border-left: 4px solid #f59e0b; background: #0f172a; padding: 20px; margin: 24px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
  <h4 style="margin: 0 0 10px 0; color: #f8fafc;">
💰 <b>經濟分析＆基礎設施成本規避模型</b>
  </h4>
  </h4>
除了理論上的正確性之外，底層硬化是<b>生產工程的經濟槓桿</b>。在 2026 年後的計量式 AI 定價制度與計量式 CI/CD 執行器帳單下，底層回歸會直接複利累積成營運消耗。我們的經驗性硬化技術堆疊可在四個主要方向上提供可測量、可量化的成本規避：
  </p>
  </p>
  <ul style="margin: 0 0 12px 0; padding-left: 20px; color: #94a3b8; font-size: 13px; line-height: 1.5;">
    <li><b>Metered-AI API &amp; Token Avoidance:</b> Deterministic Sovereign RAG (<code>DSVH</code>) bounds vector projection costs as a function of corpus size rather than token throughput or third-party rate cards. The <code>Zero-Prefill Keep-Alive Protocol</code> reduces token probe burn by <b>800× vs cold starts</b> and <b>50× vs re-compression cycles</b> under <code>5,000 req/hour</code> rate limits.</li>
    <li><b>Database &amp; Edge Compute Capacity Lift:</b> Persisted GraphQL (APQ at 90.9% hit rate) + Brotli q11 compression achieves a <b>+125% throughput lift at $0/mo incremental infrastructure spend</b> on 135k-line schemas, eliminating the need for database scale-ups or serverless instance multiplier tiers.</li>
    <li><b>CI/CD Build-Runner Hours Reclaim:</b> Watchdog kernel RST (<code>lzt-broker-stall-reaper</code>) and POSIX process reapers (<code>PR_SET_PDEATHSIG</code>) eliminate zombie long-poll socket hangs and runaway worker processes, reclaiming <b>hundreds of billable runner hours per month</b> across GitHub Actions fleets.</li>

<details>
<details>

```python
# Substrate ROI & Financial Cost Avoidance Calculator
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
    # 2. CI/CD Runner Reclaim (preventing socket hangs & zombie leaks)
    runner_cost_reclaimed = (ci_runner_hours_monthly * 60) * ci_runner_minute_rate * 12
    # 3. Total Financial Savings
    # 3. Total Financial Savings
    total_cost_avoidance = token_cost_avoided + runner_cost_reclaimed + apq_baseline_serverless_cost
    return {
    return {
        "Token_API_Avoidance": f"${token_cost_avoided:,.2f}/yr",
        "CI_Runner_Reclaim": f"${runner_cost_reclaimed:,.2f}/yr",
        "APQ_Infra_Capacity_Lift": f"${apq_baseline_serverless_cost:,.2f}/yr",
        "Total_Annual_Cost_Avoidance": f"${total_cost_avoidance:,.2f}/yr"
    }
if __name__ == "__main__":
if __name__ == "__main__":
    print(calculate_substrate_savings())
```

<p align="center" style="margin-top: 12px;">
<p align="center" style="margin-top: 12px;">
  &nbsp;
  <a href="https://colab.research.google.com/"><img src="https://img.shields.io/badge/Run_in-Google_Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white" alt="Run in Google Colab"/></a>
  &nbsp;
  <a href="https://replit.com/"><img src="https://img.shields.io/badge/Run_on-Replit-66788F?style=for-the-badge&logo=replit&logoColor=white" alt="Run on Replit"/></a>
  &nbsp;
  <a href="https://onecompiler.com/python"><img src="https://img.shields.io/badge/Run_on-OneCompiler-38BDF8?style=for-the-badge&logo=python&logoColor=white" alt="Run on OneCompiler"/></a>
  <a href="https://onecompiler.com/python"><img src="https://img.shields.io/badge/Run_on-OneCompiler-38BDF8?style=for-the-badge&logo=python&logoColor=white" alt="Run on OneCompiler"/></a>
</p>
</details>

<blockquote style="border-left: 4px solid #06b6d4; background: #0f172a; padding: 20px; margin: 20px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
<blockquote style="border-left: 4px solid #06b6d4; background: #0f172a; padding: 20px; margin: 20px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
🧬 <b>HexCortex-H4-LRS — 第四類六角形細胞自動機研究套件</b> (INDAUTOR註冊, 2026)
    <img src="https://img.shields.io/badge/INDAUTOR-Registered-8B5CF6?style=flat-square&logo=googlescholar&logoColor=white" align="right" alt="INDAUTOR Registered"/>
    <img src="https://img.shields.io/badge/INDAUTOR-Registered-8B5CF6?style=flat-square&logo=googlescholar&logoColor=white" align="right" alt="INDAUTOR Registered"/>
  </h4>
本地研究套件，專門設計用於第四類六角形細胞自動機的分析、驗證與遙測，以正式科學軟體構件的形式建構，用於 IP 註冊（INDAUTOR）。超緊湊型 C99 程式引擎掌握香農熵追蹤、Floyd 環形偵測、對數雪崩直方圖及執行階段記憶體隔離——零負擔執行且零第三方依賴的高傳真數學遙測。目前正在積極開發中的網路安全 AST 生態系統之基礎核心。
  </p>
  </p>
  <p style="margin: 0 0 10px 0; color: #cbd5e1; font-size: 13px; line-height: 1.5;">
    <b>System Architecture &amp; Empirical Methods:</b>
  </p>
  <ul style="margin: 0 0 12px 0; padding-left: 20px; color: #94a3b8; font-size: 13px; line-height: 1.5;">
    <li><b>C99 execution kernel:</b> Floyd's cycle-finding for constant-memory transient analysis + logarithmic avalanche histograms measuring damage propagation across the hexagonal lattice.</li>
    <li><b>Deterministic classification layer:</b> BM25/TF-IDF bridge between theoretical queries and exact, auditable source-code hooks across the entire repository.</li>
    <li><b>Bun + TypeScript intelligence loop:</b> Local laboratory environment managing RAG queries, metadata validation, and SVG report generation; exports empirical findings as RDF triples for downstream knowledge-base queries.</li>
    <li><b>Process isolation &amp; portable probes:</b> Strict shell scripting dynamically compiles portable C probes to evaluate cellular reservoir signatures, event routing, and state collisions in complete isolation.</li>
  </ul>
  <p align="center" style="margin: 12px 0;">
    &nbsp;
    <a href="https://gist.github.com/louzt/079e249ae2452603088863037fc9c8d1"><img src="https://img.shields.io/badge/HexCortex-CART_Decision_Tree_C99-0EA5E9?style=for-the-badge&logo=c&logoColor=white" alt="HexCortex CART C99"/></a>
    &nbsp;
    <a href="https://gist.github.com/louzt/2b2cb125abaf6ee2df9deab03ff47a72"><img src="https://img.shields.io/badge/HexCortex-Split_Criteria_Comparison-22C55E?style=for-the-badge&logo=c&logoColor=white" alt="HexCortex Split Criteria Comparison"/></a>
    <a href="https://gist.github.com/louzt/2b2cb125abaf6ee2df9deab03ff47a72"><img src="https://img.shields.io/badge/HexCortex-Split_Criteria_Comparison-22C55E?style=for-the-badge&logo=c&logoColor=white" alt="HexCortex Split Criteria Comparison"/></a>
  </p>
堆疊：C99（無堆積，嵌入式友善）+ Bun + TypeScript + BM25/TF-IDF + Floyd 循環偵測 + Shannon 熵 + RDF 三元組匯出。作為正式科學軟體構件，於 INDAUTOR 登記，先於 AST 生態系 IP 申請案。
  </p>
  </p>

<blockquote style="border-left: 4px solid #e11d48; background: #0f172a; padding: 20px; margin: 20px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
<blockquote style="border-left: 4px solid #e11d48; background: #0f172a; padding: 20px; margin: 20px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
🎮 <b>Epic Games Zen Storage Server — I/O 抑制 &amp; JSON 串流架構</b> (<a href="https://github.com/EpicGames/zen-server/pull/711">PR #711</a>, Unreal Engine 5 DDC)
    <img src="https://img.shields.io/badge/Upstream_Contribution-E11D48?style=flat-square&logo=unrealengine&logoColor=white" align="right" alt="Upstream Contribution"/>
    <img src="https://img.shields.io/badge/Upstream_Contribution-E11D48?style=flat-square&logo=unrealengine&logoColor=white" align="right" alt="Upstream Contribution"/>
  </h4>
參與開發<b>Epic Games' Zen Storage Server</b> — 這是支撐 Unreal Engine 5 <b>Derived Data Cache (DDC)</b> 和資源烹飪管線的 C++20 分散式物件引擎。解決了上游 <code>main</code> (v5.8.18-pre3) 的深層結構性程式碼漂移問題，設計了用於無頭 Linux 容器和 systemd 環境的關鍵診斷隔離層，消除了 overlay2 檔案系統上繁重資源轉換期間的<b>分頁快取顛簸、區塊寫入放大（CoW 中繼資料膨脹）以及工作者飢餓</b>問題。
  </p>
  </p>
  <p style="margin: 0 0 10px 0; color: #cbd5e1; font-size: 13px; line-height: 1.5;">
    <b>Structural Re-architecture &amp; Validation:</b>
  </p>
  <ul style="margin: 0 0 12px 0; padding-left: 20px; color: #94a3b8; font-size: 13px; line-height: 1.5;">
    <li><b>Atomic path sanitization:</b> <code>--no-log-file</code> flag invokes <code>AbsLogFile.clear()</code> inside <code>ZenLoggingCmdLineOptions::ApplyOptions</code>, completely dropping file sink allocations for a <b>write-zero storage footprint</b> under overlay2.</li>
    <li><b>Sink lifecycle decoupling:</b> <code>FileSink</code> and <code>ConsoleSink</code> initialization split into independent sibling execution blocks, isolating user-space mutex contention so <code>fdatasync</code> blocking cannot propagate into kernel-level I/O Wait states that starve parallel engine workers.</li>
    <li><b>O(1) JSON telemetry:</b> <code>--log-json</code> offloads super-linear regex backtracking from external log collectors (Loki/Vector) into the native binary core, routing through <code>AsyncSink</code> to guarantee zero main-thread block regressions.</li>
    <li><b>API diff forensics:</b> Reconstructed stale telemetry configurations from archived public PRs to resolve complex git merge blocks on long-drifted upstream main.</li>
  </ul>
💡 <b>執行摘要與效能翻譯：</b><br/>
    <i>Why this matters for your organization:</i> Heavy Unreal Engine 5 asset cooking pipelines routinely saturate Linux overlay2 storage with Copy-on-Write metadata churn, causing parallel build workers to stall in uninterruptible I/O Wait. By forcing write-zero log files and decoupling sink lifecycles, we eliminated the amplification at the OS level rather than fighting it at the application level. For VPs of Engineering and CTOs, this delivers <b>stable CI throughput under heavy DDC loads, zero worker starvation, and zero behavioral regressions across 139 native unit test vectors</b>.
    <i>Why this matters for your organization:</i> Heavy Unreal Engine 5 asset cooking pipelines routinely saturate Linux overlay2 storage with Copy-on-Write metadata churn, causing parallel build workers to stall in uninterruptible I/O Wait. By forcing write-zero log files and decoupling sink lifecycles, we eliminated the amplification at the OS level rather than fighting it at the application level. For VPs of Engineering and CTOs, this delivers <b>stable CI throughput under heavy DDC loads, zero worker starvation, and zero behavioral regressions across 139 native unit test vectors</b>.
  </p>
技術架構：C++20 + ZenLoggingCmdLineOptions + AsyncSink + xmake + 139 個原生單元測試向量 + overlay2 感知 I/O 語意
  </p>
  </p>

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider.svg" width="100%" alt="divider"/></p>

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/section-investigations-and-notes.svg" width="100%" alt="Investigations and Notes — section banner"/></p>

公開研究筆記、作業取證，以及上游修補程式系列 — 按技術領域編入索引，配有可稽核的程式證明以及效能指標。

<p align="center" style="margin: 16px 0 8px 0;">
<p align="center" style="margin: 16px 0 8px 0;">
  <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/banner-domain-systems-kernel.svg" width="100%" alt="Systems, Vulkan and Kernel Hardening Domain Banner"/>

<table width="100%">
<table width="100%">
  <tr>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #eb0029; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-red.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
🎮 <b>Valve/Fossilize 著色器回放工具強化</b>
        </h4>
        </h4>
編寫了 <code>PR_SET_PDEATHSIG</code> + <code>getppid()</code> 競速條件檢查 (<a href="https://github.com/ValveSoftware/Fossilize/pull/305">PR #305</a>)，能在 Steam/Proton 當機時立即終止孤立的 Vulkan 著色器重播器。根除了全球數百萬台 Steam Deck / Linux 遊戲裝置上 100% CPU 工作執行緒洩漏及電力消耗問題。編寫了 <a href="https://github.com/ValveSoftware/Fossilize/pull/311">PR #311</code></a> <code>static_assert</code>，解除了 Valve 的 +7,913 LOC Mesa CI 稽核套件封鎖 (<a href="https://github.com/ValveSoftware/Fossilize/pull/310">PR #310</a>)。
        </p>
        </p>
⚡ <b>影響力：</b>全球排名第 7，與 <code>ValveSoftware/Fossilize</code> 主分支（2024–2026）的 DXVK 和 Mesa 核心維護者並列。
        </p>
        </p>
        <div>
          &nbsp;
          <a href="https://github.com/ValveSoftware/Fossilize/pull/308"><img src="https://img.shields.io/badge/PR_%23308-Merged-10B981?style=flat-square&logo=github&logoColor=white" alt="PR 308"/></a>
          &nbsp;
          <a href="https://github.com/ValveSoftware/Fossilize/pull/311"><img src="https://img.shields.io/badge/PR_%23311-Merged-10B981?style=flat-square&logo=github&logoColor=white" alt="PR 311"/></a>
          <a href="https://github.com/ValveSoftware/Fossilize/pull/311"><img src="https://img.shields.io/badge/PR_%23311-Merged-10B981?style=flat-square&logo=github&logoColor=white" alt="PR 311"/></a>
        </div>
      </div>
    </td>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #6366f1; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-cyan.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
🐧 <b>NVIDIA DKMS 核心 7.0+ 技術建議與 Optimus 熱插拔</b>
        </h4>
        </h4>
專為 Kernel 7.0 API 重構設計的前向相容 RFC 修補程式系列：VMA 鎖定（<code>__is_vma_write_locked()</code>）、DMA 柵欄訊號（<code>dma_fence_signal_locked()</code>）以及 <code>vm_flags_reset()</code>（<a href="https://gist.github.com/louzt/1c85044d5090d19223c3f5edf426a19e">RFC Gist</a>）。新增 <code>NVreg_DynamicPowerManagement=0x02</code> modprobe 規則，解決混合式筆記型電腦上 USB-C D3cold 熱插拔當機問題。
        </p>
        </p>
⚡ <b>影響：</b> 消除橫跨混合式 Optimus 筆電的核心崩潰和 GPU 懸掛/恢復鎖定問題。
        </p>
        </p>
        <div>
          <a href="https://gist.github.com/louzt/1c85044d5090d19223c3f5edf426a19e"><img src="https://img.shields.io/badge/NVIDIA_Kernel_7.0-RFC_Gist-76B900?style=flat-square&logo=nvidia&logoColor=white" alt="NVIDIA RFC Gist"/></a>
        </div>
      </div>
    </td>
  </tr>

<p align="center" style="margin: 16px 0 8px 0;">
<p align="center" style="margin: 16px 0 8px 0;">
  <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/banner-domain-audio-desktop.svg" width="100%" alt="Audio Subsystems and Desktop Compositors Domain Banner"/>

<table width="100%">
<table width="100%">
  <tr>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #38bdf8; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-emerald.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
🔊 <b>PipeWire &amp; 音訊子系統硬化</b>
        </h4>
        </h4>
在 <code>pw_protocol_native_connect_local_socket()</code> 上設計 5 秒 <code>spa timer</code> 協定原生連線逾時（<a href="https://github.com/louzt/pipewire/commit/2f747a7">commit 2f747a7</a>），消除永久性音訊指令列死結（<code>wpctl</code>/<code>pactl</code> 無回應）。記錄 Distrobox/LXC 下的 OpenAL Soft 和 ALSA 容器緩衝區溢位解決方案。
        </p>
        </p>
⚡ <b>影響：</b>在 Fedora、Arch、Ubuntu 和 SteamOS 上從鎖死的音訊插座中實現 100% 恢復。
        </p>
        </p>
        <div>
          &nbsp;
          <a href="https://gist.github.com/louzt/c175973d8e8bae8c8fef6af4d9d6aca7"><img src="https://img.shields.io/badge/OpenAL_Gist-Notes-7C3AED?style=flat-square&logo=github&logoColor=white" alt="OpenAL Gist"/></a>
          <a href="https://gist.github.com/louzt/c175973d8e8bae8c8fef6af4d9d6aca7"><img src="https://img.shields.io/badge/OpenAL_Gist-Notes-7C3AED?style=flat-square&logo=github&logoColor=white" alt="OpenAL Gist"/></a>
        </div>
      </div>
    </td>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #14b8a6; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-pink.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
🎵 <b>spotify-player &amp; rspotify 終端機生態系統</b>
        </h4>
        </h4>
啟用無頭終端機原生 Spotify 播放 (TUI)，具有作用中工作階段繼承且零 GUI 額外負荷。在 `spotify-player` 中將 `is_active` Connect 裝置存在狀態與作用中播放 (`is_playing`) 區分開來 (PR #1049)，解除待命喇叭上 `librespot` 音訊引擎的資源飢餓問題。將搜尋請求序列化 (PR #1048) 以消除 429 配額爆量問題。在 `rspotify` 中提議非破壞性的 Serde `#[serde(default)]` 結構描述漂移回退機制 (Issue #572)。
        </p>
        </p>
⚡ <b>影響：</b>無周邊介面 TUI 程式工作階段繼承、100% 消除 HTTP 429 速率限制尖峰與待命喇叭播放死結。
        </p>
        </p>
        <div>
          &nbsp;
          <a href="https://github.com/aome510/spotify-player/pull/1048"><img src="https://img.shields.io/badge/PR_%231048-Merged-10B981?style=flat-square&logo=github&logoColor=white" alt="PR 1048"/></a>
          &nbsp;
          <a href="https://github.com/ramsayleung/rspotify/issues/572"><img src="https://img.shields.io/badge/Issue_%23572-Triaged-38BDF8?style=flat-square&logo=github&logoColor=white" alt="Issue 572"/></a>
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
🖼️ <b>Wayland Compositor &amp; 顯示 IPC 診斷</b>
        </h4>
        </h4>
主導了基於拉取的类型化进程间通讯诊断、語義資產標記，以及橫跨 Niri Wayland 顯示管線的每輸出端互斥執行緒隔離（<a href="https://gist.github.com/louzt/1c5230a2e9471faf9ce4243314361fa1">5 PRs Gist</a>）。在 Waypaper 中橫跨 swww/awww 後端暴露縮放濾波器矩陣（<a href="https://github.com/louzt/761e227ad8cfe55b29e79cf861214a62">PR #286</a>）。
        </p>
        </p>
⚡ <b>影響：</b>在具有異質刷新率的多螢幕顯示器上實現零掉幀的幀率節奏控制。
        </p>
        </p>
        <div>
          &nbsp;
          <a href="https://github.com/louzt/761e227ad8cfe55b29e79cf861214a62"><img src="https://img.shields.io/badge/Waypaper-PR_%23286-38BDF8?style=flat-square&logo=github&logoColor=white" alt="Waypaper PR"/></a>
          <a href="https://github.com/louzt/761e227ad8cfe55b29e79cf861214a62"><img src="https://img.shields.io/badge/Waypaper-PR_%23286-38BDF8?style=flat-square&logo=github&logoColor=white" alt="Waypaper PR"/></a>
        </div>
      </div>
    </td>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #8b5cf6; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-violet.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
🌐 <b>Chromium 148 CSP 稽核與網路安全</b>
        </h4>
        </h4>
在 Chromium 148 中識別出跨來源 <code>srcdoc</code> 沙箱 CSP Level 3 策略碰撞回歸問題（<a href="https://gist.github.com/louzt/77f0804ca11bad6636f0ac67928bd384">Gist</a>）。在 Opera 安全揭露追蹤 GB-80414 下已被上游接受。
        </p>
        </p>
⚡ <b>影響：</b>可稽核的安全性分類、CSP 沙箱碰撞隔離，以及上游瀏覽器修補程式驗證。
        </p>
        </p>
        <div>
          &nbsp;
          <img src="https://img.shields.io/badge/Opera_Tracking-GB--80414-FF1B2D?style=flat-square&logo=opera&logoColor=white" alt="Opera GB-80414"/>
          <img src="https://img.shields.io/badge/Opera_Tracking-GB--80414-FF1B2D?style=flat-square&logo=opera&logoColor=white" alt="Opera GB-80414"/>
        </div>
      </div>
    </td>
  </tr>

<p align="center" style="margin: 16px 0 8px 0;">
<p align="center" style="margin: 16px 0 8px 0;">
  <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/banner-domain-network-security.svg" width="100%" alt="Resilient Network Transport and Web Security Domain Banner"/>

<table width="100%">
<table width="100%">
  <tr>
    <td valign="top" width="100%">
      <div style="background: #0f172a; border-left: 4px solid #f59e0b; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-amber.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
🛰️ <b>彈性傳輸代理程式 &amp; Linux 遙測</b>
        </h4>
        </h4>
設計 5 層備援傳輸代理，在 <200 毫秒內競速 QUIC / Hysteria2 / TLS / SSH，使用 CA 固定拓撲（<a href="https://gist.github.com/louzt/3991f144c7d67726045af3cefc60f42a">Gist</a>）。記錄 Linux PSI 輪詢監控和 Redis <code>KEYS</code> → <code>SCAN/COUNT</code> 零負擔可觀測性（<a href="https://gist.github.com/louzt/b8349629b602a782ac98d0cbfd0df0c0">Gist</a>）。
        </p>
        </p>
⚡ <b>影響：</b> Sub-200ms 傳輸穿越嚴格防火牆進行競速，且 Redis 頻道膨脹減少 70%。
        </p>
        </p>
        <div>
          &nbsp;
          <a href="https://gist.github.com/louzt/b8349629b602a782ac98d0cbfd0df0c0"><img src="https://img.shields.io/badge/Observability-PSI_Gist-10B981?style=flat-square&logo=github&logoColor=white" alt="Observability Gist"/></a>
          <a href="https://gist.github.com/louzt/b8349629b602a782ac98d0cbfd0df0c0"><img src="https://img.shields.io/badge/Observability-PSI_Gist-10B981?style=flat-square&logo=github&logoColor=white" alt="Observability Gist"/></a>
        </div>
      </div>
    </td>
  </tr>
  <tr>
    <td valign="top" width="100%">
      <div style="background: #0f172a; border-left: 4px solid #008000; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-green.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
🛡️ <b>NGINX 執行階段 CRLF 注入強化 &amp; 分支分離驗證</b>
        </h4>
        </h4>
NGINX 為全球<b>約 30% 的網站</b>提供支援，並且是 LOUST 多租戶堆疊的標準反向代理/TLS 終止器。記錄了一個透過 <code>$uri</code> 在 <code>proxy_pass</code>、<code>proxy_set_header</code>、<code>add_header</code> 和 <code>add_trailer</code> 指令中傳播的執行階段 CRLF 注入向量——這使得透過格式錯誤的上游變數進行任意 HTTP 標頭走私成為可能。編寫了具有 ApacheBench 測量的分支分割驗證工具，以及 nginx/nginx-tests 中的回歸測試。作為上游 PR <a href="https://github.com/nginx/nginx/pull/590">nginx#590</a>（執行階段 CRLF 清理）、<a href="https://github.com/nginx/nginx/pull/1414">#1414</a>（<code>add_header</code>/<code>add_trailer</code> 逸出）、<a href="https://github.com/nginx/nginx-tests/pull/55">nginx-tests#55</a> 和 <a href="https://github.com/nginx/nginx-tests/pull/58">#58</a>（<a href="https://gist.github.com/louzt/7bdf370a28126718e7e7b69d53b0ae86">Evidence Gist</a>）提交了強化修補程式。
        </p>
        </p>
⚡ <b>影響：</b> 強化 <code>ngx_http_proxy_module.c</code> + <code>ngx_http_headers_filter_module.c</code> 防止標頭偽造 · 4.6k–4.9k req/s ApacheBench 吞吐量在消毒處理下。
        </p>
        </p>
        <div>
          &nbsp;
          <a href="https://github.com/nginx/nginx/pull/590"><img src="https://img.shields.io/badge/PR-nginx%23590-009639?style=flat-square&logo=nginx&logoColor=white" alt="PR nginx#590"/></a>
          &nbsp;
          <a href="https://github.com/nginx/nginx/pull/1414"><img src="https://img.shields.io/badge/PR-nginx%231414-009639?style=flat-square&logo=nginx&logoColor=white" alt="PR nginx#1414"/></a>
          &nbsp;
          <a href="https://github.com/nginx/nginx-tests/pull/55"><img src="https://img.shields.io/badge/PR-tests%2355-009639?style=flat-square&logo=nginx&logoColor=white" alt="PR nginx-tests#55"/></a>
          <a href="https://github.com/nginx/nginx-tests/pull/55"><img src="https://img.shields.io/badge/PR-tests%2355-009639?style=flat-square&logo=nginx&logoColor=white" alt="PR nginx-tests#55"/></a>
        </div>
      </div>
    </td>
  </tr>

<p align="center" style="margin: 16px 0 8px 0;">
<p align="center" style="margin: 16px 0 8px 0;">
  <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/banner-domain-agents-cloud.svg" width="100%" alt="Sovereign Agent Fleets and Kubernetes Substrates Domain Banner"/>

<table width="100%">
<table width="100%">
  <tr>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #ec4899; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-pink.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
🤖 <b>主權代理艦隊溯源與 Git 聲明閘道</b>
        </h4>
        </h4>
設計確定性 <code>agent_id</code> 溯源標記與跨分層代理工作流程的子代理對話 ID 稽核追蹤。實作工作樹作者分類（我的 / 外部 / 混合 / 未知）並搭配自動化作者電子郵件歸屬閘道。工程化 F80.14 感知 <code>lzt-branch-claim</code> 驗證，防止自動化 PR 分片與多代理程式碼生成管線期間的並行代理分支偏移或競態條件（<a href="https://gist.github.com/louzt/3ba453b2876a4b105a9893b26541ffc3">Gist</a>）。
        </p>
        </p>
⚡ <b>影響：</b>零漂移多代理程式 git 分支宣告驗證與 100% 可稽核代理程式執行溯源。
        </p>
        </p>
        <div>
          <a href="https://gist.github.com/louzt/3ba453b2876a4b105a9893b26541ffc3"><img src="https://img.shields.io/badge/Agent_Provenance-Gist-EC4899?style=flat-square&logo=github&logoColor=white" alt="Provenance Gist"/></a>
        </div>
      </div>
    </td>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #326ce5; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-cyan.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
🎮 <b>H4KKEN 格鬥遊戲引擎 & GGPO 網路程式</b>
        </h4>
        </h4>
線上格鬥遊戲專案，具備<b>GGPO 風格 30 幀回滾網路程式</b>以及即時 P2P/無伺服器對戰協調。開發 WebRTC DataChannel 傳輸層，採用 Babylon.js 8 WebGPU 渲染以及逐幀輸入預測。在私有 VPS 上設計身份錨定工作階段綁定，位於 <a href="https://h4kken.loust.pro">h4kken.loust.pro</a>。公開成果尚未發布；所有設計文件與效能基準皆存放於 VPS 防火牆後方。
        </p>
        </p>
⚡ <b>影響：</b>H4KKEN 回溯網路程式 & P2P 對戰編排 · 次框架輸入預測 · 身份錨定工作階段繫結。
        </p>
        </p>
        <div>
          <a href="https://h4kken.loust.pro"><img src="https://img.shields.io/badge/H4KKEN-Live_VPS-326CE5?style=flat-square&logo=cloudflare&logoColor=white" alt="H4KKEN Live VPS"/></a>
        </div>
      </div>
    </td>
  </tr>
  <tr>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #4caf50; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <img src="https://raw.githubusercontent.com/louzt/louzt/main/static/lava-border-green.svg" width="100%" height="4" alt="Lava Lamp Glow Border"/>
        <h4 style="margin: 8px 0 6px 0; color: #f8fafc;">
⛏️ <b>Minecraft Servers on k3s 待機自動擴展</b>
        </h4>
        </h4>
設計無伺服器備用基礎設施與 RCON 驅動的自動擴展，適用於在 k3s / 輕量級 Kubernetes 上運行的兩個 Java 架構的 <b>Minecraft 伺服器</b>（Fabric 模組版 + Paper 原版）。透過 CronJob 設計自動化 RCON 狀態輪詢、原子性儲存/刷新，以及優雅節點關閉。當零名玩家在線時，匹配的 Pod 自動擴展至 0 個副本（回收約 8 GB RSS RAM），在新的玩家連線探測時實現快速暖開機旋轉啟動（<15s）（<a href="https://gist.github.com/louzt/b333b5601628a159630da13857834246">English Gist</a> · <a href="https://gist.github.com/louzt/8e3b86c7398016964699e87d52222cf7">Español</a>）。
        </p>
        </p>
⚡ <b>影響：</b> Minecraft Fabric+Paper 自動擴展 · RCON 驅動的閒置關機 · <15秒暖開機啟動 · 100% 閒置成本消除。
        </p>
        </p>
        <div>
          &nbsp;
          <a href="https://gist.github.com/louzt/8e3b86c7398016964699e87d52222cf7"><img src="https://img.shields.io/badge/Minecraft_k3s-Gist_ES-D97706?style=flat-square&logo=github&logoColor=white" alt="Minecraft k3s Gist (ES)"/></a>
          <a href="https://gist.github.com/louzt/8e3b86c7398016964699e87d52222cf7"><img src="https://img.shields.io/badge/Minecraft_k3s-Gist_ES-D97706?style=flat-square&logo=github&logoColor=white" alt="Minecraft k3s Gist (ES)"/></a>
        </div>
      </div>
    </td>
      &nbsp;
    </td>
    </td>
  </tr>

<blockquote style="border-left: 3px solid #10b981; background: #0f172a; padding: 20px; margin: 24px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
<blockquote style="border-left: 3px solid #10b981; background: #0f172a; padding: 20px; margin: 24px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
  <h4 align="center">💡 <b>What This Systems Engineering Posture Means For Your Platform</b></h4>
  <p>The formal proofs, upstream PRs, and kernel investigations above reflect a single operational rule: <b>we fix substrate root causes before scaling</b>.</p>
  <ul>
    <li><b>Zero-Regression Production Safety:</b> Compile-time safeguards (<code>static_assert</code>), process reapers (<code>PR_SET_PDEATHSIG</code>), and deterministic RAG bounds ensure your systems remain memory-leak-free and resilient under heavy traffic.</li>
    <li><b>Substrate-First Cost Efficiency:</b> Edge-persisted GraphQL (90.9% APQ hit rate) and Linux kernel TCP tuning keep infrastructure costs at $0/mo incremental overhead while lifting throughput by +125%.</li>
    <li><b>Zero-Trust Security & IP Protection:</b> Locked-egress agent runtimes, CA-pinned transport proxies, and auditable 72-hour vulnerability disclosure protect your business data and user trust.</li>
  </ul>
  <p align="center">
    &nbsp;
    <a href="mailto:security@loust.pro"><img src="https://img.shields.io/badge/Security_Triage-security%40loust.pro-38BDF8?style=for-the-badge&logo=hackerone&logoColor=white" alt="Security Triage"/></a>
    &nbsp;
    <a href="mailto:research@loust.pro"><img src="https://img.shields.io/badge/R%26D_Collaboration-research%40loust.pro-8B5CF6?style=for-the-badge&logo=orcid&logoColor=white" alt="R&D Collaboration"/></a>
    <a href="mailto:research@loust.pro"><img src="https://img.shields.io/badge/R%26D_Collaboration-research%40loust.pro-8B5CF6?style=for-the-badge&logo=orcid&logoColor=white" alt="R&D Collaboration"/></a>
  </p>

<p align="right"><sub><em>LOUST · Leverage Opportunities Unleashing Success and Transformation</em></sub></p>

> _公開的 gists 會在發布時個別連結於上方。如需私下進行中的工作與作業分析，請參閱 [LinkedIn](https://www.linkedin.com/in/davidmirelesll/?locale=es_ES) 以取得整理過的檢視。_

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider-bracket-closing.svg" width="100%" alt="closing bracket divider"/></p>

<!-- ============================================================ -->
<!-- ============================================================ -->
<!-- FOOTER: animated squares grid + tagline (no operator name).  -->
<!-- Served from profile-public static/ alongside the section     -->
<!-- banners. Editor-only provenance; GitHub strips the comment.  -->
<div align="center">
<div align="center">
  <img alt="Animated footer tagline" src="https://raw.githubusercontent.com/louzt/louzt/main/static/profile-footer.svg" width="100%" style="display:block;margin:0 auto"/>
