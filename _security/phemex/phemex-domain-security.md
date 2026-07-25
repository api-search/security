---
api_specs:
- filename: phemex-account-api-openapi.yml
  format: yaml
  label: Phemex Account API
  slug: phemex-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/phemex-account-api-openapi.yml
- filename: phemex-conversion-api-openapi.yml
  format: yaml
  label: Phemex Conversion API
  slug: phemex-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/phemex-conversion-api-openapi.yml
- filename: phemex-market-data-api-openapi.yml
  format: yaml
  label: Phemex Market Data API
  slug: phemex-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/phemex-market-data-api-openapi.yml
- filename: phemex-orders-api-openapi.yml
  format: yaml
  label: Phemex Orders API
  slug: phemex-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/phemex-orders-api-openapi.yml
- filename: phemex-positions-api-openapi.yml
  format: yaml
  label: Phemex Positions API
  slug: phemex-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/phemex-positions-api-openapi.yml
- filename: phemex-sub-account-transfers-api-openapi.yml
  format: yaml
  label: Phemex Sub-Account Transfers API
  slug: phemex-sub-account-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/phemex-sub-account-transfers-api-openapi.yml
- filename: phemex-trades-api-openapi.yml
  format: yaml
  label: Phemex Trades API
  slug: phemex-trades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/phemex-trades-api-openapi.yml
- filename: phemex-transfers-api-openapi.yml
  format: yaml
  label: Phemex Transfers API
  slug: phemex-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/phemex-transfers-api-openapi.yml
- filename: phemex-wallets-api-openapi.yml
  format: yaml
  label: Phemex Wallets API
  slug: phemex-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/phemex-wallets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: phemex.com
  spf: true
hosts:
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: api.phemex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: testnet-api.phemex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Phemex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phemex, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Phemex
provider_slug: phemex
slug: phemex-domain-security
source_filename: phemex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.phemex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: null\n- host: testnet-api.phemex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: phemex.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/security/phemex-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Cryptocurrency
- Derivatives
- Spot Trading
- Perpetual Contracts
- Futures
- WebSocket
- Market Data
---
