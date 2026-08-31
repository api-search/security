---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agentsea.dev
  spf: true
hosts:
- cert_expires: Sep 22 04:28:34 2026 GMT
  host: agentsea.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 04:28:35 2026 GMT
  host: www.agentsea.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agentsea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentSea, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AgentSea
provider_slug: agentsea
slug: agentsea-domain-security
source_filename: agentsea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentsea.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 04:28:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.agentsea.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 04:28:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agentsea.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentsea/refs/heads/main/security/agentsea-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agent Orchestration
- Large Language Models
- MCP
- Agentic Commerce
- Open-Source
- Developer Tools
- SDK
- TypeScript
- Elixir
- Voice
---
