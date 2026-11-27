---
api_specs:
- filename: coinmate-account-api-openapi.yml
  format: yaml
  label: Coinmate Account API
  slug: coinmate-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-account-api-openapi.yml
- filename: coinmate-bitcoin-api-openapi.yml
  format: yaml
  label: Coinmate Bitcoin API
  slug: coinmate-bitcoin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-bitcoin-api-openapi.yml
- filename: coinmate-cardano-api-openapi.yml
  format: yaml
  label: Coinmate Cardano API
  slug: coinmate-cardano-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-cardano-api-openapi.yml
- filename: coinmate-currencies-api-openapi.yml
  format: yaml
  label: Coinmate Currencies API
  slug: coinmate-currencies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-currencies-api-openapi.yml
- filename: coinmate-ethereum-api-openapi.yml
  format: yaml
  label: Coinmate Ethereum API
  slug: coinmate-ethereum-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-ethereum-api-openapi.yml
- filename: coinmate-fiat-api-openapi.yml
  format: yaml
  label: Coinmate FIAT API
  slug: coinmate-fiat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-fiat-api-openapi.yml
- filename: coinmate-history-api-openapi.yml
  format: yaml
  label: Coinmate History API
  slug: coinmate-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-history-api-openapi.yml
- filename: coinmate-litecoin-api-openapi.yml
  format: yaml
  label: Coinmate Litecoin API
  slug: coinmate-litecoin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-litecoin-api-openapi.yml
- filename: coinmate-market-data-api-openapi.yml
  format: yaml
  label: Coinmate Market Data API
  slug: coinmate-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-market-data-api-openapi.yml
- filename: coinmate-orders-api-openapi.yml
  format: yaml
  label: Coinmate Orders API
  slug: coinmate-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-orders-api-openapi.yml
- filename: coinmate-ripple-api-openapi.yml
  format: yaml
  label: Coinmate Ripple API
  slug: coinmate-ripple-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-ripple-api-openapi.yml
- filename: coinmate-solana-api-openapi.yml
  format: yaml
  label: Coinmate Solana API
  slug: coinmate-solana-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-solana-api-openapi.yml
- filename: coinmate-system-api-openapi.yml
  format: yaml
  label: Coinmate System API
  slug: coinmate-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-system-api-openapi.yml
- filename: coinmate-virtual-currency-api-openapi.yml
  format: yaml
  label: Coinmate Virtual Currency API
  slug: coinmate-virtual-currency-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-virtual-currency-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: coinmate.io
  spf: true
hosts:
- cert_expires: Dec 23 13:44:55 2026 GMT
  host: coinmate.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coinmate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coinmate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Coinmate
provider_slug: coinmate
slug: coinmate-domain-security
source_filename: coinmate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coinmate.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 13:44:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coinmate.io\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/coinmate/security/coinmate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cryptocurrency Exchange
- Trading Platform
- Recurring Buy
- Premium Trading
- Czech Market
---
