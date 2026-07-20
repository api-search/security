---
api_specs:
- filename: coactive-openapi-original.json
  format: json
  label: Coactive API
  slug: coactive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coactive/refs/heads/main/openapi/coactive-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coactive.ai
  spf: true
hosts:
- cert_expires: Sep 11 05:46:13 2026 GMT
  host: www.coactive.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 03:18:16 2026 GMT
  host: docs.coactive.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: api.coactive.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coactive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coactive, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Coactive
provider_slug: coactive
slug: coactive-domain-security
source_filename: coactive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coactive.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 05:46:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.coactive.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 03:18:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.coactive.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: coactive.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coactive/refs/heads/main/security/coactive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Multimodal AI
- Computer Vision
- Video Intelligence
- Image Search
- Content Intelligence
- Semantic Search
- Contextual Advertising
- Metadata
- Machine Learning
- Media
---
