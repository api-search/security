---
api_specs:
- filename: openapi.json
  format: json
  label: Reducto Document API
  slug: reducto-document-api
  spec_type: OpenAPI
  url: https://api.reductoai.com/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reducto.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: reductoai.com
  spf: true
hosts:
- cert_expires: Sep  6 01:49:49 2026 GMT
  host: reducto.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 11:39:00 2026 GMT
  host: docs.reducto.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.reductoai.com
  https: false
kind: domain-security
layout: security
method: probed
name: Reducto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reducto, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Reducto
provider_slug: reducto
slug: reducto-domain-security
source_filename: reducto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reducto.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 01:49:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.reducto.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 11:39:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.reductoai.com\n  https: false\ndomains:\n- domain: reducto.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: reductoai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/security/reducto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Document Parsing
- PDF
- OCR
- Data Extraction
- AI
- Machine Learning
- Document Intelligence
- Structured Data
---
