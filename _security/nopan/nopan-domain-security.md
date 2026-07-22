---
api_specs:
- filename: nopan-openapi-original.yml
  format: yaml
  label: Nopan API
  slug: nopan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nopan/refs/heads/main/openapi/nopan-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: nopan.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: nopan.io
  spf: false
hosts:
- cert_expires: Aug 31 10:06:25 2026 GMT
  host: nopan.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: api.nopan.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nopan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nopan, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Nopan
provider_slug: nopan
slug: nopan-domain-security
source_filename: nopan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nopan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 10:06:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nopan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: nopan.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n- domain: nopan.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nopan/refs/heads/main/security/nopan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Payments
- Payment Service Provider
- Account to Account
- Wallet Payments
- Open Banking
- PSD2
- Fintech
- Europe
- Tokenization
- Recurring Payments
---
