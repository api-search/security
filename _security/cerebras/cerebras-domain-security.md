---
api_specs:
- filename: cerebras-openapi.yml
  format: yaml
  label: Cerebras Inference API
  slug: cerebras-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerebras/refs/heads/main/openapi/cerebras-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cerebras.ai
  spf: true
hosts:
- cert_expires: Aug 20 16:18:39 2026 GMT
  host: cerebras.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 02:37:48 2026 GMT
  host: inference-docs.cerebras.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 00:26:37 2026 GMT
  host: api.cerebras.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cerebras Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cerebras, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cerebras
provider_slug: cerebras
slug: cerebras-domain-security
source_filename: cerebras-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cerebras.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 16:18:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: inference-docs.cerebras.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 02:37:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cerebras.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 00:26:37 2026 GMT\n  hsts: null\ndomains:\n- domain: cerebras.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerebras/refs/heads/main/security/cerebras-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Inference
- Large Language Models
- Wafer Scale
- Hardware
- Cloud
- OpenAI Compatible
- LLM
- SDK
- Accelerator
- High Performance Computing
---
