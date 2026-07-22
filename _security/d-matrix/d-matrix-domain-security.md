---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: d-matrix.ai
  spf: true
hosts:
- cert_expires: Sep 26 17:39:58 2026 GMT
  host: www.d-matrix.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: D Matrix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for d-Matrix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: d-Matrix
provider_slug: d-matrix
slug: d-matrix-domain-security
source_filename: d-matrix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.d-matrix.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 17:39:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: d-matrix.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/d-matrix/refs/heads/main/security/d-matrix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Compute
- AI
- Inference
- Hardware
- Accelerator
- Machine Learning
- Semiconductors
---
