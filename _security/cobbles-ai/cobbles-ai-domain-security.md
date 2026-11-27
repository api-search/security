---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cobbles.ai
  spf: true
hosts:
- cert_expires: Dec  2 11:36:04 2026 GMT
  host: cobbles.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cobbles Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cobbles, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cobbles
provider_slug: cobbles-ai
slug: cobbles-ai-domain-security
source_filename: cobbles-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cobbles.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 11:36:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cobbles.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cobbles-ai/security/cobbles-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- Agent Orchestration
- Human-in-the-Loop
- Approvals
- Audit Logs
- Permissions
- MCP
---
