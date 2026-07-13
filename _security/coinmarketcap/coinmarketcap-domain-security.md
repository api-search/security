---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coinmarketcap.com
  spf: true
hosts:
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: coinmarketcap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: pro-api.coinmarketcap.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coinmarketcap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoinMarketCap, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CoinMarketCap
provider_slug: coinmarketcap
slug: coinmarketcap-domain-security
source_filename: coinmarketcap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coinmarketcap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pro-api.coinmarketcap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: coinmarketcap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinmarketcap/refs/heads/main/security/coinmarketcap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web3
- Crypto
- Market Data
- Rankings
- DEX
- Exchanges
- Cryptocurrency
---
