---
api_specs:
- filename: coinspot-public-api-api-openapi.yml
  format: yaml
  label: CoinSpot Public API
  slug: coinspot-public-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinspot/refs/heads/main/openapi/coinspot-public-api-api-openapi.yml
- filename: coinspot-read-only-api-api-openapi.yml
  format: yaml
  label: CoinSpot Read Only API
  slug: coinspot-read-only-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinspot/refs/heads/main/openapi/coinspot-read-only-api-api-openapi.yml
- filename: coinspot-trading-api-api-openapi.yml
  format: yaml
  label: CoinSpot Trading API
  slug: coinspot-trading-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinspot/refs/heads/main/openapi/coinspot-trading-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coinspot.com.au
  spf: true
hosts:
- cert_expires: Dec 13 23:27:13 2026 GMT
  host: www.coinspot.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coinspot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoinSpot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CoinSpot
provider_slug: coinspot
slug: coinspot-domain-security
source_filename: coinspot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coinspot.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:27:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: coinspot.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinspot/refs/heads/main/security/coinspot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Australia
- Bitcoin
- Market Data
---
