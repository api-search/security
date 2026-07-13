---
api_specs:
- filename: rocket-pool-smart-node-openapi.yml
  format: yaml
  label: Rocket Pool Smart Node Daemon API
  slug: smart-node-daemon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-pool/refs/heads/main/openapi/rocket-pool-smart-node-openapi.yml
- filename: rocket-pool-protocol-openapi.yml
  format: yaml
  label: Rocket Pool Protocol API (rocketpool-go)
  slug: rocketpool-go-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-pool/refs/heads/main/openapi/rocket-pool-protocol-openapi.yml
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
