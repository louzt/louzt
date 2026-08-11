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
      <img src="https://img.shields.io/badge/Voc%C3%AA_est%C3%A1_lendo_em-Portugu%C3%AAs-009B3A?style=flat-square&logo=readme&logoColor=white" alt="Você está lendo em Português"/>
      <a href="https://github.com/louzt/louzt/blob/main/README.md"><img src="https://img.shields.io/badge/Read_in-English-0093D0?style=flat-square&logo=readme&logoColor=white" alt="Read in English"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.es.md"><img src="https://img.shields.io/badge/Leer_en-Espa%C3%B1ol-D97706?style=flat-square&logo=readme&logoColor=white" alt="Leer en Español"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.it.md"><img src="https://img.shields.io/badge/Leggi_in-Italiano-009246?style=flat-square&logo=readme&logoColor=white" alt="Leggi in Italiano"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.de.md"><img src="https://img.shields.io/badge/Auf-Deutsch_lesen-DD0000?style=flat-square&logo=readme&logoColor=white" alt="Auf Deutsch lesen"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.ja.md"><img src="https://img.shields.io/badge/%E6%97%A5%E6%9C%AC%E8%AA%9E%E3%81%A7-%E8%AA%AD%E3%82%80-BC002D?style=flat-square&logo=readme&logoColor=white" alt="日本語で読む"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.ko.md"><img src="https://img.shields.io/badge/%ED%95%9C%EA%B5%AD%EC%96%B4%EB%A1%9C-%EC%9D%BD%EA%B8%B0-0047A0?style=flat-square&logo=readme&logoColor=white" alt="한국어로 읽기"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.fr.md"><img src="https://img.shields.io/badge/Lire_en-Fran%C3%A7ais-0055A5?style=flat-square&logo=readme&logoColor=white" alt="Lire en Français"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.nl.md"><img src="https://img.shields.io/badge/In_het_Nederlands-lezen-21468B?style=flat-square&logo=readme&logoColor=white" alt="In het Nederlands lesen"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.sv.md"><img src="https://img.shields.io/badge/L%C3%A4s_p%C3%A5-Svenska-006AA7?style=flat-square&logo=readme&logoColor=white" alt="Läs på Svenska"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.zh-TW.md"><img src="https://img.shields.io/badge/%E9%96%B1%E8%AE%80%E7%B9%81%E9%AB%94%E4%B8%AD%E6%96%87-(%E5%8F%B0%E7%81%A3)-D97706?style=flat-square&logo=readme&logoColor=white" alt="閱讀繁體中文 (台灣)"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.pl.md"><img src="https://img.shields.io/badge/Czytaj_po-Polsku-DC143C?style=flat-square&logo=readme&logoColor=white" alt="Czytaj po Polsku"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.tr.md"><img src="https://img.shields.io/badge/T%C3%BCrk%C3%A7e-okuyun-E30A17?style=flat-square&logo=readme&logoColor=white" alt="Türkçe okuyun"/></a>
      <a href="https://github.com/louzt/louzt/blob/main/README.hi.md"><img src="https://img.shields.io/badge/%E0%A4%A8%E0%A5%80%E0%A4%9A%E0%A5%87_%E0%A4%A5%E0%A5%80-%E0%A4%B9%E0%A4%BF%E0%A4%A8%E0%A5%8D%E0%A4%A6%E0%A5%80-%E0%A4%B9%E0%A4%BF%E0%A4%A8%E0%A5%8D%E0%A4%A6%E0%A5%80-FF9933?style=flat-square&logo=readme&logoColor=white" alt="हिन्दी में पढ़ें"/></a>
    </td>
  </tr>
    <!-- Row 2: Contact channels & Schedule a meeting & Spoken Languages -->
    <td align="left" valign="middle">
    <td align="left" valign="middle">
      <a href="https://calendar.app.google/XR7FkZXWVwfmZ57x6"><img src="https://img.shields.io/badge/Agendar_uma_Reuni%C3%A3o-34A853?style=flat-square&logo=googlecalendar&logoColor=white" alt="Agendar uma Reunião (Google Calendar)"/></a>
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
      <a href="mailto:pesquisa@loust.pro"><img src="https://img.shields.io/badge/research%40loust.pro-7C3AED?style=flat-square&logo=protonmail&logoColor=white" alt="pesquisa@loust.pro"/></a>
      <a href="https://opensource.org/"><img src="https://img.shields.io/badge/OSI-Membro-3DA639?style=flat-square&logo=opensourceinitiative&logoColor=white" alt="OSI Member"/></a>
      <a href="https://github.com/django-commons"><img src="https://img.shields.io/badge/Django_Commons-0C4B33?style=flat-square&logo=django&logoColor=white" alt="Django Commons Member"/></a>
      <a href="https://kernel.org/"><img src="https://img.shields.io/badge/Linux_Kernel-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux Kernel"/></a>
      <a href="https://crates.io/users/louzt"><img src="https://img.shields.io/badge/crates.io-000000?style=flat-square&logo=rust&logoColor=e43717" alt="crates.io packages"/></a>
      <img src="https://img.shields.io/badge/%2b_muitas_outras-1E293B?style=flat-square" alt="+ many more communities"/>
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
      <img src="https://img.shields.io/badge/Sempre_curioso_para_depurar_em_outra_stack-8b5cf6?style=flat-square&logoColor=white" alt="Always curious to debug in another tech stack"/>
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
      <img src="https://img.shields.io/badge/Pagamentos_Cripto_(BTC%2fSOL)-121D33?style=flat-square&logo=solana&logoColor=white" alt="Crypto Payments"/>
      <img src="https://img.shields.io/badge/APIs_Personalizadas_REST_%26_GraphQL-00A1E0?style=flat-square" alt="Custom REST & GraphQL APIs"/>
      <img src="https://img.shields.io/badge/Rastreamento_Server--Side-00A1E0?style=flat-square&logo=salesforce&logoColor=white" alt="Server-Side Tracking"/>
      <img src="https://img.shields.io/badge/CRM-00A1E0?style=flat-square&logo=salesforce&logoColor=white" alt="CRM"/>
      <img src="https://img.shields.io/badge/ERP-714B67?style=flat-square" alt="ERP"/>
      <img src="https://img.shields.io/badge/SaaS--to--SaaS-2C3E50?style=flat-square" alt="SaaS-to-SaaS"/>
    </td>
  </tr>
    <!-- Row 5: Web3 & Decentralized Infrastructure -->
    <td align="left" valign="middle">
    <td align="left" valign="middle">
      <img src="https://img.shields.io/badge/Blockchain_%26_Web3-121D33?style=flat-square&logo=blockchaindotcom&logoColor=white" alt="Blockchain & Web3"/>
      <img src="https://img.shields.io/badge/Protocolos_MCP_%26_Agentes-000000?style=flat-square&logo=github&logoColor=white" alt="MCP & Agent Protocols"/>
      <img src="https://img.shields.io/badge/Fluxos_de_Agentes-7c3aed?style=flat-square" alt="Agentic Workflows"/>
      <img src="https://img.shields.io/badge/Isolamento_RBAC_%26_Multi--Tenant-0f172a?style=flat-square" alt="RBAC & Multi-Tenant Isolation"/>
      <img src="https://img.shields.io/badge/Identidade_Ed25519-2C3E50?style=flat-square" alt="Ed25519 Identity"/>
      <img src="https://img.shields.io/badge/Triplas_Virtuoso_%2f_SPARQL-2C3E50?style=flat-square" alt="Virtuoso Triples / SPARQL"/>
      <img src="https://img.shields.io/badge/Grafos_de_Conhecimento-0f172a?style=flat-square" alt="Knowledge Graphs"/>
      <img src="https://img.shields.io/badge/Local--First_%26_CRDT-064E3B?style=flat-square" alt="Local-First & CRDT"/>
    </td>
  </tr>
    <!-- Row 6: Research Specializations, Engineering Categories & Community Call -->
    <td align="left" valign="middle">
    <td align="left" valign="middle">
      <a href="https://gist.github.com/louzt/376f48c722d4a15d7e78f940818cbade"><img src="https://img.shields.io/badge/Harneses_Determin%C3%ADsticos-8b5cf6?style=flat-square" alt="Deterministic Harnesses"/></a>
      <a href="https://gist.github.com/louzt/d1ce71c05460c2c32bf31342cd0c6a3f"><img src="https://img.shields.io/badge/Sovereign_RAG-7c3aed?style=flat-square" alt="Sovereign RAG"/></a>
      <img src="https://img.shields.io/badge/Engenharia_Baseada_em_Especifica%C3%A7%C3%B5es-0284c7?style=flat-square" alt="Spec-Driven Engineering"/>
      <img src="https://img.shields.io/badge/Seguran%C3%A7a_Zero--Egress-1F2937?style=flat-square" alt="Zero-Egress Security"/>
      <img src="https://img.shields.io/badge/Endurecimento_de_Kernel_%26_Runtime-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Kernel & Runtime Hardening"/>
      <img src="https://img.shields.io/badge/Governan%C3%A7a_CLA_%26_FOSS-004D40?style=flat-square" alt="CLA & FOSS Governance"/>
      <a href="mailto:partnership@loust.pro"><img src="https://img.shields.io/badge/partnership%40loust.pro-0A66C2?style=flat-square&logo=minutemailer&logoColor=white" alt="partnership@loust.pro"/></a>
      <a href="mailto:partnership@loust.pro?subject=FOSS%20Community%20Collaboration"><img src="https://img.shields.io/badge/Open_to_contribute_to_FOSS%2FOSS_Communities-34A853?style=flat-square&logo=opensourceinitiative&logoColor=white" alt="Open to contribute to FOSS/OSS Communities"/></a>
      <a href="mailto:partnership@loust.pro?subject=Peer%20Collaboration"><img src="https://img.shields.io/badge/Procurando_colegas_%26_projetos_empolgantes-0284c7?style=flat-square" alt="Looking for peers & exciting projects"/></a>
    </td>
  </tr>
    <!-- Row 7: Roles, Infrastructure & Mindset -->
    <td align="left" valign="middle">
    <td align="left" valign="middle">
      <img src="https://img.shields.io/badge/Arquiteto_de_Sistemas-0f172a?style=flat-square" alt="Systems Architect"/>
      <img src="https://img.shields.io/badge/DevOps_%26_SRE-2563eb?style=flat-square&logo=kubernetes&logoColor=white" alt="DevOps & SRE"/>
      <img src="https://img.shields.io/badge/Engenharia_de_Plataformas-0891b2?style=flat-square" alt="Platform Engineering"/>
      <img src="https://img.shields.io/badge/Pesquisador_de_Seguran%C3%A7a-eb0029?style=flat-square&logo=hackerone&logoColor=white" alt="Security Researcher"/>
      <img src="https://img.shields.io/badge/Engenharia_de_Primeiros_Princ%C3%ADpios-6366f1?style=flat-square" alt="First-Principles Engineering"/>
      <img src="https://img.shields.io/badge/Infraestrutura_Zero--Trust-1e293b?style=flat-square" alt="Zero-Trust Infrastructure"/>
      <img src="https://img.shields.io/badge/Pesquisa_de_Kernel_%26_Sistemas-0f172a?style=flat-square&logo=linux&logoColor=white" alt="Kernel & Systems Research"/>
      <img src="https://img.shields.io/badge/Estudante_para_Toda_a_Vida-7c3aed?style=flat-square" alt="Lifelong Student"/>
    </td>
  </tr>

