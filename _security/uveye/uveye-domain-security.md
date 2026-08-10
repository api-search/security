---
api_specs:
- filename: uveye-appraisal-api-openapi.yml
  format: yaml
  label: UVeye Appraisal API
  slug: uveye-appraisal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uveye/refs/heads/main/openapi/uveye-appraisal-api-openapi.yml
- filename: uveye-inspections-api-openapi.yml
  format: yaml
  label: UVeye Inspections API
  slug: uveye-inspections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uveye/refs/heads/main/openapi/uveye-inspections-api-openapi.yml
- filename: uveye-media-api-openapi.yml
  format: yaml
  label: UVeye Media API
  slug: uveye-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uveye/refs/heads/main/openapi/uveye-media-api-openapi.yml
- filename: uveye-merchandise-api-openapi.yml
  format: yaml
  label: UVeye Merchandise API
  slug: uveye-merchandise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uveye/refs/heads/main/openapi/uveye-merchandise-api-openapi.yml
- filename: uveye-public-links-api-openapi.yml
  format: yaml
  label: UVeye Public Links API
  slug: uveye-public-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uveye/refs/heads/main/openapi/uveye-public-links-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uveye.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: uveye.dev
  spf: true
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: uveye.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 21:20:21 2026 GMT
  host: api.v1.uveye.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 02:53:30 2026 GMT
  host: api.uveye.dev
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uveye Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UVeye, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: UVeye
provider_slug: uveye
slug: uveye-domain-security
source_filename: uveye-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uveye.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: false\n- host: api.v1.uveye.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 21:20:21 2026 GMT\n  hsts: null\n- host: api.uveye.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 02:53:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: uveye.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: uveye.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uveye/refs/heads/main/security/uveye-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Vehicle Inspection
- Artificial Intelligence
- Computer Vision
- Dealerships
- Fleet Management
- Auctions and Remarketing
- Automotive Retail
- Inspection Data
- Company
---
