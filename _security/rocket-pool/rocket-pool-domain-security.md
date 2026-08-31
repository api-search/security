---
api_specs:
- filename: rocket-pool-auction-api-openapi.yml
  format: yaml
  label: Rocket Pool Auction API
  slug: rocket-pool-auction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-pool/refs/heads/main/openapi/rocket-pool-auction-api-openapi.yml
- filename: rocket-pool-deposit-api-openapi.yml
  format: yaml
  label: Rocket Pool Deposit API
  slug: rocket-pool-deposit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-pool/refs/heads/main/openapi/rocket-pool-deposit-api-openapi.yml
- filename: rocket-pool-megapool-api-openapi.yml
  format: yaml
  label: Rocket Pool Megapool API
  slug: rocket-pool-megapool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-pool/refs/heads/main/openapi/rocket-pool-megapool-api-openapi.yml
- filename: rocket-pool-minipool-api-openapi.yml
  format: yaml
  label: Rocket Pool Minipool API
  slug: rocket-pool-minipool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-pool/refs/heads/main/openapi/rocket-pool-minipool-api-openapi.yml
- filename: rocket-pool-network-api-openapi.yml
  format: yaml
  label: Rocket Pool Network API
  slug: rocket-pool-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-pool/refs/heads/main/openapi/rocket-pool-network-api-openapi.yml
- filename: rocket-pool-node-api-openapi.yml
  format: yaml
  label: Rocket Pool Node API
  slug: rocket-pool-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-pool/refs/heads/main/openapi/rocket-pool-node-api-openapi.yml
- filename: rocket-pool-oracledao-api-openapi.yml
  format: yaml
  label: Rocket Pool OracleDAO API
  slug: rocket-pool-oracledao-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-pool/refs/heads/main/openapi/rocket-pool-oracledao-api-openapi.yml
- filename: rocket-pool-protocoldao-api-openapi.yml
  format: yaml
  label: Rocket Pool ProtocolDAO API
  slug: rocket-pool-protocoldao-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-pool/refs/heads/main/openapi/rocket-pool-protocoldao-api-openapi.yml
- filename: rocket-pool-queue-api-openapi.yml
  format: yaml
  label: Rocket Pool Queue API
  slug: rocket-pool-queue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-pool/refs/heads/main/openapi/rocket-pool-queue-api-openapi.yml
- filename: rocket-pool-rewards-api-openapi.yml
  format: yaml
  label: Rocket Pool Rewards API
  slug: rocket-pool-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-pool/refs/heads/main/openapi/rocket-pool-rewards-api-openapi.yml
- filename: rocket-pool-service-api-openapi.yml
  format: yaml
  label: Rocket Pool Service API
  slug: rocket-pool-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-pool/refs/heads/main/openapi/rocket-pool-service-api-openapi.yml
- filename: rocket-pool-settings-api-openapi.yml
  format: yaml
  label: Rocket Pool Settings API
  slug: rocket-pool-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-pool/refs/heads/main/openapi/rocket-pool-settings-api-openapi.yml
- filename: rocket-pool-tokens-api-openapi.yml
  format: yaml
  label: Rocket Pool Tokens API
  slug: rocket-pool-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-pool/refs/heads/main/openapi/rocket-pool-tokens-api-openapi.yml
- filename: rocket-pool-wallet-api-openapi.yml
  format: yaml
  label: Rocket Pool Wallet API
  slug: rocket-pool-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-pool/refs/heads/main/openapi/rocket-pool-wallet-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: rocketpool.net
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: rocketpool.example
  spf: false
hosts:
- cert_expires: Sep 20 08:41:01 2026 GMT
  host: rocketpool.net
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- host: protocol.rocketpool.example
  https: false
kind: domain-security
layout: security
method: probed
name: Rocket Pool Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rocket Pool, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Rocket Pool
provider_slug: rocket-pool
slug: rocket-pool-domain-security
source_filename: rocket-pool-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rocketpool.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 08:41:01 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: protocol.rocketpool.example\n  https: false\ndomains:\n- domain: rocketpool.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rocketpool.example\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rocket-pool/refs/heads/main/security/rocket-pool-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Ethereum
- Liquid Staking
- Proof of Stake
- DeFi
- Smart Contracts
- Node Operators
- Validator
- rETH
- RPL
- Minipool
- Decentralized Finance
- Decentralized Governance
- DAO
- Web3
---
