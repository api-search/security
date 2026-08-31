---
api_specs:
- filename: zerion-chains-api-openapi.yml
  format: yaml
  label: Zerion chains API
  slug: zerion-chains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerion/refs/heads/main/openapi/zerion-chains-api-openapi.yml
- filename: zerion-dapps-api-openapi.yml
  format: yaml
  label: Zerion dapps API
  slug: zerion-dapps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerion/refs/heads/main/openapi/zerion-dapps-api-openapi.yml
- filename: zerion-fungibles-api-openapi.yml
  format: yaml
  label: Zerion fungibles API
  slug: zerion-fungibles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerion/refs/heads/main/openapi/zerion-fungibles-api-openapi.yml
- filename: zerion-gas-api-openapi.yml
  format: yaml
  label: Zerion gas API
  slug: zerion-gas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerion/refs/heads/main/openapi/zerion-gas-api-openapi.yml
- filename: zerion-nfts-api-openapi.yml
  format: yaml
  label: Zerion nfts API
  slug: zerion-nfts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerion/refs/heads/main/openapi/zerion-nfts-api-openapi.yml
- filename: zerion-subscriptions-to-transactions-api-openapi.yml
  format: yaml
  label: Zerion subscriptions to transactions API
  slug: zerion-subscriptions-to-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerion/refs/heads/main/openapi/zerion-subscriptions-to-transactions-api-openapi.yml
- filename: zerion-swap-api-openapi.yml
  format: yaml
  label: Zerion swap API
  slug: zerion-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerion/refs/heads/main/openapi/zerion-swap-api-openapi.yml
- filename: zerion-wallet-sets-api-openapi.yml
  format: yaml
  label: Zerion wallet sets API
  slug: zerion-wallet-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerion/refs/heads/main/openapi/zerion-wallet-sets-api-openapi.yml
- filename: zerion-wallets-api-openapi.yml
  format: yaml
  label: Zerion wallets API
  slug: zerion-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerion/refs/heads/main/openapi/zerion-wallets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zerion.io
  spf: true
hosts:
- cert_expires: Oct  3 14:49:57 2026 GMT
  host: developers.zerion.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 01:57:44 2026 GMT
  host: api.zerion.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zerion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zerion, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zerion
provider_slug: zerion
slug: zerion-domain-security
source_filename: zerion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.zerion.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:49:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.zerion.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 01:57:44 2026 GMT\n  hsts: null\ndomains:\n- domain: zerion.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zerion/refs/heads/main/security/zerion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Web3
- Blockchain
- Cryptocurrency
- DeFi
- Wallets
- NFT
- Ethereum
- Solana
- Portfolio
- Onchain Data
- Transaction
---
