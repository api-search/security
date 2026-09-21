---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: grithgate.com
  spf: false
hosts:
- cert_expires: Nov 20 02:04:01 2026 GMT
  host: grithgate.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Grithgate Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GRITH, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: GRITH
provider_slug: grithgate-com
slug: grithgate-com-domain-security
source_filename: grithgate-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grithgate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 02:04:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: grithgate.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grithgate-com/refs/heads/main/security/grithgate-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- A2A
- MCP
- Agent Identity
- Agent Memory
- Decentralized Identity
- Sanctuary
- JSON-RPC
- Append-Only Ledger
---
