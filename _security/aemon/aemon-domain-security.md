---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aemon.ai
  spf: true
hosts:
- cert_expires: Aug 24 01:45:15 2026 GMT
  host: aemon.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aemon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aemon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aemon
provider_slug: aemon
slug: aemon-domain-security
source_filename: aemon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aemon.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 01:45:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aemon.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aemon/refs/heads/main/security/aemon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Research
- Optimization
- Autonomous Agents
- Developer Tools
- Y Combinator
---
