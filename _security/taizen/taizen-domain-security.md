---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: usetaizen.com
  spf: true
hosts:
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: usetaizen.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: docs.usetaizen.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 09:50:18 2026 GMT
  host: eu.mcp.usetaizen.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Taizen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taizen, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Taizen
provider_slug: taizen
slug: taizen-domain-security
source_filename: taizen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usetaizen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: false\n- host: docs.usetaizen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: false\n- host: eu.mcp.usetaizen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 09:50:18 2026 GMT\n  hsts: null\ndomains:\n- domain: usetaizen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taizen/refs/heads/main/security/taizen-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Win-Loss Analysis
- Competitive Intelligence
- Sales Enablement
- Revenue Intelligence
- Go-To-Market
- AI Agents
- Battlecards
- Sales
- MCP
- Agent Skills
- Conversation Intelligence
- Product Marketing
---
