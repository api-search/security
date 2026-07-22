---
api_specs:
- filename: totalis-openapi-original.json
  format: json
  label: Totalis RFQ API
  slug: totalis-rfq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/totalis/refs/heads/main/openapi/totalis-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: totalis.trade
  spf: true
hosts:
- cert_expires: Sep  9 15:00:29 2026 GMT
  host: www.totalis.trade
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 18:23:00 2026 GMT
  host: docs.totalis.trade
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 18:11:10 2026 GMT
  host: api.totalis.trade
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Totalis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Totalis, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Totalis
provider_slug: totalis
slug: totalis-domain-security
source_filename: totalis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.totalis.trade\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 15:00:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.totalis.trade\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 18:23:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.totalis.trade\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 18:11:10 2026 GMT\n  hsts: false\ndomains:\n- domain: totalis.trade\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/totalis/refs/heads/main/security/totalis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Prediction Markets
- Derivatives
- Parlays
- Trading
- RFQ
- Solana
- Crypto Web3
- Market Data
- Webhooks
---
