---
api_specs:
- filename: wisk-sales-upload-openapi.yml
  format: yaml
  label: WISK Public Sales Upload API
  slug: sales-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisk/refs/heads/main/openapi/wisk-sales-upload-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wisk.ai
  spf: true
hosts:
- cert_expires: Aug 17 13:46:01 2026 GMT
  host: www.wisk.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 19:48:10 2026 GMT
  host: help.wisk.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: api.wisk.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wisk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WISK.ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: WISK.ai
provider_slug: wisk
slug: wisk-domain-security
source_filename: wisk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wisk.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 13:46:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.wisk.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 19:48:10 2026 GMT\n  hsts: false\n- host: api.wisk.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: wisk.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wisk/refs/heads/main/security/wisk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Bar
- Inventory
- Hospitality
- Sales
- POS Integration
---
