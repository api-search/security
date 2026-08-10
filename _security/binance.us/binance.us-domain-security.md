---
api_specs:
- filename: binance.us-websocket-api-asyncapi.yml
  format: yaml
  label: Binance.US WebSocket API
  slug: websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance.us/refs/heads/main/asyncapi/binance.us-websocket-api-asyncapi.yml
- filename: binance.us-websocket-streams-asyncapi.yml
  format: yaml
  label: Binance.US WebSocket Streams
  slug: websocket-streams
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance.us/refs/heads/main/asyncapi/binance.us-websocket-streams-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: binance.us
  spf: true
hosts:
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: www.binance.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: docs.binance.us
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: api.binance.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Binance.Us Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Binance.US, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Binance.US
provider_slug: binance.us
slug: binance.us-domain-security
source_filename: binance.us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.binance.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.binance.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: false\n- host: api.binance.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: binance.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/binance.us/refs/heads/main/security/binance.us-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Digital Assets
- Exchange
- Trading
- Market Data
- Financial Services
- WebSocket
- Custody
- Staking
---
