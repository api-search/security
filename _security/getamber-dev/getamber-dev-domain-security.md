---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getamber.dev
  spf: true
hosts:
- cert_expires: Dec  4 19:29:54 2026 GMT
  host: getamber.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Getamber Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ambr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ambr
provider_slug: getamber-dev
slug: getamber-dev-domain-security
source_filename: getamber-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getamber.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 19:29:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getamber.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getamber-dev/refs/heads/main/security/getamber-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- Agentic Commerce
- Contracts
- Legal
- Ricardian Contracts
- Delegation
- Blockchain
- Base L2
- MCP
- A2A
- x402
- agent-native
---
