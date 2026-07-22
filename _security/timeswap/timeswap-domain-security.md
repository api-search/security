---
api_specs:
- filename: timeswap-api-openapi.json
  format: json
  label: Timeswap API
  slug: timeswap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timeswap/refs/heads/main/openapi/timeswap-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: timeswap.io
  spf: true
hosts:
- cert_expires: Aug 27 19:33:50 2026 GMT
  host: timeswap.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 00:08:12 2026 GMT
  host: api.timeswap.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Timeswap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Timeswap, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Timeswap
provider_slug: timeswap
slug: timeswap-domain-security
source_filename: timeswap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: timeswap.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:33:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.timeswap.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 00:08:12 2026 GMT\n  hsts: null\ndomains:\n- domain: timeswap.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/timeswap/refs/heads/main/security/timeswap-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Crypto Web3
- DeFi
- Lending
- Borrowing
- Liquidity Pools
- Fixed Income
- Blockchain
---
