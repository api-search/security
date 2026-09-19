---
api_specs:
- filename: bitculator-alarms-api-openapi.yml
  format: yaml
  label: Bitculator Alarms API
  slug: bitculator-alarms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-alarms-api-openapi.yml
- filename: bitculator-calculators-api-openapi.yml
  format: yaml
  label: Bitculator Calculators API
  slug: bitculator-calculators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-calculators-api-openapi.yml
- filename: bitculator-coins-api-openapi.yml
  format: yaml
  label: Bitculator Coins API
  slug: bitculator-coins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-coins-api-openapi.yml
- filename: bitculator-conversion-api-openapi.yml
  format: yaml
  label: Bitculator Conversion API
  slug: bitculator-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-conversion-api-openapi.yml
- filename: bitculator-editorial-api-openapi.yml
  format: yaml
  label: Bitculator Editorial API
  slug: bitculator-editorial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-editorial-api-openapi.yml
- filename: bitculator-exchanges-api-openapi.yml
  format: yaml
  label: Bitculator Exchanges API
  slug: bitculator-exchanges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-exchanges-api-openapi.yml
- filename: bitculator-global-market-api-openapi.yml
  format: yaml
  label: Bitculator Global Market API
  slug: bitculator-global-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-global-market-api-openapi.yml
- filename: bitculator-indicators-api-openapi.yml
  format: yaml
  label: Bitculator Indicators API
  slug: bitculator-indicators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-indicators-api-openapi.yml
- filename: bitculator-liquidations-api-openapi.yml
  format: yaml
  label: Bitculator Liquidations API
  slug: bitculator-liquidations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-liquidations-api-openapi.yml
- filename: bitculator-markets-api-openapi.yml
  format: yaml
  label: Bitculator Markets API
  slug: bitculator-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-markets-api-openapi.yml
- filename: bitculator-meta-api-openapi.yml
  format: yaml
  label: Bitculator Meta API
  slug: bitculator-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-meta-api-openapi.yml
- filename: bitculator-prices-api-openapi.yml
  format: yaml
  label: Bitculator Prices API
  slug: bitculator-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-prices-api-openapi.yml
- filename: bitculator-sentiment-api-openapi.yml
  format: yaml
  label: Bitculator Sentiment API
  slug: bitculator-sentiment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-sentiment-api-openapi.yml
- filename: bitculator-wallets-api-openapi.yml
  format: yaml
  label: Bitculator Wallets API
  slug: bitculator-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-wallets-api-openapi.yml
- filename: bitculator-webhooks-api-openapi.yml
  format: yaml
  label: Bitculator Webhooks API
  slug: bitculator-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bitculator.com
  spf: true
hosts:
- cert_expires: Nov  4 14:41:07 2026 GMT
  host: bitculator.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bitculator Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitculator, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bitculator
provider_slug: bitculator
slug: bitculator-domain-security
source_filename: bitculator-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitculator.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 14:41:07 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: bitculator.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/security/bitculator-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cryptocurrency
- crypto-market-data
- Blockchain
- Finance
- Fintech
- Web3
- Trading
- Exchange Data
- Wallets
- Sentiment
- Indicators
---
