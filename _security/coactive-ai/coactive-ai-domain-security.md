---
api_specs:
- filename: coactive-ai-openapi-original.json
  format: json
  label: Coactive AI API
  slug: coactive-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coactive-ai/refs/heads/main/openapi/coactive-ai-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coactive.ai
  spf: true
hosts:
- cert_expires: Sep 13 10:26:57 2026 GMT
  host: coactive.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: api.coactive.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: app.coactive.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coactive Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coactive AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Coactive AI
provider_slug: coactive-ai
slug: coactive-ai-domain-security
source_filename: coactive-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coactive.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 10:26:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.coactive.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: null\n- host: app.coactive.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: coactive.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coactive-ai/refs/heads/main/security/coactive-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Multimodal AI
- Computer Vision
- Video Understanding
- Image Search
- Contextual Advertising
- Media
- Content Moderation
- Metadata
---
