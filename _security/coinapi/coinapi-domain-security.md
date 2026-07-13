---
api_specs:
- filename: coinapi-asyncapi.yml
  format: yaml
  label: CoinAPI Market Data API
  slug: market-data-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinapi/refs/heads/main/asyncapi/coinapi-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: coinapi.io
  spf: true
hosts:
- cert_expires: Sep 22 13:42:46 2026 GMT
  host: www.coinapi.io
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 11:04:39 2026 GMT
  host: rest.coinapi.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coinapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoinAPI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: CoinAPI
provider_slug: coinapi
slug: coinapi-domain-security
source_filename: coinapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coinapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 13:42:46 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: rest.coinapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 11:04:39 2026 GMT\n  hsts: null\ndomains:\n- domain: coinapi.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinapi/refs/heads/main/security/coinapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Crypto Indexes
- Crypto Metrics
- Cryptocurrency
- EMS
- Execution Management
- FIX
- Market Data
- Order Books
- REST
- WebSocket
---
