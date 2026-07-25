---
api_specs:
- filename: gmx-allowances-api-openapi.yml
  format: yaml
  label: GMX Allowances API
  slug: gmx-allowances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-allowances-api-openapi.yml
- filename: gmx-apy-api-openapi.yml
  format: yaml
  label: GMX APY API
  slug: gmx-apy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-apy-api-openapi.yml
- filename: gmx-balances-api-openapi.yml
  format: yaml
  label: GMX Balances API
  slug: gmx-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-balances-api-openapi.yml
- filename: gmx-buyback-api-openapi.yml
  format: yaml
  label: GMX Buyback API
  slug: gmx-buyback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-buyback-api-openapi.yml
- filename: gmx-gmx-account-api-openapi.yml
  format: yaml
  label: GMX GMX Account API
  slug: gmx-gmx-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-gmx-account-api-openapi.yml
- filename: gmx-jit-api-openapi.yml
  format: yaml
  label: GMX JIT API
  slug: gmx-jit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-jit-api-openapi.yml
- filename: gmx-markets-api-openapi.yml
  format: yaml
  label: GMX Markets API
  slug: gmx-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-markets-api-openapi.yml
- filename: gmx-order-transactions-api-openapi.yml
  format: yaml
  label: GMX Order Transactions API
  slug: gmx-order-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-order-transactions-api-openapi.yml
- filename: gmx-orders-api-openapi.yml
  format: yaml
  label: GMX Orders API
  slug: gmx-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-orders-api-openapi.yml
- filename: gmx-pairs-api-openapi.yml
  format: yaml
  label: GMX Pairs API
  slug: gmx-pairs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-pairs-api-openapi.yml
- filename: gmx-performance-api-openapi.yml
  format: yaml
  label: GMX Performance API
  slug: gmx-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-performance-api-openapi.yml
- filename: gmx-positions-api-openapi.yml
  format: yaml
  label: GMX Positions API
  slug: gmx-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-positions-api-openapi.yml
- filename: gmx-prices-api-openapi.yml
  format: yaml
  label: GMX Prices API
  slug: gmx-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-prices-api-openapi.yml
- filename: gmx-rates-api-openapi.yml
  format: yaml
  label: GMX Rates API
  slug: gmx-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-rates-api-openapi.yml
- filename: gmx-staking-api-openapi.yml
  format: yaml
  label: GMX Staking API
  slug: gmx-staking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-staking-api-openapi.yml
- filename: gmx-subaccounts-api-openapi.yml
  format: yaml
  label: GMX Subaccounts API
  slug: gmx-subaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-subaccounts-api-openapi.yml
- filename: gmx-tokens-api-openapi.yml
  format: yaml
  label: GMX Tokens API
  slug: gmx-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-tokens-api-openapi.yml
- filename: gmx-trades-api-openapi.yml
  format: yaml
  label: GMX Trades API
  slug: gmx-trades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-trades-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: gmx.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: gmxapi.io
  spf: false
hosts:
- cert_expires: Aug 22 20:16:09 2026 GMT
  host: gmx.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 22:31:50 2026 GMT
  host: docs.gmx.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 01:17:29 2026 GMT
  host: arbitrum.gmxapi.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gmx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GMX, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: GMX
provider_slug: gmx
slug: gmx-domain-security
source_filename: gmx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gmx.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 20:16:09 2026 GMT\n  hsts: false\n- host: docs.gmx.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 22:31:50 2026 GMT\n  hsts: false\n- host: arbitrum.gmxapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 01:17:29 2026 GMT\n  hsts: null\ndomains:\n- domain: gmx.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gmxapi.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/security/gmx-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- DeFi
- Perpetual Exchange
- DEX
- Trading
- Leverage
- Liquidity Pools
- GLP
- GM Tokens
- GLV
- Arbitrum
- Avalanche
- Web3
---