<div align="center">
<div align="center">
  <img alt="Systems Architecture &amp; Operational Posture — section banner" src="https://raw.githubusercontent.com/louzt/louzt/main/static/section-tactical-posture.svg" width="100%" />

Mantenho uma postura de engenharia profilática, respeitosa e determinística — calibrando continuamente o raciocínio, as camadas de transporte e os fluxos operacionais contra evidência empírica. Eu projeto e entrego sistemas em produção onde a fronteira entre entrega de aplicação e engenharia de sistemas precisa se sustentar. A maior parte do meu trabalho é engenharia com viés de pesquisa: as abstrações são reutilizáveis, as provas são formais onde precisam ser, e a evidência operacional é auditável de ponta a ponta.

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

- Abordo a engenharia de sistemas como um artesão em uma oficina — estudando a arquitetura do produto, os gargalos de transporte e a telemetria de ponta a ponta antes de tocar em código ou propor refatorações.
- Mantenho uma paciência devota e metódica para extrair telemetria determinística até o último ponto de dados — construindo harnesses de teste sob medida, watchdog reapers e suites de verificação sempre que o ferramental existente deixa margem para ambiguidade.
- Digiro e compilo artefatos brutos do upstream — issues, PRs, árvores históricas de commits e especificações de API de fornecedores — em grafos de conhecimento hiper-eficientes para orçamento de tokens com zero overhead, compactação de contexto e análise diferencial multi-branch.
- Projeto sistemas auto-curativos e auto-melhoráveis construídos em torno de avaliação explícita de custo de oportunidade — reconhecendo cedo que a visão humana tem pontos cegos, então o próprio sistema deve se auto-calibrar, podar specs obsoletos e aplicar invariantes.
- Executo triagem de SAST e síntese de OSINT sob medida para o problema, sobre vulnerabilidades e artigos técnicos publicamente documentados, sintetizando achados empíricos em suites de teste reproduzíveis antes de validar hipóteses contra implementações candidatas.
- Equilibro ciclos rápidos de inovação com alavancagem de longo prazo — estruturando avanços técnicos em marcos trimestrais de roadmap, bibliotecas de padrões reutilizáveis e decisões arquiteturais duráveis que sobrevivem à rotatividade de mantenedores.
- Respeito e adoto a visão do mantenedor ao contribuir em codebases externos — enquadrando propostas por dimensões arquiteturais claras (ortogonal, horizontal ou vertical) e entregando patches de escopo mínimo que minimizam a fricção de revisão.
- Tenho atuado na interseção entre engenharia de sistemas e agentes de IA muito antes da existência de IDEs comerciais de IA — construindo loops de agentes CLI-first em terminal, pontes MCP customizadas e publicando **Investigaciones** reproduzíveis (detalhadas na seção de pesquisa abaixo).
- Endureço primeiro as camadas de rede, IPC e serviço, garantindo que o substrato subjacente esteja seguro e resiliente antes de pedir ao código de aplicação que carregue cargas de produção.
- Rastreio edge cases diretamente até o comportamento em runtime até que o contrato subjacente fique explícito, consertando fronteiras estruturais em vez de aplicar patches superficiais.
- Rodo triagem, SAST e benchmarks direcionados em C, Rust, Go, Bun, Zig e Python em setups de laboratório, avaliando trade-offs do mundo real em memória, latência e estado para construir uma biblioteca prática de padrões.
- Integro novas capacidades por meio de adaptadores limpos e isolados que respeitam a lógica de produção em funcionamento, permitindo que plataformas estabelecidas escalem com segurança sem quebrar fluxos de negócio centrais.
- Endereço ineficiências de escala de IA na raiz — otimizando substratos locais de RAG, loops de execução e compactação de contexto desde o bare-metal para cima antes de pagar por overhead bruto de modelo.
- Mantenho uma postura autossuficiente e transparente: infraestrutura sensível redigida, pull requests com escopo enxuto e revisões de código tratadas como diálogo técnico construtivo e bilateral.

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/section-working-with-me.svg" width="100%" alt="Working with me — section banner"/></p>

