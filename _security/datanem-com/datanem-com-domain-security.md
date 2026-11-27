---
api_specs:
- filename: datanem-com-extraction-api-openapi.yml
  format: yaml
  label: Datanem Extraction API
  slug: datanem-com-extraction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datanem-com/openapi/datanem-com-extraction-api-openapi.yml
- filename: datanem-com-templates-api-openapi.yml
  format: yaml
  label: Datanem Templates API
  slug: datanem-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datanem-com/openapi/datanem-com-templates-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: datanem.com
  spf: true
hosts:
- cert_expires: Jan 16 11:11:37 2027 GMT
  host: datanem.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Datanem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datanem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Datanem
provider_slug: datanem-com
slug: datanem-com-domain-security
source_filename: datanem-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datanem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 11:11:37 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: datanem.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/datanem-com/security/datanem-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data Extraction
- OCR
- Document Processing
- Spreadsheet Export
- United Kingdom
---
