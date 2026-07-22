---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ezkl.xyz
  spf: true
hosts:
- cert_expires: Sep 12 01:45:37 2026 GMT
  host: ezkl.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ezkl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EZKL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: EZKL
provider_slug: ezkl
slug: ezkl-domain-security
source_filename: ezkl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ezkl.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 01:45:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ezkl.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ezkl/refs/heads/main/security/ezkl-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Zero-Knowledge Proofs
- Machine Learning
- Verifiable AI
- ZKML
- Cryptography
- ONNX
- Blockchain
- Open Source
- SDK
- CLI
---