### Trabalhando comigo

- **Feedback e aprendizado** — se você me encontrar em algum lugar aprendendo a trabalhar melhor dentro de um time de software, eu me interesso. Revisores sêniores, leads de engenharia ou colegas de time que tenham uma observação técnica específica — uma thread de code review, uma codebase compartilhada, uma fricção de processo — podem entrar em contato. Considero sua opinião útil e trato feedback como um loop bilateral, não uma entrega unilateral; a melhor postura de aprendizado é manter o rastro de auditoria legível dos dois lados.
- **Trilha de divulgação HackerOne** — relatórios de vulnerabilidade e divulgação coordenada para infraestrutura dentro do nosso escopo passam por [security@loust.pro](mailto:security@loust.pro). Triagem em até 72 horas; PoCs reproduzíveis e uma sugestão de patch de escopo mínimo movem os relatórios para o topo da fila. Sinais fora de escopo (DMS, hardening de PipeWire) e janelas conhecidas de triagem ocupada são documentadas para que os reporters não fiquem girando em falso.
- **Colaborações de pesquisa** — provas formais, sistemas determinísticos, hardening de camada de transporte, infra soberana de IA. Melhor encaixe: labs universitários, pesquisadores independentes em trilha de doutorado e equipes privadas de P&D trabalhando em probabilidade aplicada / IR / frameworks de agentes. Entre em contato pelo [research@loust.pro](mailto:research@loust.pro) com um resumo de 1 parágrafo e um artefato concreto (gist, draft de paper, benchmark).
- **Hardening de upstream OSS** — se você mantém um projeto OSS onde o modelo de runtime é bem delimitado (contratos de ciclo de vida, hot paths de alocador, fronteiras de compositor ou daemon), eu gostaria de conversar. Aceito PRs com escopo definido contra a fronteira de runtime; traga um reprodutor + um patch de escopo mínimo, não uma apresentação. Convite aberto — trilha de contribuidor de longa data ou co-mantenedor.
- **Comunidades e chat** — IRC, Discord, Matrix e comunidades adjacentes baseadas em chat são meus canais preferidos, acima das redes sociais convencionais. Se você atua em comunidades OSS nessas superfícies (Libera.Chat / OFTC, salas Matrix, servidores OSS no Discord, canais específicos de projeto), fique à vontade para me chamar. Eu leio mais do que escrevo, mas valorizo sinal acima de volume.
- **Trabalho de plataforma B2B / parcerias** — apenas engajamentos de horizonte longo. Construímos o substrato, a observabilidade e o rastro de auditoria antes de declarar qualquer coisa como entregue — a capacidade para rollouts em estágios é a restrição, não o calendário. Entre em contato pelo [partnership@loust.pro](mailto:partnership@loust.pro).
- **Política de referências** — eu escrevo referências públicas para trabalho entregue com resultados mensuráveis. Envie o link do PR / artefato e uma métrica de resultado em 1 linha; eu respondo em até uma semana.

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

Sistemas em produção que foram entregues para usuários reais, mergeados em upstreams ou rodam como plataformas de longa duração para clientes. Artefatos públicos linkam para fora; plataformas privadas são referenciadas apenas pelo nome — a fronteira entre prova pública e trabalho confidencial de cliente é deliberada, revisável e inalterada entre engajamentos.

