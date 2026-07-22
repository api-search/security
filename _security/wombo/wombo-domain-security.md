---
api_specs:
- filename: wombo-wai-openapi.yml
  format: yaml
  label: w.ai Inference API
  slug: wai-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wombo/refs/heads/main/openapi/wombo-wai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: w.ai
  spf: false
hosts:
- cert_expires: Aug 23 23:50:08 2026 GMT
  host: w.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 01:11:46 2026 GMT
  host: docs.w.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 13:38:55 2026 GMT
  host: api.w.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wombo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wombo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Wombo
provider_slug: wombo
slug: wombo-domain-security
source_filename: wombo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: w.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 23:50:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.w.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 01:11:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.w.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 13:38:55 2026 GMT\n  hsts: false\ndomains:\n- domain: w.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wombo/refs/heads/main/security/wombo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Inference
- LLM
- Image Generation
- Generative AI
- Decentralized Compute
- GPU
- OpenAI Compatible
---
