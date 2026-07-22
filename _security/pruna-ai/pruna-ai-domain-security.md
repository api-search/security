---
api_specs:
- filename: pruna-ai-openapi.yml
  format: yaml
  label: Pruna P-API
  slug: pruna-p-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pruna-ai/refs/heads/main/openapi/pruna-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pruna.ai
  spf: true
hosts:
- cert_expires: Oct 17 00:55:21 2026 GMT
  host: www.pruna.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 14:39:25 2026 GMT
  host: docs.api.pruna.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: api.pruna.ai
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Pruna Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pruna AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pruna AI
provider_slug: pruna-ai
slug: pruna-ai-domain-security
source_filename: pruna-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pruna.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 00:55:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.api.pruna.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 14:39:25 2026 GMT\n  hsts: null\n- host: api.pruna.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: pruna.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pruna-ai/refs/heads/main/security/pruna-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Image Generation
- Video Generation
- Generative AI
- Model Optimization
- Inference
- Developer Tools
---
