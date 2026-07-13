---
api_specs:
- filename: account-status.json
  format: json
  label: tastytrade REST API
  slug: tastytrade-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tastytrade/refs/heads/main/openapi/account-status.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tastytrade.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tastyworks.com
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: developer.tastytrade.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: tastytrade.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 23:59:59 2026 GMT
  host: api.tastyworks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tastytrade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tastytrade, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: tastytrade
provider_slug: tastytrade
slug: tastytrade-domain-security
source_filename: tastytrade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.tastytrade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: false\n- host: tastytrade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.tastyworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tastytrade.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: tastyworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tastytrade/refs/heads/main/security/tastytrade-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Brokerage
- Trading
- Options
- Futures
- Equities
- Crypto
- Market Data
- WebSocket
---
