---
api_specs:
- filename: flexa-openapi.json
  format: json
  label: Flexa API
  slug: flexa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexa/refs/heads/main/openapi/flexa-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flexa.co
  spf: true
hosts:
- cert_expires: Sep  8 09:32:11 2026 GMT
  host: flexa.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 06:33:54 2026 GMT
  host: docs.flexa.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 04:33:16 2026 GMT
  host: api.flexa.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flexa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flexa, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Flexa
provider_slug: flexa
slug: flexa-domain-security
source_filename: flexa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flexa.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 09:32:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.flexa.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 06:33:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.flexa.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 04:33:16 2026 GMT\n  hsts: null\ndomains:\n- domain: flexa.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flexa/refs/heads/main/security/flexa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Payments
- Digital Currency
- Cryptocurrency
- Fintech
- Blockchain
- Merchant Payments
- Web3
---