**Como nos mantemos atualizados.** Release notes são lidas antes de instalações. Changelogs de specs (MCP, Claude, OpenAI, Gemini, cada API de modelo da qual dependemos) são acompanhados continuamente. A triagem vai várias camadas fundo antes que qualquer coisa seja entregue — o objetivo é entender a *visão*, o *escopo* e os *próximos passos* de tudo do que dependemos, para que o operador herde um sistema sólido em vez de um castelo de cartas.

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
Ao entregar uma flag de override, comece com uma variável de ambiente (<code>DMS_PLUGIN_REGISTRIES</code>) em vez de um arquivo de configuração. Atrito zero para scripting, deploys containerizados e CI. Migre para um arquivo de configuração somente quando o estado precisar persistir ou uma UI precisar editá-lo.
</p>
</p>
⚠️ <b>Tradeoff:</b> nenhuma camada de validação até que a persistência chegue.<br>
🚫 <b>Quando NÃO aplicar:</b> configuração stateful com múltiplos campos correlacionados.
</p>
</p>
</div>
</td>
<td valign="top" width="50%">
<div style="background: #0f172a; border-left: 4px solid #f472b6; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
<h4 style="margin: 8px 0 6px 0; color: #f8fafc;">🪜 Third-caller applies</h4>
Código duplicado é OK entre 2 pacotes. Extraia uma abstração compartilhada somente quando ≥3 chamadores precisarem da mesma forma (ex. plugins + themes + handlers de servidor + CLI = 4 → hora de extrair <code>core/internal/registries</code>). Força nomenclatura honesta e validação compartilhada, adia a sobre-abstração.
</p>
</p>
⚠️ <b>Tradeoff:</b> um pequeno imposto de duplicação; elimina abstração prematura.
</p>
</p>
</div>
</td>
</tr>
<tr>
<td valign="top" width="50%">
<div style="background: #0f172a; border-left: 4px solid #34d399; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
<h4 style="margin: 8px 0 6px 0; color: #f8fafc;">🔁 Idempotent cache migration by signature</h4>
Ao reestruturar estado em disco, detecte o legado pelo <b>que ele parece</b> (ex. <code>&lt;cache&gt;/.git</code> presente, ou diretório plano <code>&lt;cache&gt;/plugins/</code>) — não por número de versão. A migração precisa ser um no-op quando o novo layout já existe, para que re-execuções sejam seguras e processos concorrentes não corrompam o estado.
</p>
</p>
⚠️ <b>Tradeoff:</b> a detecção heurística exige tratamento defensivo com <code>os.IsNotExist</code>.
</p>
</p>
</div>
</td>
<td valign="top" width="50%">
<div style="background: #0f172a; border-left: 4px solid #facc15; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
<h4 style="margin: 8px 0 6px 0; color: #f8fafc;">⚖️ Declaration order = priority</h4>
Ao compor múltiplas fontes, "primeiro acerto vence" via iteração ordenada. Evite adicionar campos <code>priority: int</code> ou <code>disabled: bool</code> — a ordem da lista <i>é</i> o contrato de prioridade. Usuários avançados conseguem empilhar registries naturalmente: <code>official → personal → experimental</code>.
</p>
</p>
⚠️ <b>Tradeoff:</b> não há como "pular" um registry sem removê-lo da lista.
</p>
</p>
</div>
</td>
</tr>
<tr>
<td valign="top" width="50%">
<div style="background: #0f172a; border-left: 4px solid #a78bfa; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
<h4 style="margin: 8px 0 6px 0; color: #f8fafc;">🧩 Errors.Join for partial-failure aggregation</h4>
Ao agregar de N fontes, retorne <code>errors.Join(errs...)</code> em vez de abortar no primeiro erro. Um registry quebrado não deve bloquear os outros. Expor estado parcial é mais honesto do que falha silenciosa e mais útil do que aborto total. Traçado diretamente a partir do rewrite do mantenedor em <a href="https://github.com/AvengeMedia/DankMaterialShell/pull/2972">DMS #2972</a> depois que minha primeira iteração abortou no primeiro erro.
</p>
</p>
⚠️ <b>Tradeoff:</b> chamadores precisam inspecionar o erro joined para saber quais fontes falharam.
</p>
</p>
</div>
</td>
<td valign="top" width="50%">
<div style="background: #0f172a; border-left: 4px solid #fb7185; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
<h4 style="margin: 8px 0 6px 0; color: #f8fafc;">🛡️ Reserved name + validation regex</h4>
Qualquer feature "default + lista customizada" (registries, themes, profiles, frotas de agentes) precisa de um nome reservado para o default oficial (<code>"official"</code>) mais uma regex estrita de validação (<code>^[a-z0-9][a-z0-9-]{0,31}$</code>). Previne spoofing, path traversal e defaults silenciosamente sombreados quando um arquivo de configuração sobrescreve os defaults de env.
</p>
</p>
⚠️ <b>Tradeoff:</b> mais custo upfront de validação; elimina uma classe inteira de bugs do tipo "por que meu default sumiu".
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
          ⚡ <a href="https://github.com/LOUST-PRO/NetBoozt_InternetUpgrade/releases" style="color: #38bdf8; text-decoration: none;"><b>NetBoozt — Performance de Rede, Fallback de DNS &amp; Tuning de Socket</b></a>
        </h4>
        </h4>
          Engine multiplataforma de upgrade de performance de rede &amp; tuning de socket construída com Rust, Tauri e netcode C nativo. Conta com um <b>módulo de Fallback DNS experimental para Windows &amp; Linux</b> projetado para contornar servidores DNS instáveis de ISP e travas de resolução em modem de operadora, além de autotuning de janela TCP, seleção de congestionamento BBR/Cubic, <code>TCP_NODELAY</code>, priorização QoS DSCP e descoberta de MTU/MSS.
        </p>
        </p>
          ⚡ <b>Destaques:</b> ganho de throughput de +15–20% · módulo de Fallback DNS para ISP/Modem · releases Windows &amp; Linux · tuning BBR/Cubic.
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
          🔐 <a href="https://github.com/LOUST-PRO/SnapPipe" style="color: #38bdf8; text-decoration: none;"><b>SnapPipe — Transporte de Identidade &amp; Criptografia</b></a>
        </h4>
        </h4>
          Protocolo de transporte de identidade e troca de chaves de alta performance escrito em Rust. Aplica handshakes criptográficos zero-trust, isolamento de sessão peer-to-peer e sincronização de estado zero-egress entre nós de borda não gerenciados.
        </p>
        </p>
          ⚡ <b>Destaques:</b> handshakes criptográficos zero-trust · isolamento de sessão P2P · núcleo em Rust puro.
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
          🏷️ <a href="https://github.com/LOUST-PRO/TaxonRouter" style="color: #38bdf8; text-decoration: none;"><b>TaxonRouter — Microsserviço de Auto-Tagging de Webhooks</b></a>
        </h4>
        </h4>
          Microsserviço concorrente em Go para categorização de payloads em tempo real, roteamento por regex e tagging automatizado de webhooks em pipelines B2B event-driven de alto throughput, com zero alocações de memória.
        </p>
        </p>
          ⚡ <b>Destaques:</b> parser em Go zero-alloc · categorização de payload em tempo real · alta concorrência.
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
          🧹 <a href="https://github.com/LOUST-PRO/LLMmempipe" style="color: #38bdf8; text-decoration: none;"><b>LLMmempipe — Limpador de Exports de LLM &amp; Markdown Token-Eficiente</b></a>
        </h4>
        </h4>
          Compila exports ruidosos de LLM (ChatGPT, Claude, Gemini) em JSONL e Markdown token-eficientes sob medida para Claude Code, Claude Projects e runtimes de agentes downstream. Schema determinístico, re-ingestão idempotente e rebuilds reproduzíveis em corpora multi-provider.
        </p>
        </p>
          ⚡ <b>Destaques:</b> JSONL/Markdown token-eficiente · normalização multi-provider · re-ingestão idempotente para pipelines de agentes.
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
          🖼️ <a href="https://github.com/LOUST-PRO/paperforge" style="color: #38bdf8; text-decoration: none;"><b>paperforge — Frontend Linux para Wallpaper Engine</b></a>
        </h4>
        </h4>
          Frontend em Rust sob licença MIT para o <b>Workshop do linux-wallpaperengine</b>. Encapsula assets da Steam Workshop em uma superfície de renderização Linux nativa com reprodução determinística de shaders, cache offline de cenas e integração com compositor via Vulkan. Aplicação desktop standalone — não é um pipeline de RAG.
        </p>
        </p>
          ⚡ <b>Destaques:</b> ingestão de assets da Steam Workshop · UI nativa em Rust GTK4 · reprodução determinística de shaders &amp; cache offline.
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
          🤝 <a href="https://github.com/LOUST-PRO/LZT-Developers" style="color: #38bdf8; text-decoration: none;"><b>LZT-Developers — Diretório YAML de Devs</b></a>
        </h4>
        </h4>
          Diretório declarativo de desenvolvedores em <a href="https://devs-github.loust.pro">devs-github.loust.pro</a>. Contribuintes adicionam um único arquivo YAML em <code>/members</code> e abrem um PR — ingestão zero-conflito para o roster público da comunidade. Revisado na hora de buscar talento para iniciativas open source, CRM interno e contratos B2B.
        </p>
        </p>
          ⚡ <b>Destaques:</b> diretório YAML <code>/members</code> · onboarding zero-conflito · superfície pública devs-github.loust.pro.
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
          📅 <a href="https://github.com/LOUST-PRO/ical-to-caldav" style="color: #38bdf8; text-decoration: none;"><b>ical-to-caldav — Daemon Ponte de iCal → CalDAV</b></a>
        </h4>
        </h4>
          Daemon leve sob Apache-2.0 que converte URLs públicas de assinatura de iCal (<code>.ics</code>) em um servidor CalDAV totalmente funcional. Conecta-se em <code>khal</code>, DankCalendar, Evolution, Thunderbird, GNOME Calendar e qualquer cliente CalDAV compatível com o padrão — sem vendor lock-in, sem round-trips para SaaS.
        </p>
        </p>
          ⚡ <b>Destaques:</b> Go stdlib puro · Apache-2.0 · ponte CalDAV plug-and-play para qualquer URL <code>.ics</code>.
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
          📚 <a href="https://github.com/LOUST-PRO/spec-snapshot-scraper" style="color: #38bdf8; text-decoration: none;"><b>spec-snapshot-scraper — Corpora de Docs AI-Ready</b></a>
        </h4>
        </h4>
          Ferramenta de snapshot para criar corpora de documentação AI-ready. Suporta web crawling, árvores GitHub e listas de URL com versionamento determinístico, change tracking e cabeçalhos de metadados em YAML. Projetada como substrato upstream para pipelines de ingestão Sovereign RAG e mirrors offline de specs.
        </p>
        </p>
          ⚡ <b>Destaques:</b> ingestão Web/GitHub/URL · cabeçalhos de metadados em YAML · snapshots versionados para RAG offline.
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
          🔎 <a href="https://github.com/louzt/serpapi-mcp" style="color: #38bdf8; text-decoration: none;"><b>serpapi-mcp — Servidor MCP de Busca Multi-Engine</b></a>
        </h4>
        </h4>
          Servidor MCP stdio em Go expondo <b>busca multi-engine da SerpApi</b> (Google + 20+ engines) atrás de um pipeline de autenticação OAuth 2.0 + JWT, instanciação dinâmica de <code>ResourceTemplate</code> por RFC 6570 e conformidade com o protocolo Anthropic Research. Projetei um proxy OIDC, mapeamento criptográfico de estado para validação de discovery, regras determinísticas de garbage collection e constraints de prioridade de memória para otimizar os limites de contexto ativo.
        </p>
        </p>
          ⚡ <b>Destaques:</b> redução de ~97,5% no payload do handshake via expansão lazy de <code>ResourceTemplate</code> · OAuth 2.0 + JWT · protocolo Anthropic Research · fan-out multi-engine.
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

