---
api_specs:
- filename: shift4-api-openapi.yml
  format: yaml
  label: Shift4 Payments API
  slug: shift4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/main/openapi/shift4-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shift4.com
  spf: true
hosts:
- cert_expires: Sep 23 06:56:58 2026 GMT
  host: www.shift4.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 11:27:24 2026 GMT
  host: dev.shift4.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 01:55:32 2026 GMT
  host: api.shift4.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shift4 Payments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shift4 Payments, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Shift4 Payments
provider_slug: shift4-payments
slug: shift4-payments-domain-security
source_filename: shift4-payments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shift4.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 06:56:58 2026 GMT\n  hsts: null\n- host: dev.shift4.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 11:27:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.shift4.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 01:55:32 2026 GMT\n  hsts: null\ndomains:\n- domain: shift4.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shift4-payments/refs/heads/main/security/shift4-payments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Fintech
- Commerce
- Checkout
---
