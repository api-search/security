---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Paidy Payments API
  slug: paidy-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidy/refs/heads/main/openapi/openapi.yml
- filename: openapi.yml
  format: yaml
  label: Paidy Tokens API
  slug: paidy-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paidy/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: paidy.com
  spf: true
hosts:
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: paidy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: api.paidy.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: apps.paidy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paidy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paidy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Paidy
provider_slug: paidy
slug: paidy-domain-security
source_filename: paidy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paidy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.paidy.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: null\n- host: apps.paidy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: paidy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paidy/refs/heads/main/security/paidy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Buy Now Pay Later
- BNPL
- Payments
- Japan
- Checkout
- Deferred Payments
- Recurring Payments
- Tokens
---
