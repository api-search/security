---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agentsmyth.com
  spf: false
hosts:
- cert_expires: Dec  1 10:58:24 2026 GMT
  host: agentsmyth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 13:20:42 2026 GMT
  host: developer.agentsmyth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: api.agentsmyth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Agentsmyth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentSmyth, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: AgentSmyth
provider_slug: agentsmyth
slug: agentsmyth-domain-security
source_filename: agentsmyth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentsmyth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 10:58:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.agentsmyth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 13:20:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.agentsmyth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: agentsmyth.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentsmyth/refs/heads/main/security/agentsmyth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Capital Markets
- Artificial Intelligence
- AI Agents
- Trading
- Investment Research
- Market Intelligence
- MCP
- agent-native
- Fintech
---
