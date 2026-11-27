---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mypenny.ai
  spf: false
hosts:
- cert_expires: Dec 23 00:14:19 2026 GMT
  host: mypenny.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Helper Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Helper Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Helper Labs
provider_slug: mypenny-ai
slug: mypenny-ai-domain-security
source_filename: mypenny-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mypenny.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 00:14:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mypenny.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mypenny-ai/security/mypenny-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Memory
- Data Portability
- Encryption
- MCP
- Cross‑AI Integration
- User Identity
---
