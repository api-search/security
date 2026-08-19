---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: roofline.ai
  spf: true
hosts:
- cert_expires: Oct  3 15:31:31 2026 GMT
  host: www.roofline.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Roofline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Roofline, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Roofline
provider_slug: roofline
slug: roofline-domain-security
source_filename: roofline-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.roofline.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 15:31:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: roofline.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roofline/refs/heads/main/security/roofline-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Ai Data
- Edge AI
- AI Compiler
- MLIR
- IREE
- Machine Learning
- Model Deployment
- Embedded
- NPU
- Quantization
- On-Device LLM
- Developer Tools
- Germany
---
