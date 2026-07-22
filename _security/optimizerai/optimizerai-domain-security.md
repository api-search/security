---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: optimizerai.xyz
  spf: true
hosts:
- cert_expires: Sep 11 11:38:00 2026 GMT
  host: www.optimizerai.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: docs.optimizerai.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Optimizerai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OptimizerAI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: OptimizerAI
provider_slug: optimizerai
slug: optimizerai-domain-security
source_filename: optimizerai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.optimizerai.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 11:38:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.optimizerai.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: optimizerai.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optimizerai/refs/heads/main/security/optimizerai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Sound Effects
- Audio
- Generative AI
- Text to Audio
- Game Development
- Media and Entertainment
- Machine Learning
- Creator Tools
---
