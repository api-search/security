---
api_specs:
- filename: alpaca-trading-api-openapi.yml
  format: yaml
  label: Alpaca Trading API
  slug: trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-trading-api-openapi.yml
- filename: alpaca-data-api-openapi.yml
  format: yaml
  label: Alpaca Market Data API
  slug: market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-data-api-openapi.yml
- filename: alpaca-broker-api-openapi.yml
  format: yaml
  label: Alpaca Broker API
  slug: broker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-broker-api-openapi.yml
- filename: alpaca-oauth-api-openapi.yml
  format: yaml
  label: Alpaca OAuth API
  slug: oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-oauth-api-openapi.yml
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
