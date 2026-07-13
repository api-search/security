---
api_specs:
- filename: stonex-payments-openapi.yml
  format: yaml
  label: StoneX Payments API
  slug: stonex-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stonex/refs/heads/main/openapi/stonex-payments-openapi.yml
- filename: stonex-clearing-openapi.yml
  format: yaml
  label: StoneX Clearing API
  slug: stonex-clearing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stonex/refs/heads/main/openapi/stonex-clearing-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stonex.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stonex.io
  spf: false
hosts:
- cert_expires: Aug 16 23:11:03 2026 GMT
  host: www.stonex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 11:47:18 2026 GMT
  host: docs.payments.stonex.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 23:59:59 2026 GMT
  host: docs.clearing.stonex.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stonex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StoneX, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: StoneX
provider_slug: stonex
slug: stonex-domain-security
source_filename: stonex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stonex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 23:11:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.payments.stonex.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 11:47:18 2026 GMT\n  hsts: null\n- host: docs.clearing.stonex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: stonex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: stonex.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stonex/refs/heads/main/security/stonex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Financial Services
- Payments
- Clearing
- Futures
- Trading
- Risk Management
---
