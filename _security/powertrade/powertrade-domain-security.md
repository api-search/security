---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: power.trade
  spf: true
hosts:
- cert_expires: Sep 26 15:48:24 2026 GMT
  host: power.trade
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 01:27:37 2026 GMT
  host: api.rest.prod.power.trade
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 01:27:50 2026 GMT
  host: api.wss.prod.power.trade
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Powertrade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PowerTrade, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PowerTrade
provider_slug: powertrade
slug: powertrade-domain-security
source_filename: powertrade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: power.trade\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 15:48:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.rest.prod.power.trade\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 01:27:37 2026 GMT\n  hsts: null\n- host: api.wss.prod.power.trade\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 01:27:50 2026 GMT\n  hsts: null\ndomains:\n- domain: power.trade\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powertrade/refs/heads/main/security/powertrade-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Cryptocurrency
- Derivatives
- Options
- Perpetual Futures
- Trading
- Exchange
- Financial Services
- WebSocket
- FIX
- Market Data
---
