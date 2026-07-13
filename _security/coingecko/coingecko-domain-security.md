---
api_specs:
- filename: coingecko-crypto-market-data-api-openapi.yml
  format: yaml
  label: CoinGecko Crypto Market Data API
  slug: crypto-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coingecko/refs/heads/main/openapi/coingecko-crypto-market-data-api-openapi.yml
- filename: coingecko-pro-api-openapi.yml
  format: yaml
  label: CoinGecko Pro API
  slug: pro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coingecko/refs/heads/main/openapi/coingecko-pro-api-openapi.yml
- filename: coingecko-onchain-dex-api-openapi.yml
  format: yaml
  label: CoinGecko Onchain DEX API
  slug: onchain-dex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coingecko/refs/heads/main/openapi/coingecko-onchain-dex-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coingecko.com
  spf: true
hosts:
- cert_expires: Sep 23 14:12:30 2026 GMT
  host: www.coingecko.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 09:27:30 2026 GMT
  host: docs.coingecko.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 18:14:10 2026 GMT
  host: api.coingecko.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coingecko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoinGecko, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CoinGecko
provider_slug: coingecko
slug: coingecko-domain-security
source_filename: coingecko-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coingecko.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 14:12:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.coingecko.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 09:27:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.coingecko.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 18:14:10 2026 GMT\n  hsts: null\ndomains:\n- domain: coingecko.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coingecko/refs/heads/main/security/coingecko-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aggregator
- Blockchain
- Cryptocurrency
- Decentralized Exchanges
- DeFi
- DEX
- Exchanges
- Liquidity Pools
- Market Data
- NFTs
- Onchain Data
- Prices
---
