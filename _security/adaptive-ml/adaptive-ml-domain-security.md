---
api_specs:
- filename: adaptive-ml-openapi-original.json
  format: json
  label: Adaptive Engine API
  slug: adaptive-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adaptive-ml/refs/heads/main/openapi/adaptive-ml-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adaptive-ml.com
  spf: true
hosts:
- cert_expires: Sep 10 23:57:49 2026 GMT
  host: adaptive-ml.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adaptive Ml Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adaptive ML, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Adaptive ML
provider_slug: adaptive-ml
slug: adaptive-ml-domain-security
source_filename: adaptive-ml-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adaptive-ml.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:57:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: adaptive-ml.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adaptive-ml/refs/heads/main/security/adaptive-ml-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- LLM
- Fine-Tuning
- Reinforcement Learning
- Model Evaluation
- Inference
- OpenAI-Compatible
- MLOps
---
