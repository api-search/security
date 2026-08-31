---
api_specs:
- filename: covalent-abi-api-openapi.yml
  format: yaml
  label: Covalent ABI API
  slug: covalent-abi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-abi-api-openapi.yml
- filename: covalent-balances-api-openapi.yml
  format: yaml
  label: Covalent Balances API
  slug: covalent-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-balances-api-openapi.yml
- filename: covalent-base-api-openapi.yml
  format: yaml
  label: Covalent Base API
  slug: covalent-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-base-api-openapi.yml
- filename: covalent-bitcoin-api-openapi.yml
  format: yaml
  label: Covalent Bitcoin API
  slug: covalent-bitcoin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-bitcoin-api-openapi.yml
- filename: covalent-cross-chain-api-openapi.yml
  format: yaml
  label: Covalent Cross-Chain API
  slug: covalent-cross-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-cross-chain-api-openapi.yml
- filename: covalent-data-api-openapi.yml
  format: yaml
  label: Covalent Data API
  slug: covalent-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-data-api-openapi.yml
- filename: covalent-destinations-api-openapi.yml
  format: yaml
  label: Covalent Destinations API
  slug: covalent-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-destinations-api-openapi.yml
- filename: covalent-discovery-api-openapi.yml
  format: yaml
  label: Covalent Discovery API
  slug: covalent-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-discovery-api-openapi.yml
- filename: covalent-graphql-api-openapi.yml
  format: yaml
  label: Covalent GraphQL API
  slug: covalent-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-graphql-api-openapi.yml
- filename: covalent-info-api-openapi.yml
  format: yaml
  label: Covalent Info API
  slug: covalent-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-info-api-openapi.yml
- filename: covalent-nft-api-openapi.yml
  format: yaml
  label: Covalent NFT API
  slug: covalent-nft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-nft-api-openapi.yml
- filename: covalent-pipelines-api-openapi.yml
  format: yaml
  label: Covalent Pipelines API
  slug: covalent-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-pipelines-api-openapi.yml
- filename: covalent-pricing-api-openapi.yml
  format: yaml
  label: Covalent Pricing API
  slug: covalent-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-pricing-api-openapi.yml
- filename: covalent-security-api-openapi.yml
  format: yaml
  label: Covalent Security API
  slug: covalent-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-security-api-openapi.yml
- filename: covalent-transactions-api-openapi.yml
  format: yaml
  label: Covalent Transactions API
  slug: covalent-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-transactions-api-openapi.yml
- filename: covalent-transforms-api-openapi.yml
  format: yaml
  label: Covalent Transforms API
  slug: covalent-transforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/openapi/covalent-transforms-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: covalenthq.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: goldrush.dev
  spf: true
hosts:
- cert_expires: Sep  4 08:32:44 2026 GMT
  host: www.covalenthq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 02:11:03 2026 GMT
  host: goldrush.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 14:55:08 2026 GMT
  host: api.covalenthq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Covalent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Covalent, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Covalent
provider_slug: covalent
slug: covalent-domain-security
source_filename: covalent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.covalenthq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 08:32:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: goldrush.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 02:11:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.covalenthq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 14:55:08 2026 GMT\n  hsts: null\ndomains:\n- domain: covalenthq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: goldrush.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/covalent/refs/heads/main/security/covalent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Web3
- Multi-Chain
- Data Infrastructure
- Crypto
- DeFi
- NFT
- Hyperliquid
- GoldRush
- AI Agents
---
