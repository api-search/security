---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: datologyai.com
  spf: true
hosts:
- cert_expires: Sep  9 10:47:54 2026 GMT
  host: datologyai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datologyai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DatologyAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: DatologyAI
provider_slug: datologyai
slug: datologyai-domain-security
source_filename: datologyai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datologyai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 10:47:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: datologyai.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datologyai/refs/heads/main/security/datologyai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai Ml
- Data Curation
- Machine Learning
- Training Data
- Foundation Models
- Data Optimization
- Artificial Intelligence
---
