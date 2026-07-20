---
api_specs:
- filename: interfaze-openapi-original.json
  format: json
  label: Interfaze Chat Completion API
  slug: interfaze-chat-completion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfaze/refs/heads/main/openapi/interfaze-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: interfaze.ai
  spf: true
hosts:
- cert_expires: Sep  3 20:50:41 2026 GMT
  host: interfaze.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 00:39:56 2026 GMT
  host: api.interfaze.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Interfaze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Interfaze, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Interfaze
provider_slug: interfaze
slug: interfaze-domain-security
source_filename: interfaze-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: interfaze.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 20:50:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.interfaze.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 00:39:56 2026 GMT\n  hsts: null\ndomains:\n- domain: interfaze.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interfaze/refs/heads/main/security/interfaze-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- LLM
- OCR
- Speech to Text
- Structured Output
- Object Detection
- Web Scraping
- Web Search
- Multimodal
- Developer Tools
---