- **Mais de 850 mil linhas de código em produção** entregues em 50+ projetos (2019–2026)
- **Compactação & Triagem de Knowledge Graph**: indexação de corpus SPARQL/TriG digerindo issues históricos, PRs e diffs de commits vs forks locais para orçamento de tokens com zero overhead e análise diferencial multi-branch
- **Scanners Customizados de SAST & OSINT**: regras de análise estática sob medida para o problema e mapeamento de threat intelligence OSINT público documentando regressões contra codebases locais antes da submissão do patch
- **Harnesses de Teste Diferencial Cross-Fork**: suites de simulação multi-branch medindo latência de execução, pegada de memória e invariância de estado entre patches candidatos vs forks upstream
- **9 pacotes e 391 arquivos TypeScript** no monorepo Nexus Engine
- **42 modelos Prisma e mais de 600 endpoints GraphQL** em engines B2B multi-tenant em produção
- **Isolamento RBAC multi-tenant corporativo** & workflows agentic autônomos
- **Framework legal de governança FOSS CLA, DMCA e Acceptable Use (AUP)** da comunidade
- **50 mil embeddings consultados em 188 ms** em pipelines de retrieval RAG orientadas a GPU
- **Ganhos de throughput de 15–20%** nos benchmarks de otimização TCP do NetBoozt em Windows
- **Latência de resposta lead-to-quote de menos de 2 minutos** no pipeline de atribuição de conversão SYPREME
- **Pipeline atômico de faturamento CFDI 4.0** (e-commerce multi-tenant + Stripe / MercadoPago / Crypto)
- **Contagem de canais Redis reduzida de 59 → 18** via migração de KEYS para SCAN/COUNT

</details>


<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/section-what-we-ship.svg" width="100%" alt="What we ship at loust.pro — Software company section banner"/></p>

O provedor de tecnologia por trás do meu trabalho — transporte multi-protocolo, substrato Linux endurecido e plataformas B2B que sobrevivem a horizontes de múltiplos anos. Artefatos públicos aterrissam em **Research & Publications** e **Investigations & Notes**; esta seção é a superfície de produto que eu opero no dia a dia.

<p align="right"><sub><em>LOUST · Leverage Opportunities Unleashing Success and Transformation</em></sub></p>

<table width="100%">
<table width="100%">
  <tr>
    <td valign="top" width="50%">
      <div style="background: #0f172a; border-left: 4px solid #38bdf8; padding: 14px; border-radius: 6px; margin-bottom: 8px;">
        <h4 style="margin: 0 0 6px 0; color: #f8fafc;">
          🏢 <b>Enterprise CMS</b>
        </h4>
        </h4>
          Plataforma multi-tenant de conteúdo, comércio e operações que sustenta marketing dinâmico, workflows ERP-lite, agendamentos e storefronts a partir de uma única codebase com evolução de schema sem downtime.
        </p>
        </p>
          ⚡ <b>Destaques:</b> namespaces isolados Postgres/Redis por tenant · Schema de 135 mil linhas · APQ @ 90,9% hit rate.
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
          ⚡ <b>Automations Engine</b>
        </h4>
        </h4>
          Engine event-driven de regras e webhooks para operações de cliente. Conecta Meta CAPI, Google Ads, Stripe, MercadoPago e faturamento CFDI 4.0 em pipelines auditáveis com capacidade de replay.
        </p>
        </p>
          ⚡ <b>Destaques:</b> tracking zero data-loss · ingestão de webhooks sub-segundo · replay de eventos &amp; logs de auditoria.
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
          Superfícies de pipeline, contato e fechamento desenhadas para times de vendas sob alta pressão. Entrega ingestão de leads em tempo real e isolamento de pipeline multi-tenant.
        </p>
        </p>
          ⚡ <b>Destaques:</b> latência lead-to-quote &lt;2 min sob carga de feira · isolamento multi-tenant nativo.
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
          🌐 <a href="https://socialspheremx.loust.pro" style="color: #38bdf8; text-decoration: none;"><b>SocialSphereMX — SaaS Multi-Tenant, ERP &amp; Tecido MarTech</b></a>
        </h4>
        </h4>
          Tecido SaaS multi-tenant &amp; ecossistema MarTech para agências, criadores de conteúdo, imobiliárias PropTech e empresas de hospitalidade. Conta com Digital MediaKits interativos com streams de metadados de API ao vivo (Spotify/YouTube), ERP nativo em cloud para restaurantes (menus QR, KDS em tempo real, UI de garçom), tracking de inventário imobiliário em tempo real e workflows de leads de baixa latência. Atuo como CTO &amp; Lead SaaS Architect.
        </p>
        </p>
          ⚡ <b>Destaques:</b> core SaaS multi-tenant · ingestão ao vivo Spotify/YouTube · KDS de restaurante &amp; ERP QR · inventário PropTech · 99,9% uptime.
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
          Suíte de geradores spec-driven e sistema de scaffolding de monorepo que mantém consistência estrutural em deploys multi-app a partir de uma única fonte de verdade.
        </p>
        </p>
          ⚡ <b>Destaques:</b> 9 pacotes &amp; 391 arquivos TypeScript · code gen determinístico · tipos compartilhados.
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
          🛒 <b>Marketplace</b>
        </h4>
        </h4>
          Plataforma de e-commerce multi-vendor com faturamento automático de impostos CFDI 4.0, split payouts via Stripe Connect e MercadoPago, e verificação de diretório de vendedores.
        </p>
        </p>
          ⚡ <b>Destaques:</b> pipeline atômico de billing fiscal · splits de payout multi-moeda · ledger auditável.
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
          🤖 <b>AI Chatbot</b>
        </h4>
        </h4>
          Superfície de IA conversacional multi-tenant com loops de raciocínio ReAct, failover dinâmico de providers (MiniMax M3, ChatGPT, Claude, DeepSeek, Gemini, Llama) e exportação para CRM.
        </p>
        </p>
          ⚡ <b>Destaques:</b> orçamentos limitados de retry de tokens · memória Redis isolada por tenant · handoff humano ao vivo.
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
          📚 <b>Notas Públicas de Pesquisa</b>
        </h4>
        </h4>
          Notas de pesquisa longas, drafts de papers e writeups de segurança open-access sobre RAG soberano, hardening de camada de transporte, regressões de kernel e auditorias de infraestrutura.
        </p>
        </p>
          ⚡ <b>Destaques:</b> P&amp;D public-by-default · teoremas formais &amp; PoCs · MDX machine-readable.
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

Notas de pesquisa longas, drafts de papers e cadeias de prova que eu mantenho como parte do trabalho do dia a dia. Cada entrada tem um artefato concreto (gist, draft ou medição) — sem ambições abstratas.

<blockquote style="border-left: 4px solid #8b5cf6; background: #0f172a; padding: 20px; margin: 20px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
<blockquote style="border-left: 4px solid #8b5cf6; background: #0f172a; padding: 20px; margin: 20px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
    🔬 <b>RAG Soberano Determinístico via Projeção por Hash Assinado</b> (draft de paper, 2026)
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
    💡 <b>Executive Summary &amp; Tradução de Impacto Financeiro:</b><br/>
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
    Stack: Rust (DSVH) + Go (APG) + Virtuoso 7.2.6 + FNV-1a 64-bit + normalização L2. Questão em aberto: comparativo empírico frente a frente contra embedders densos (BGE-M3, multilingual) — deixado para trabalho futuro.
  </p>
  </p>

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider.svg" width="100%" alt="divider"/></p>

