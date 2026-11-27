---
api_specs:
- filename: safetydatasheetapi-account-api-openapi.yml
  format: yaml
  label: SafetyDataSheetAPI Account API
  slug: safetydatasheetapi-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/safetydatasheetapi/openapi/safetydatasheetapi-account-api-openapi.yml
- filename: safetydatasheetapi-bulk-api-openapi.yml
  format: yaml
  label: SafetyDataSheetAPI Bulk API
  slug: safetydatasheetapi-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/safetydatasheetapi/openapi/safetydatasheetapi-bulk-api-openapi.yml
- filename: safetydatasheetapi-extraction-api-openapi.yml
  format: yaml
  label: SafetyDataSheetAPI Extraction API
  slug: safetydatasheetapi-extraction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/safetydatasheetapi/openapi/safetydatasheetapi-extraction-api-openapi.yml
- filename: safetydatasheetapi-website-api-openapi.yml
  format: yaml
  label: SafetyDataSheetAPI Website API
  slug: safetydatasheetapi-website-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/safetydatasheetapi/openapi/safetydatasheetapi-website-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: safetydatasheetapi.com
  spf: true
hosts:
- cert_expires: Jan 16 20:42:43 2027 GMT
  host: safetydatasheetapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SafetyDataSheetAPI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SafetyDataSheetAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SafetyDataSheetAPI
provider_slug: safetydatasheetapi
slug: safetydatasheetapi-domain-security
source_filename: safetydatasheetapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: safetydatasheetapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 20:42:43 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: safetydatasheetapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/safetydatasheetapi/security/safetydatasheetapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Safety Data Sheets
- msds
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
