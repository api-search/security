---
api_specs:
- filename: getpaid-openapi-original.yml
  format: yaml
  label: Getpaid API v2
  slug: getpaid-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getpaid/refs/heads/main/openapi/getpaid-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getpaid.io
  spf: true
hosts:
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: api.getpaid.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: api.sandbox.getpaid.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Getpaid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GetPaid, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GetPaid
provider_slug: getpaid
slug: getpaid-domain-security
source_filename: getpaid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.getpaid.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: null\n- host: api.sandbox.getpaid.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: getpaid.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getpaid/refs/heads/main/security/getpaid-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Embedded Payments
- Split Settlement
- Checkout
- Marketplace
- Onboarding
- Subscriptions
- Agent Payments
- Europe
---
