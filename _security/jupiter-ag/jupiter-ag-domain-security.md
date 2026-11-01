---
api_specs:
- filename: jupiter-ag-events-api-openapi.yml
  format: yaml
  label: Jupiter Events API
  slug: jupiter-ag-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-events-api-openapi.yml
- filename: jupiter-ag-forecast-api-openapi.yml
  format: yaml
  label: Jupiter Forecast API
  slug: jupiter-ag-forecast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-forecast-api-openapi.yml
- filename: jupiter-ag-history-api-openapi.yml
  format: yaml
  label: Jupiter History API
  slug: jupiter-ag-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-history-api-openapi.yml
- filename: jupiter-ag-leaderboards-api-openapi.yml
  format: yaml
  label: Jupiter Leaderboards API
  slug: jupiter-ag-leaderboards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-leaderboards-api-openapi.yml
- filename: jupiter-ag-markets-api-openapi.yml
  format: yaml
  label: Jupiter Markets API
  slug: jupiter-ag-markets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-markets-api-openapi.yml
- filename: jupiter-ag-orderbook-api-openapi.yml
  format: yaml
  label: Jupiter Orderbook API
  slug: jupiter-ag-orderbook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-orderbook-api-openapi.yml
- filename: jupiter-ag-orders-api-openapi.yml
  format: yaml
  label: Jupiter Orders API
  slug: jupiter-ag-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-orders-api-openapi.yml
- filename: jupiter-ag-positions-api-openapi.yml
  format: yaml
  label: Jupiter Positions API
  slug: jupiter-ag-positions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-positions-api-openapi.yml
- filename: jupiter-ag-profile-api-openapi.yml
  format: yaml
  label: Jupiter Profile API
  slug: jupiter-ag-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-profile-api-openapi.yml
- filename: jupiter-ag-trades-api-openapi.yml
  format: yaml
  label: Jupiter Trades API
  slug: jupiter-ag-trades-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-trades-api-openapi.yml
- filename: jupiter-ag-trading-api-openapi.yml
  format: yaml
  label: Jupiter Trading API
  slug: jupiter-ag-trading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-trading-api-openapi.yml
- filename: jupiter-ag-vault-api-openapi.yml
  format: yaml
  label: Jupiter Vault API
  slug: jupiter-ag-vault-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-vault-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: jup.ag
  spf: true
hosts:
- cert_expires: Oct  8 08:47:09 2026 GMT
  host: jup.ag
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 22:12:57 2026 GMT
  host: dev.jup.ag
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: api.jup.ag
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Jupiter Ag Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jupiter, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Jupiter
provider_slug: jupiter-ag
slug: jupiter-ag-domain-security
source_filename: jupiter-ag-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jup.ag\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 08:47:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dev.jup.ag\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 22:12:57 2026 GMT\n  hsts: false\n- host: api.jup.ag\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: jup.ag\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/jupiter-ag/security/jupiter-ag-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Solana
- DeFi
- DEX Aggregator
- Swap
- Perpetuals
- Limit Orders
- DCA
- Lending
---
