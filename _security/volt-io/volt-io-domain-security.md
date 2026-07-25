---
api_specs:
- filename: volt-io-accounts-openapi-original.yaml
  format: yaml
  label: Volt Accounts API
  slug: volt-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volt-io/refs/heads/main/openapi/volt-io-accounts-openapi-original.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: volt.io
  spf: true
hosts:
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: volt.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 09:33:55 2026 GMT
  host: docs.volt.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: gateway.volt.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Volt Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Volt, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: Volt
provider_slug: volt-io
slug: volt-io-domain-security
source_filename: volt-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: volt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: false\n- host: docs.volt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 09:33:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gateway.volt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: volt.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/volt-io/refs/heads/main/security/volt-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- United Kingdom
- Open Banking
- Account-to-Account
- Real-Time Payments
- Payment Initiation
- Payouts
- Recurring Payments
- Cross-Border
- Pay by Bank
---
