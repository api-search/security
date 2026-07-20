---
api_specs:
- filename: gptzero-openapi-original.json
  format: json
  label: GPTZero API
  slug: gptzero-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gptzero/refs/heads/main/openapi/gptzero-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gptzero.me
  spf: true
hosts:
- cert_expires: Sep  5 13:30:14 2026 GMT
  host: gptzero.me
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 13:30:14 2026 GMT
  host: api.gptzero.me
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gptzero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GPTZero, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GPTZero
provider_slug: gptzero
slug: gptzero-domain-security
source_filename: gptzero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gptzero.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 13:30:14 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.gptzero.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 13:30:14 2026 GMT\n  hsts: null\ndomains:\n- domain: gptzero.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gptzero/refs/heads/main/security/gptzero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- AI Detection
- Content Moderation
- Machine Learning
- Text Analysis
- Natural Language Processing
- Education
---
