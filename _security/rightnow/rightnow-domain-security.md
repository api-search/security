---
api_specs:
- filename: rightnow-openapi.json
  format: json
  label: RunInfra Inference API
  slug: runinfra-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightnow/refs/heads/main/openapi/rightnow-openapi.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: runinfra.ai
  spf: true
hosts:
- cert_expires: Oct  2 05:32:00 2026 GMT
  host: runinfra.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 05:32:00 2026 GMT
  host: api.runinfra.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rightnow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RightNow AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RightNow AI
provider_slug: rightnow
slug: rightnow-domain-security
source_filename: rightnow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: runinfra.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 05:32:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.runinfra.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 05:32:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: runinfra.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rightnow/refs/heads/main/security/rightnow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- LLM Inference
- GPU
- Model Deployment
- Serverless
- OpenAI Compatible
- Embeddings
- MLOps
---
