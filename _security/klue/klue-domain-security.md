---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: klue.com
  spf: true
hosts:
- cert_expires: Sep 24 23:19:21 2026 GMT
  host: klue.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:19:21 2026 GMT
  host: app.klue.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Klue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Klue, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Klue
provider_slug: klue
slug: klue-domain-security
source_filename: klue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: klue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:19:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.klue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:19:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: klue.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klue/refs/heads/main/security/klue-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SaaS
- Competitive Intelligence
- Competitive Enablement
- Sales Enablement
- Win-Loss Analysis
- Market Intelligence
- Battlecards
- Agents
- MCP
---
