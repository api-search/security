---
api_specs:
- filename: sarvam-openapi-original.json
  format: json
  label: Sarvam AI API
  slug: sarvam-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam/refs/heads/main/openapi/sarvam-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sarvam.ai
  spf: true
hosts:
- cert_expires: Oct  1 12:46:21 2026 GMT
  host: api.sarvam.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sarvam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sarvam, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sarvam
provider_slug: sarvam
slug: sarvam-domain-security
source_filename: sarvam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.sarvam.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 12:46:21 2026 GMT\n  hsts: null\ndomains:\n- domain: sarvam.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sarvam/refs/heads/main/security/sarvam-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai Ml
- Artificial Intelligence
- Machine Learning
- Speech To Text
- Text To Speech
- Translation
- Large Language Models
- Document Intelligence
- Indian Languages
- Voice
---