<blockquote style="border-left: 4px solid #38bdf8; background: #0f172a; padding: 20px; margin: 20px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
<blockquote style="border-left: 4px solid #38bdf8; background: #0f172a; padding: 20px; margin: 20px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
    ⚡ <b>APQ em Escala em um Schema GraphQL de 135 mil Linhas</b> (estudo de caso, 2026)
    <img src="https://img.shields.io/badge/Case_Study-0284C7?style=flat-square&logo=graphql&logoColor=white" align="right" alt="Case Study"/>
    <img src="https://img.shields.io/badge/Case_Study-0284C7?style=flat-square&logo=graphql&logoColor=white" align="right" alt="Case Study"/>
  </h4>
    Prova empírica em produção para APIs GraphQL de alto throughput: <b>90,9% cache hit rate, latência p95 de 12 ms, ganho de +125% de throughput, $0/mês de gasto incremental em infraestrutura</b> no stack LOUST multi-tenant com Next.js 16 + Apollo Server v4 contra um schema GraphQL massivo derivado de Prisma com 135 mil linhas.
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
    💡 <b>Executive Summary &amp; Tradução de Impacto Financeiro:</b><br/>
    <i>Why this matters for your organization:</i> Large enterprise schemas (700+ models, 2,000+ endpoints) typically require forced multi-server database upgrades ($15K–$50K/yr) due to server-side query parsing overhead and massive JSON payloads. By persist-hashing queries at the edge (90.9% hit rate) and applying cgroup v2 build isolation, we achieved a <b>+125% capacity increase at $0/mo incremental cloud spend</b>. For engineering directors and CTOs, this demonstrates elite systems mastery that directly protects company profit margins.
  </p>
  </p>
  <p align="center" style="margin: 12px 0;">
    &nbsp;
    <a href="https://gist.github.com/louzt/0c91771bf6370f0eb47e905934ab47e8"><img src="https://img.shields.io/badge/Leer_el_caso_de_estudio-Espa%C3%B1ol-D97706?style=for-the-badge&logo=github&logoColor=white" alt="Leer el caso de estudio APQ (Español)"/></a>
    <a href="https://gist.github.com/louzt/0c91771bf6370f0eb47e905934ab47e8"><img src="https://img.shields.io/badge/Leer_el_caso_de_estudio-Espa%C3%B1ol-D97706?style=for-the-badge&logo=github&logoColor=white" alt="Leer el caso de estudio APQ (Español)"/></a>
  </p>
    Stack: Next.js 16 <code>cacheComponents</code> + Apollo Server v4 + <code>ApolloAPQCache</code> + Redis 7 <code>ioredis</code> keyPrefix + Lua EVAL atômico + cgroup v2 <code>compile-runner.slice</code> + runner self-hosted do GitHub Actions com volume persistente em <code>/opt/build-cache</code>.
  </p>
  </p>

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider.svg" width="100%" alt="divider"/></p>

<blockquote style="border-left: 4px solid #10b981; background: #0f172a; padding: 20px; margin: 20px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
<blockquote style="border-left: 4px solid #10b981; background: #0f172a; padding: 20px; margin: 20px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
    📡 <b>Protocolo Keep-Alive Zero-Prefill &amp; Drift de Clock Multi-Região</b> (draft de paper do operator stack, 2026)
    <img src="https://img.shields.io/badge/Protocol_Spec-10B981?style=flat-square&logo=go&logoColor=white" align="right" alt="Protocol Spec"/>
    <img src="https://img.shields.io/badge/Protocol_Spec-10B981?style=flat-square&logo=go&logoColor=white" align="right" alt="Protocol Spec"/>
  </h4>
    Um protocolo leve e determinístico de probe keep-alive para clusters GPU upstream e planos de controle de agentes de IA multi-região. Avalia estados de TTL de warm-up de cache usando um único probe com <code>max_tokens=1</code> em uma cadência dinâmica de heartbeat Weibull de 5 minutos, reduzindo custos de re-prefill de VRAM em <b>800× vs cold starts</b> e <b>50× vs ciclos de re-compressão</b> sob rate limits de <code>5.000 req/hora</code>.
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
    💡 <b>Executive Summary &amp; Tradução de Impacto Financeiro:</b><br/>
    <i>Why this matters for your organization:</i> Upstream LLM APIs and GPU clusters suffer from high "cold start" latency and expensive context re-prefilling when idle. By running a 5-minute Weibull heartbeat probe (<code>max_tokens=1</code>), we keep GPU VRAM context hot for <b>800× cheaper than cold starts</b> and <b>50× cheaper than re-compression cycles</b>. For VPs of Engineering and HR leadership, this proves rare operational maturity: zero wasted token burn, sub-second AI response times, and clock-drift-immune multi-region deployments.
    <i>Why this matters for your organization:</i> Upstream LLM APIs and GPU clusters suffer from high "cold start" latency and expensive context re-prefilling when idle. By running a 5-minute Weibull heartbeat probe (<code>max_tokens=1</code>), we keep GPU VRAM context hot for <b>800× cheaper than cold starts</b> and <b>50× cheaper than re-compression cycles</b>. For VPs of Engineering and HR leadership, this proves rare operational maturity: zero wasted token burn, sub-second AI response times, and clock-drift-immune multi-region deployments.
  </p>
    Stack: Go (APG) + Rust (DSVH) + ordenação happens-before de Lamport + intersection bound de Marzullo 1994 + CLOCK_MONOTONIC + limites de sobrevivência Weibull. Documentado em §5, §8, §9 e §12 do paper de operator do Sovereign RAG.
  </p>
  </p>

<blockquote style="border-left: 4px solid #f59e0b; background: #0f172a; padding: 20px; margin: 24px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
<blockquote style="border-left: 4px solid #f59e0b; background: #0f172a; padding: 20px; margin: 24px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
  <h4 style="margin: 0 0 10px 0; color: #f8fafc;">
    💰 <b>Análise Econômica &amp; Modelo de Evasão de Custo de Infraestrutura</b>
  </h4>
  </h4>
    Além da correção teórica, o hardening de substrato é uma <b>alavanca econômica para engenharia de produção</b>. Sob regimes pós-2026 de pricing metered de IA e billing metered de runners de CI/CD, regressões de substrato se compõem diretamente em queima operacional. Nosso stack empírico de hardening entrega evasão de custo mensurável e quantificável em quatro vetores primários:
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
    🧬 <b>HexCortex-H4-LRS — Suíte de Pesquisa em Autômatos Celulares Hexagonais Classe 4</b> (registrada no INDAUTOR, 2026)
    <img src="https://img.shields.io/badge/INDAUTOR-Registered-8B5CF6?style=flat-square&logo=googlescholar&logoColor=white" align="right" alt="INDAUTOR Registered"/>
    <img src="https://img.shields.io/badge/INDAUTOR-Registered-8B5CF6?style=flat-square&logo=googlescholar&logoColor=white" align="right" alt="INDAUTOR Registered"/>
  </h4>
    Suíte local de pesquisa projetada para análise, validação e telemetria de <b>autômatos celulares hexagonais Classe 4</b>, estruturada como artefato formal de software científico para registro de propriedade intelectual (INDAUTOR). Engine em C99 ultra-compacto dominando tracking de Entropia de Shannon, Floyd cycle-finding, histogramas logarítmicos de avalanche e isolamento de memória em runtime — telemetria matemática de alta fidelidade com execução zero-overhead e zero dependências de terceiros. Semente fundacional para o ecossistema de AST de cibersegurança atualmente em desenvolvimento ativo.
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
    Stack: C99 (sem heap, embedded-friendly) + Bun + TypeScript + BM25/TF-IDF + Floyd cycle-finding + Entropia de Shannon + exportação de triples RDF. Registrada no INDAUTOR como o artefato formal de software científico que precede os registros de IP do ecossistema de AST.
  </p>
  </p>

