---
api_specs:
- filename: myocr-app-convert-api-openapi.yml
  format: yaml
  label: MyOCR Convert API
  slug: myocr-app-convert-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myocr-app/openapi/myocr-app-convert-api-openapi.yml
- filename: myocr-app-jobs-api-openapi.yml
  format: yaml
  label: MyOCR Jobs API
  slug: myocr-app-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myocr-app/openapi/myocr-app-jobs-api-openapi.yml
- filename: myocr-app-keys-api-openapi.yml
  format: yaml
  label: MyOCR Keys API
  slug: myocr-app-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myocr-app/openapi/myocr-app-keys-api-openapi.yml
- filename: myocr-app-status-api-openapi.yml
  format: yaml
  label: MyOCR Status API
  slug: myocr-app-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myocr-app/openapi/myocr-app-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: myocr.app
  spf: true
hosts:
- cert_expires: Jan 13 11:41:44 2027 GMT
  host: myocr.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MyOCR Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyOCR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MyOCR
provider_slug: myocr-app
slug: myocr-app-domain-security
source_filename: myocr-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myocr.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 11:41:44 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: myocr.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/myocr-app/security/myocr-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- OCR
- Document Conversion
- Excel Export
- Finance
- Accounting
---
