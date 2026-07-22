---
api_specs:
- filename: simplismart-llama-3.3-70b-openapi.yml
  format: yaml
  label: Simplismart LLM Inference API
  slug: simplismart-llm-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplismart/refs/heads/main/openapi/simplismart-llama-3.3-70b-openapi.yml
- filename: simplismart-flux-dev-openapi.yml
  format: yaml
  label: Simplismart Image Generation API
  slug: simplismart-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplismart/refs/heads/main/openapi/simplismart-flux-dev-openapi.yml
- filename: simplismart-whisper-v3-openapi.yml
  format: yaml
  label: Simplismart Audio Transcription API
  slug: simplismart-audio-transcription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplismart/refs/heads/main/openapi/simplismart-whisper-v3-openapi.yml
- filename: simplismart-llm-training-openapi.yml
  format: yaml
  label: Simplismart Training API
  slug: simplismart-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplismart/refs/heads/main/openapi/simplismart-llm-training-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: simplismart.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: simplismart.live
  spf: false
hosts:
- cert_expires: Oct 15 23:20:32 2026 GMT
  host: www.simplismart.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 13:45:39 2026 GMT
  host: api.simplismart.live
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: http.flux.proxy.prod.s9t.link
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simplismart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simplismart, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Simplismart
provider_slug: simplismart
slug: simplismart-domain-security
source_filename: simplismart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.simplismart.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:20:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.simplismart.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 13:45:39 2026 GMT\n  hsts: null\n- host: http.flux.proxy.prod.s9t.link\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: simplismart.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: simplismart.live\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simplismart/refs/heads/main/security/simplismart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Inference
- LLM
- Model Deployment
- Fine-Tuning
- MLOps
- GPU
- Speech to Text
- Image Generation
---
