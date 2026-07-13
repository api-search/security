---
api_specs:
- filename: openapi.yml
  format: yaml
  label: CryptoNews REST API
  slug: cryptonews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptonews/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cryptonews-api.com
  spf: false
hosts:
- cert_expires: Aug 12 22:54:33 2026 GMT
  host: cryptonews-api.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cryptonews Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CryptoNews API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: CryptoNews API
provider_slug: cryptonews
slug: cryptonews-domain-security
source_filename: cryptonews-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cryptonews-api.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 12 22:54:33 2026 GMT\n  hsts: false\ndomains:\n- domain: cryptonews-api.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cryptonews/refs/heads/main/security/cryptonews-domain-security.yml
summary_line: TLSv1.2
tags:
- Cryptocurrency
- News
- Sentiment Analysis
- Bitcoin
- Market Data
- Whale Transactions
- Crypto Prices
---
