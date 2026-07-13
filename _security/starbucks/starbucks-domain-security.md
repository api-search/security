---
api_specs:
- filename: starbucks-starbucks-api-openapi.yml
  format: yaml
  label: Starbucks API
  slug: starbucks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starbucks/refs/heads/main/openapi/starbucks-starbucks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: starbucks.com
  spf: true
hosts:
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: www.starbucks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: developer.starbucks.com
  hsts: true
  hsts_max_age: 160770400
  https: true
  tls_version: TLSv1.3
- host: api.starbucks.com
  https: false
kind: domain-security
layout: security
method: probed
name: Starbucks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Starbucks, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Starbucks
provider_slug: starbucks
slug: starbucks-domain-security
source_filename: starbucks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.starbucks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.starbucks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 160770400\n- host: api.starbucks.com\n  https: false\ndomains:\n- domain: starbucks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starbucks/refs/heads/main/security/starbucks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Coffee
- Food Service
- Loyalty
- Ordering
- Retail
- Fortune 500
---
