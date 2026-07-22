---
api_specs:
- filename: preciser-api-openapi.yml
  format: yaml
  label: Preciser API
  slug: preciser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preciser/refs/heads/main/openapi/preciser-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: preciser.io
  spf: true
hosts:
- cert_expires: Sep 23 08:11:42 2026 GMT
  host: preciser.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: plg-api.preciser.io
  https: false
kind: domain-security
layout: security
method: probed
name: Preciser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Preciser, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Preciser
provider_slug: preciser
slug: preciser-domain-security
source_filename: preciser-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: preciser.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 08:11:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: plg-api.preciser.io\n  https: false\ndomains:\n- domain: preciser.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/preciser/refs/heads/main/security/preciser-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sports
- Sports Analytics
- Computer Vision
- Artificial Intelligence
- Video Analysis
- Statistics
- Basketball
- Baseball
- Data
---
