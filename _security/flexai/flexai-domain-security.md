---
api_specs:
- filename: flexai-token-factory-openapi.yml
  format: yaml
  label: FlexAI Token Factory API
  slug: flexai-token-factory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexai/refs/heads/main/openapi/flexai-token-factory-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flex.ai
  spf: true
hosts:
- cert_expires: Sep 27 15:20:07 2026 GMT
  host: www.flex.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 20:15:52 2026 GMT
  host: docs.flex.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 18:58:39 2026 GMT
  host: tokens.flex.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flexai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FlexAI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FlexAI
provider_slug: flexai
slug: flexai-domain-security
source_filename: flexai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flex.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 15:20:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.flex.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 20:15:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: tokens.flex.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 18:58:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flex.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flexai/refs/heads/main/security/flexai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai/Ml
- Artificial Intelligence
- Machine Learning
- Inference
- LLM
- Large Language Models
- OpenAI Compatible
- GPU Compute
- Embeddings
- Fine-Tuning
- Agents
---
