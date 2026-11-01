---
api_specs:
- filename: cow-protocol-account-api-openapi.yml
  format: yaml
  label: CoW Swap Account API
  slug: cow-protocol-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-account-api-openapi.yml
- filename: cow-protocol-app-data-api-openapi.yml
  format: yaml
  label: CoW Swap App Data API
  slug: cow-protocol-app-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-app-data-api-openapi.yml
- filename: cow-protocol-auction-api-openapi.yml
  format: yaml
  label: CoW Swap Auction API
  slug: cow-protocol-auction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-auction-api-openapi.yml
- filename: cow-protocol-notify-api-openapi.yml
  format: yaml
  label: CoW Swap Notify API
  slug: cow-protocol-notify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-notify-api-openapi.yml
- filename: cow-protocol-orders-api-openapi.yml
  format: yaml
  label: CoW Swap Orders API
  slug: cow-protocol-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-orders-api-openapi.yml
- filename: cow-protocol-quote-api-openapi.yml
  format: yaml
  label: CoW Swap Quote API
  slug: cow-protocol-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-quote-api-openapi.yml
- filename: cow-protocol-quotes-api-openapi.yml
  format: yaml
  label: CoW Swap Quotes API
  slug: cow-protocol-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-quotes-api-openapi.yml
- filename: cow-protocol-restricted-api-openapi.yml
  format: yaml
  label: CoW Swap Restricted API
  slug: cow-protocol-restricted-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-restricted-api-openapi.yml
- filename: cow-protocol-reveal-api-openapi.yml
  format: yaml
  label: CoW Swap Reveal API
  slug: cow-protocol-reveal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-reveal-api-openapi.yml
- filename: cow-protocol-settle-api-openapi.yml
  format: yaml
  label: CoW Swap Settle API
  slug: cow-protocol-settle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-settle-api-openapi.yml
- filename: cow-protocol-settle-fast-path-api-openapi.yml
  format: yaml
  label: CoW Swap Settle Fast Path API
  slug: cow-protocol-settle-fast-path-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-settle-fast-path-api-openapi.yml
- filename: cow-protocol-solve-api-openapi.yml
  format: yaml
  label: CoW Swap Solve API
  slug: cow-protocol-solve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-solve-api-openapi.yml
- filename: cow-protocol-solver-competition-api-openapi.yml
  format: yaml
  label: CoW Swap Solver Competition API
  slug: cow-protocol-solver-competition-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-solver-competition-api-openapi.yml
- filename: cow-protocol-token-api-openapi.yml
  format: yaml
  label: CoW Swap Token API
  slug: cow-protocol-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-token-api-openapi.yml
- filename: cow-protocol-trades-api-openapi.yml
  format: yaml
  label: CoW Swap Trades API
  slug: cow-protocol-trades-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-trades-api-openapi.yml
- filename: cow-protocol-transactions-api-openapi.yml
  format: yaml
  label: CoW Swap Transactions API
  slug: cow-protocol-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-transactions-api-openapi.yml
- filename: cow-protocol-users-api-openapi.yml
  format: yaml
  label: CoW Swap Users API
  slug: cow-protocol-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-users-api-openapi.yml
- filename: cow-protocol-version-api-openapi.yml
  format: yaml
  label: CoW Swap Version API
  slug: cow-protocol-version-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-version-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cow.fi
  spf: true
hosts:
- cert_expires: Jan 16 06:05:39 2027 GMT
  host: cow.fi
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cow Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoW Swap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CoW Swap
provider_slug: cow-protocol
slug: cow-protocol-domain-security
source_filename: cow-protocol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cow.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 06:05:39 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cow.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cow-protocol/security/cow-protocol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DeFi
- Ethereum
- Swap
- Liquidity
- Governance
- AMM
---
