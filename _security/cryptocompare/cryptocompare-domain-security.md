---
api_specs:
- filename: cryptocompare-asyncapi.yml
  format: yaml
  label: CryptoCompare Streaming WebSocket
  slug: streamer
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/asyncapi/cryptocompare-asyncapi.yml
- filename: cryptocompare-asset-api-openapi.yml
  format: yaml
  label: CryptoCompare Asset API
  slug: cryptocompare-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-asset-api-openapi.yml
- filename: cryptocompare-blockchain-api-openapi.yml
  format: yaml
  label: CryptoCompare Blockchain API
  slug: cryptocompare-blockchain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-blockchain-api-openapi.yml
- filename: cryptocompare-coins-api-openapi.yml
  format: yaml
  label: CryptoCompare Coins API
  slug: cryptocompare-coins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-coins-api-openapi.yml
- filename: cryptocompare-exchanges-api-openapi.yml
  format: yaml
  label: CryptoCompare Exchanges API
  slug: cryptocompare-exchanges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-exchanges-api-openapi.yml
- filename: cryptocompare-futures-api-openapi.yml
  format: yaml
  label: CryptoCompare Futures API
  slug: cryptocompare-futures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-futures-api-openapi.yml
- filename: cryptocompare-historical-api-openapi.yml
  format: yaml
  label: CryptoCompare Historical API
  slug: cryptocompare-historical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-historical-api-openapi.yml
- filename: cryptocompare-index-api-openapi.yml
  format: yaml
  label: CryptoCompare Index API
  slug: cryptocompare-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-index-api-openapi.yml
- filename: cryptocompare-news-api-openapi.yml
  format: yaml
  label: CryptoCompare News API
  slug: cryptocompare-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-news-api-openapi.yml
- filename: cryptocompare-on-chain-api-openapi.yml
  format: yaml
  label: CryptoCompare On-Chain API
  slug: cryptocompare-on-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-on-chain-api-openapi.yml
- filename: cryptocompare-options-api-openapi.yml
  format: yaml
  label: CryptoCompare Options API
  slug: cryptocompare-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-options-api-openapi.yml
- filename: cryptocompare-order-book-api-openapi.yml
  format: yaml
  label: CryptoCompare Order Book API
  slug: cryptocompare-order-book-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-order-book-api-openapi.yml
- filename: cryptocompare-overview-api-openapi.yml
  format: yaml
  label: CryptoCompare Overview API
  slug: cryptocompare-overview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-overview-api-openapi.yml
- filename: cryptocompare-price-api-openapi.yml
  format: yaml
  label: CryptoCompare Price API
  slug: cryptocompare-price-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-price-api-openapi.yml
- filename: cryptocompare-social-api-openapi.yml
  format: yaml
  label: CryptoCompare Social API
  slug: cryptocompare-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-social-api-openapi.yml
- filename: cryptocompare-spot-api-openapi.yml
  format: yaml
  label: CryptoCompare Spot API
  slug: cryptocompare-spot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-spot-api-openapi.yml
- filename: cryptocompare-top-lists-api-openapi.yml
  format: yaml
  label: CryptoCompare Top Lists API
  slug: cryptocompare-top-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptocompare/refs/heads/main/openapi/cryptocompare-top-lists-api-openapi.yml
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
- Onchain
- Order Book
- Streaming
- Index
---
