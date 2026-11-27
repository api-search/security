---
api_specs:
- filename: convert-online-catalogue-api-openapi.yml
  format: yaml
  label: Convert.Online Catalogue API
  slug: convert-online-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convert-online/openapi/convert-online-catalogue-api-openapi.yml
- filename: convert-online-downloads-api-openapi.yml
  format: yaml
  label: Convert.Online Downloads API
  slug: convert-online-downloads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convert-online/openapi/convert-online-downloads-api-openapi.yml
- filename: convert-online-imports-api-openapi.yml
  format: yaml
  label: Convert.Online Imports API
  slug: convert-online-imports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convert-online/openapi/convert-online-imports-api-openapi.yml
- filename: convert-online-jobs-api-openapi.yml
  format: yaml
  label: Convert.Online Jobs API
  slug: convert-online-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convert-online/openapi/convert-online-jobs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: convert.online
  spf: true
hosts:
- cert_expires: Jan  3 07:47:09 2027 GMT
  host: convert.online
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Convert.Online Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Convert.Online, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Convert.Online
provider_slug: convert-online
slug: convert-online-domain-security
source_filename: convert-online-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: convert.online\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 07:47:09 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: convert.online\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/convert-online/security/convert-online-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- File Conversion
- Document Conversion
- Image Conversion
- Video Conversion
- Audio Conversion
- OCR
- MCP
---
