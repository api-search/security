---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mangoboost.io
  spf: true
hosts:
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: www.mangoboost.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: llmboost.mangoboost.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: sdk.mangoboost.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mangoboost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MangoBoost, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MangoBoost
provider_slug: mangoboost
slug: mangoboost-domain-security
source_filename: mangoboost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mangoboost.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: false\n- host: llmboost.mangoboost.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: false\n- host: sdk.mangoboost.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: mangoboost.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mangoboost/refs/heads/main/security/mangoboost-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- Machine-Learning
- Infrastructure
- Data-Center
- Semiconductors
- Hardware
- Storage
- Networking
- Inference
- GPU
- DPU
---
