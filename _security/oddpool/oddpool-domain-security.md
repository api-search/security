---
api_specs:
- filename: oddpool-feeds-asyncapi.yml
  format: yaml
  label: Oddpool WebSocket Feeds
  slug: oddpool-websocket-feeds
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/oddpool/refs/heads/main/asyncapi/oddpool-feeds-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oddpool.com
  spf: true
hosts:
- cert_expires: Sep 29 13:58:44 2026 GMT
  host: www.oddpool.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 00:47:51 2026 GMT
  host: docs.oddpool.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 24 05:02:59 2026 GMT
  host: api.oddpool.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oddpool Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oddpool, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Oddpool
provider_slug: oddpool
slug: oddpool-domain-security
source_filename: oddpool-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oddpool.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 13:58:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.oddpool.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 00:47:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.oddpool.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 24 05:02:59 2026 GMT\n  hsts: null\ndomains:\n- domain: oddpool.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oddpool/refs/heads/main/security/oddpool-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Prediction Markets
- Market Data
- Financial Data
- Trading
- Fintech
- Data Aggregation
- WebSocket
- Historical Data
- Kalshi
- Polymarket
---
