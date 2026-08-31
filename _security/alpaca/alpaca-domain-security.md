---
api_specs:
- filename: alpaca-trading-api-openapi.yml
  format: yaml
  label: Alpaca Trading API
  slug: trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-trading-api-openapi.yml
- filename: alpaca-oauth-api-openapi.yml
  format: yaml
  label: Alpaca OAuth API
  slug: oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-oauth-api-openapi.yml
- filename: alpaca-accounts-api-openapi.yml
  format: yaml
  label: Alpaca Accounts API
  slug: alpaca-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-accounts-api-openapi.yml
- filename: alpaca-assets-api-openapi.yml
  format: yaml
  label: Alpaca Assets API
  slug: alpaca-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-assets-api-openapi.yml
- filename: alpaca-calendar-api-openapi.yml
  format: yaml
  label: Alpaca Calendar API
  slug: alpaca-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-calendar-api-openapi.yml
- filename: alpaca-clock-api-openapi.yml
  format: yaml
  label: Alpaca Clock API
  slug: alpaca-clock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-clock-api-openapi.yml
- filename: alpaca-corporate-actions-api-openapi.yml
  format: yaml
  label: Alpaca Corporate Actions API
  slug: alpaca-corporate-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-corporate-actions-api-openapi.yml
- filename: alpaca-crypto-pricing-data-api-api-openapi.yml
  format: yaml
  label: Alpaca Crypto Pricing Data API API
  slug: alpaca-crypto-pricing-data-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-crypto-pricing-data-api-api-openapi.yml
- filename: alpaca-documents-api-openapi.yml
  format: yaml
  label: Alpaca Documents API
  slug: alpaca-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-documents-api-openapi.yml
- filename: alpaca-events-api-openapi.yml
  format: yaml
  label: Alpaca Events API
  slug: alpaca-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-events-api-openapi.yml
- filename: alpaca-funding-api-openapi.yml
  format: yaml
  label: Alpaca Funding API
  slug: alpaca-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-funding-api-openapi.yml
- filename: alpaca-journals-api-openapi.yml
  format: yaml
  label: Alpaca Journals API
  slug: alpaca-journals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-journals-api-openapi.yml
- filename: alpaca-logo-api-openapi.yml
  format: yaml
  label: Alpaca Logo API
  slug: alpaca-logo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-logo-api-openapi.yml
- filename: alpaca-news-api-openapi.yml
  format: yaml
  label: Alpaca News API
  slug: alpaca-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-news-api-openapi.yml
- filename: alpaca-screener-api-openapi.yml
  format: yaml
  label: Alpaca Screener API
  slug: alpaca-screener-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-screener-api-openapi.yml
- filename: alpaca-stock-pricing-data-api-api-openapi.yml
  format: yaml
  label: Alpaca Stock Pricing Data API API
  slug: alpaca-stock-pricing-data-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-stock-pricing-data-api-api-openapi.yml
- filename: alpaca-watchlist-api-openapi.yml
  format: yaml
  label: Alpaca Watchlist API
  slug: alpaca-watchlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-watchlist-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alpaca.markets
  spf: true
hosts:
- cert_expires: Sep 14 13:31:07 2026 GMT
  host: alpaca.markets
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 20:13:14 2026 GMT
  host: docs.alpaca.markets
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 18:17:22 2026 GMT
  host: api.alpaca.markets
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alpaca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alpaca, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alpaca
provider_slug: alpaca
slug: alpaca-domain-security
source_filename: alpaca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alpaca.markets\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 13:31:07 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: docs.alpaca.markets\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 20:13:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.alpaca.markets\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 18:17:22 2026 GMT\n  hsts: null\ndomains:\n- domain: alpaca.markets\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/security/alpaca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Trading
- Stocks
- Crypto
- Brokerage
- Market Data
- Options
---
