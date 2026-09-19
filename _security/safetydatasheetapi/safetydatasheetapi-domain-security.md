---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: SDS/MSDS Extraction REST API
  slug: sdsmsds-extraction-rest-api
  spec_type: OpenAPI
  url: https://safetydatasheetapi.com/openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: safetydatasheetapi.com
  spf: true
hosts:
- cert_expires: Nov 18 19:36:59 2026 GMT
  host: safetydatasheetapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.safetydatasheetapi.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Safetydatasheetapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Safety Data Sheet (SDS/MSDS) Extraction API, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Safety Data Sheet (SDS/MSDS) Extraction API
provider_slug: safetydatasheetapi
slug: safetydatasheetapi-domain-security
source_filename: safetydatasheetapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: safetydatasheetapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 19:36:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.safetydatasheetapi.com\n  https: false\ndomains:\n- domain: safetydatasheetapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/safetydatasheetapi/refs/heads/main/security/safetydatasheetapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SDS
- msds
- Safety Data Sheets
- ghs-classification
- chemical-compliance
- EHS
- Regulatory Compliance
- Document Extraction
- OCR
- pdf-to-json
- data-normalization
- ERP Integration
- PLM
- Supply Chain
- Chemicals
---
