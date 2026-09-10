---
api_specs:
- filename: modelrush-public.openapi.yaml
  format: yaml
  label: ModelRush API
  slug: modelrush-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Moonveil-AI/modelrush-developer-tools/main/openapi/modelrush-public.openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "awstrust.com"
  - 0 issue "pki.goog"
  - 0 issue "amazontrust.com"
  dmarc: false
  dnssec: false
  domain: modelrush.ai
  spf: true
hosts:
- cert_expires: Nov  6 23:58:00 2026 GMT
  host: modelrush.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:58:00 2026 GMT
  host: api.modelrush.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Modelrush Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ModelRush, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ModelRush
provider_slug: modelrush
slug: modelrush-domain-security
source_filename: modelrush-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modelrush.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:58:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.modelrush.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:58:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: modelrush.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modelrush/refs/heads/main/security/modelrush-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI
- LLM
- Inference
- Multimodal
- Model Hosting
- Speech
- Image Generation
---
