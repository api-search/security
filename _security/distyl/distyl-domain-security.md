---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: distyl.ai
  spf: true
hosts:
- cert_expires: Aug 23 12:18:10 2026 GMT
  host: distyl.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Distyl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Distyl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Distyl
provider_slug: distyl
slug: distyl-domain-security
source_filename: distyl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: distyl.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 12:18:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: distyl.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/distyl/refs/heads/main/security/distyl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Enterprise AI
- Agentic AI
- AI Agents
- Machine Learning
- Healthcare
- Financial Services
- Telecom
---