<blockquote style="border-left: 4px solid #e11d48; background: #0f172a; padding: 20px; margin: 20px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
<blockquote style="border-left: 4px solid #e11d48; background: #0f172a; padding: 20px; margin: 20px 0; border-radius: 0 8px 8px 0; color: #e2e8f0;">
    🎮 <b>Epic Games Zen Storage Server — Supressão de I/O &amp; Arquitetura de Stream JSON</b> (<a href="https://github.com/EpicGames/zen-server/pull/711">PR #711</a>, Unreal Engine 5 DDC)
    <img src="https://img.shields.io/badge/Upstream_Contribution-E11D48?style=flat-square&logo=unrealengine&logoColor=white" align="right" alt="Upstream Contribution"/>
    <img src="https://img.shields.io/badge/Upstream_Contribution-E11D48?style=flat-square&logo=unrealengine&logoColor=white" align="right" alt="Upstream Contribution"/>
  </h4>
    Contribuí para o <b>Zen Storage Server da Epic Games</b> — o engine distribuído de objetos em C++20 que sustenta o <b>Derived Data Cache (DDC)</b> do Unreal Engine 5 e os pipelines de cooking de assets. Resolvi um drift estrutural profundo no <code>main</code> upstream (v5.8.18-pre3) para projetar uma camada crítica de isolamento de diagnóstico para ambientes Linux container headless e systemd, eliminando <b>thrashing de page-cache, amplificação de block writes (bloat de metadados CoW) e starvation de workers</b> durante transformações pesadas de assets em filesystems overlay2.
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
    💡 <b>Executive Summary &amp; Tradução de Performance:</b><br/>
    <i>Why this matters for your organization:</i> Heavy Unreal Engine 5 asset cooking pipelines routinely saturate Linux overlay2 storage with Copy-on-Write metadata churn, causing parallel build workers to stall in uninterruptible I/O Wait. By forcing write-zero log files and decoupling sink lifecycles, we eliminated the amplification at the OS level rather than fighting it at the application level. For VPs of Engineering and CTOs, this delivers <b>stable CI throughput under heavy DDC loads, zero worker starvation, and zero behavioral regressions across 139 native unit test vectors</b>.
    <i>Why this matters for your organization:</i> Heavy Unreal Engine 5 asset cooking pipelines routinely saturate Linux overlay2 storage with Copy-on-Write metadata churn, causing parallel build workers to stall in uninterruptible I/O Wait. By forcing write-zero log files and decoupling sink lifecycles, we eliminated the amplification at the OS level rather than fighting it at the application level. For VPs of Engineering and CTOs, this delivers <b>stable CI throughput under heavy DDC loads, zero worker starvation, and zero behavioral regressions across 139 native unit test vectors</b>.
  </p>
    Stack: C++20 + ZenLoggingCmdLineOptions + AsyncSink + xmake + 139 vetores nativos de teste unitário + semântica de I/O overlay2-aware.
  </p>
  </p>

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider.svg" width="100%" alt="divider"/></p>

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/section-investigations-and-notes.svg" width="100%" alt="Investigations and Notes — section banner"/></p>

Notas públicas de pesquisa, forense operacional e séries de patch upstream — indexadas por domínio técnico com provas de código auditáveis e métricas de performance.

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
          🎮 <b>Hardening do Shader Replayer do Valve/Fossilize</b>
        </h4>
        </h4>
          Autorei a verificação de race condition em <code>PR_SET_PDEATHSIG</code> + <code>getppid()</code> (<a href="https://github.com/ValveSoftware/Fossilize/pull/305">PR #305</a>) terminando replayers órfãos de shaders Vulkan imediatamente em crashes do Steam/Proton. Erradiquei 100% de vazamentos de worker de CPU &amp; dreno de bateria em milhões de Steam Deck / dispositivos de jogos Linux no mundo. Autorei <a href="https://github.com/ValveSoftware/Fossilize/pull/311">PR #311</a> com <code>static_assert</code> desbloqueando a suite de auditoria CI do Mesa da Valve com +7.913 LOC (<a href="https://github.com/ValveSoftware/Fossilize/pull/310">PR #310</a>).
        </p>
        </p>
          ⚡ <b>Impacto:</b> ranqueado #7 mundial no <code>ValveSoftware/Fossilize</code> master (2024–2026) ao lado de leads de DXVK e Mesa.
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
          🐧 <b>RFC do NVIDIA DKMS Kernel 7.0+ &amp; Hotplug do Optimus</b>
        </h4>
        </h4>
          Engenhei uma série de patch RFC forward-compat para o refactoring de API do Kernel 7.0: VMA locking (<code>__is_vma_write_locked()</code>), sinais de DMA fence (<code>dma_fence_signal_locked()</code>) e <code>vm_flags_reset()</code> (<a href="https://gist.github.com/louzt/1c85044d5090d19223c3f5edf426a19e">RFC Gist</a>). Adicionei regras modprobe de <code>NVreg_DynamicPowerManagement=0x02</code> resolvendo panics de hotplug USB-C D3cold em laptops híbridos.
        </p>
        </p>
          ⚡ <b>Impacto:</b> panics de kernel e lockups de suspend/resume de GPU erradicados em laptops Optimus híbridos.
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
          🔊 <b>Hardening do PipeWire &amp; Subsistema de Áudio</b>
        </h4>
        </h4>
          Engenhei um timeout nativo de protocolo <code>spa timer</code> de 5s em <code>pw_protocol_native_connect_local_socket()</code> (<a href="https://github.com/louzt/pipewire/commit/2f747a7">commit 2f747a7</a>), eliminando deadlocks permanentes de CLI de áudio (<code>wpctl</code>/<code>pactl</code> travando). Documentei resoluções de overrun de buffer do OpenAL Soft &amp; ALSA em container sob Distrobox/LXC.
        </p>
        </p>
          ⚡ <b>Impacto:</b> 100% de recuperação de sockets de áudio deadlockados em Fedora, Arch, Ubuntu e SteamOS.
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
          🎵 <b>Ecossistema Terminal do spotify-player &amp; rspotify</b>
        </h4>
        </h4>
          Habilitei playback Spotify nativo em terminal headless (TUI) com herança de sessão ativa e zero overhead de GUI. Desambiguei presença do dispositivo Connect em <code>is_active</code> do playback ativo (<code>is_playing</code>) em <code>spotify-player</code> (<a href="https://github.com/aome510/spotify-player/pull/1049">PR #1049</a>), desbloqueando starvation do engine de áudio <code>librespot</code> em speakers em standby. Serializei requests de busca (<a href="https://github.com/aome510/spotify-player/pull/1048">PR #1048</a>) eliminando explosões de quota 429. Propus fallback de drift de schema Serde não-breaking com <code>#[serde(default)]</code> em <code>rspotify</code> (<a href="https://github.com/ramsayleung/rspotify/issues/572">Issue #572</a>).
        </p>
        </p>
          ⚡ <b>Impacto:</b> herança de sessão TUI headless, 100% de eliminação de picos de rate-limit HTTP 429 &amp; deadlocks de playback em speakers em standby.
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
          🖼️ <b>Compositor Wayland &amp; Diagnósticos de IPC de Display</b>
        </h4>
        </h4>
          Autorei diagnósticos de IPC tipados pull-based, rotulagem semântica de assets e isolamento de thread por mutex de output nos pipelines de display Niri Wayland (<a href="https://gist.github.com/louzt/1c5230a2e9471faf9ce4243314361fa1">Gist de 5 PRs</a>). Exposei matriz de filtros de scaling nos backends swww/awww no Waypaper (<a href="https://github.com/louzt/761e227ad8cfe55b29e79cf861214a62">PR #286</a>).
        </p>
        </p>
          ⚡ <b>Impacto:</b> frame pacing zero-drop em displays multi-monitor com taxas de refresh heterogêneas.
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
          🌐 <b>Auditoria de CSP do Chromium 148 &amp; Segurança Web</b>
        </h4>
        </h4>
          Identifiquei regressões de colisão de política CSP Level 3 em sandbox <code>srcdoc</code> cross-origin no Chromium 148 (<a href="https://gist.github.com/louzt/77f0804ca11bad6636f0ac67928bd384">Gist</a>). Aceito upstream sob tracking de disclosure de segurança da Opera GB-80414.
        </p>
        </p>
          ⚡ <b>Impacto:</b> triagem de segurança auditável, isolamento de colisão de sandbox CSP e validação de patch de browser upstream.
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
          🛰️ <b>Proxy de Transporte Resiliente &amp; Telemetria Linux</b>
        </h4>
        </h4>
          Engenhei um proxy de transporte de fallback em 5 níveis correndo QUIC / Hysteria2 / TLS / SSH em &lt;200 ms com topologia pinned por CA (<a href="https://gist.github.com/louzt/3991f144c7d67726045af3cefc60f42a">Gist</a>). Documentei observabilidade zero-overhead de PSI Linux sobre polling e migração de <code>KEYS</code> → <code>SCAN/COUNT</code> no Redis (<a href="https://gist.github.com/louzt/b8349629b602a782ac98d0cbfd0df0c0">Gist</a>).
        </p>
        </p>
          ⚡ <b>Impacto:</b> corrida de transporte sub-200ms através de firewalls restritivos &amp; redução de 70% no bloat de canais do Redis.
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
          🛡️ <b>Hardening de Injeção CRLF em Runtime do NGINX &amp; Validação por Branch-Split</b>
        </h4>
        </h4>
          O NGINX sustenta <b>~30% da web global</b> e é o reverse-proxy / TLS terminator canônico para o stack LOUST multi-tenant. Documentei um vetor de injeção CRLF em runtime via propagação de <code>$uri</code> pelas diretivas <code>proxy_pass</code>, <code>proxy_set_header</code>, <code>add_header</code> e <code>add_trailer</code> — habilitando smuggling arbitrário de headers HTTP através de variáveis upstream malformadas. Autorei um harness de validação por branch-split com medições de ApacheBench, mais testes de regressão em nginx/nginx-tests. Encaminhei patches de hardening como PRs upstream <a href="https://github.com/nginx/nginx/pull/590">nginx#590</a> (sanitização CRLF em runtime), <a href="https://github.com/nginx/nginx/pull/1414">#1414</a> (escape de <code>add_header</code>/<code>add_trailer</code>), <a href="https://github.com/nginx/nginx-tests/pull/55">nginx-tests#55</a> e <a href="https://github.com/nginx/nginx-tests/pull/58">#58</a> (<a href="https://gist.github.com/louzt/7bdf370a28126718e7e7b69d53b0ae86">Gist de Evidência</a>).
        </p>
        </p>
          ⚡ <b>Impacto:</b> endurece <code>ngx_http_proxy_module.c</code> + <code>ngx_http_headers_filter_module.c</code> contra header smuggling · throughput ApacheBench de 4,6k–4,9k req/s sob sanitização.
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
          🤖 <b>Proveniência da Frota Soberana de Agentes &amp; Gates de Claim Git</b>
        </h4>
        </h4>
          Projetei tagging de proveniência determinístico por <code>agent_id</code> e rastros de auditoria de IDs de conversa de subagentes através de workflows agentic hierárquicos. Implementei classificação de autor de working-tree (meu / estrangeiro / misto / desconhecido) com gates automatizados de atribuição de email de autor. Engenhei verificação <code>lzt-branch-claim</code> F80.14-aware, prevenindo drift de branch de agentes paralelos ou condições de corrida durante slicing automatizado de PR e pipelines de geração de código multi-agente (<a href="https://gist.github.com/louzt/3ba453b2876a4b105a9893b26541ffc3">Gist</a>).
        </p>
        </p>
          ⚡ <b>Impacto:</b> verificação de claim de branch git multi-agente zero-drift &amp; 100% de proveniência de execução de agente auditável.
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
          🎮 <b>Engine de Jogo de Luta H4KKEN &amp; Netcode Rollback GGPO</b>
        </h4>
        </h4>
          Projeto de jogo de luta online com <b>netcode rollback estilo GGPO de 30 frames</b> e orquestração de partida P2P/serverless em tempo real. Autorei a camada de transporte WebRTC DataChannel com renderização Babylon.js 8 WebGPU e predição de input sub-frame. Engenhei session binding ancorado em identidade em uma VPS privada em <a href="https://h4kken.loust.pro">h4kken.loust.pro</a>. Artefatos públicos ainda não foram publicados; todas as notas de design e benchmarks vivem atrás do firewall da VPS.
        </p>
        </p>
          ⚡ <b>Impacto:</b> netcode rollback &amp; orquestração de partida P2P do H4KKEN · predição de input sub-frame · session binding ancorado em identidade.
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
          ⛏️ <b>Servidores de Minecraft em Auto-Scaling Standby sobre k3s</b>
        </h4>
        </h4>
          Arquitetei infraestrutura standby serverless &amp; auto-scaling dirigido por RCON para dois <b>servidores de Minecraft</b> em Java (Fabric modded + Paper vanilla) em k3s / Lightweight Kubernetes. Engenhei polling automatizado de estado RCON via CronJob, save/flushes atômicos e tear-downs graciosos de node. Quando zero jogadores estão ativos, os pods de match auto-scaleiam para 0 réplicas (recuperando ~8 GB de RSS RAM), atingindo spin-up rápido de warm-start (&lt;15s) ao receber probes de conexão de novos jogadores (<a href="https://gist.github.com/louzt/b333b5601628a159630da13857834246">Gist em Inglês</a> · <a href="https://gist.github.com/louzt/8e3b86c7398016964699e87d52222cf7">Espanhol</a>).
        </p>
        </p>
          ⚡ <b>Impacto:</b> auto-scaling de Minecraft Fabric+Paper · shutdown idle dirigido por RCON · spin-up de warm-start em &lt;15s · 100% de eliminação de custo idle.
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
    <a href="mailto:pesquisa@loust.pro"><img src="https://img.shields.io/badge/R%26D_Collaboration-research%40loust.pro-8B5CF6?style=for-the-badge&logo=orcid&logoColor=white" alt="R&D Collaboration"/></a>
  </p>

<p align="right"><sub><em>LOUST · Leverage Opportunities Unleashing Success and Transformation</em></sub></p>

> _Gists públicos são linkados individualmente acima conforme saem. Para work-in-progress privado e forense operacional, veja o [LinkedIn](https://www.linkedin.com/in/davidmirelesll/?locale=es_ES) para a visão curada._

<p align="center"><img src="https://raw.githubusercontent.com/louzt/louzt/main/static/divider-bracket-closing.svg" width="100%" alt="closing bracket divider"/></p>

<!-- ============================================================ -->
<!-- ============================================================ -->
<!-- FOOTER: animated squares grid + tagline (no operator name).  -->
<!-- Served from profile-public static/ alongside the section     -->
<!-- banners. Editor-only provenance; GitHub strips the comment.  -->
<div align="center">
<div align="center">
  <img alt="Animated footer tagline" src="https://raw.githubusercontent.com/louzt/louzt/main/static/profile-footer.svg" width="100%" style="display:block;margin:0 auto"/>
