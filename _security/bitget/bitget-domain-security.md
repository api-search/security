---
api_specs:
- filename: intro
  format: yaml
  label: Bitget Spot Trading API
  slug: bitget-spot-trading-api
  spec_type: OpenAPI
  url: https://www.bitget.com/api-doc/spot/intro
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bitget.com
  spf: true
hosts:
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: www.bitget.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: api.bitget.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: ws.bitget.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitget Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitget, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bitget
provider_slug: bitget
slug: bitget-domain-security
source_filename: bitget-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bitget.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.bitget.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: null\n- host: ws.bitget.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bitget.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitget/refs/heads/main/security/bitget-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Exchange
- Spot Trading
- Futures
- Perpetual Contracts
- Copy Trading
- WebSocket
- Finance
---
