---
api_specs:
- filename: cryptocompare-min-api-openapi.yml
  format: yaml
  label: CryptoCompare min-api (Legacy)
  slug: min-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-min-api-openapi.yml
- filename: cryptocompare-data-api-openapi.yml
  format: yaml
  label: CoinDesk Data API (CCData)
  slug: data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-data-api-openapi.yml
- filename: cryptocompare-asyncapi.yml
  format: yaml
  label: CryptoCompare Streaming WebSocket
  slug: streamer
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/asyncapi/cryptocompare-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coindesk.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cryptocompare.com
  spf: true
hosts:
- cert_expires: Oct  7 14:06:11 2026 GMT
  host: data.coindesk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 15:02:27 2026 GMT
  host: developers.coindesk.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 19 22:09:34 2026 GMT
  host: min-api.cryptocompare.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cryptocompare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CryptoCompare, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CryptoCompare
provider_slug: cryptocompare
slug: cryptocompare-domain-security
source_filename: cryptocompare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.coindesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 14:06:11 2026 GMT\n  hsts: false\n- host: developers.coindesk.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  4 15:02:27 2026 GMT\n  hsts: false\n- host: min-api.cryptocompare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 22:09:34 2026 GMT\n  hsts: null\ndomains:\n- domain: coindesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cryptocompare.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/security/cryptocompare-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Cryptocurrency
- Market Data
- Reference Rates
- News
- Social
- Blockchain
- On-Chain
- Order Book
- Streaming
- Index
---
