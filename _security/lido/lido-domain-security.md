---
api_specs:
- filename: lido-apr-for-eth-and-steth-api-openapi.yml
  format: yaml
  label: Lido APR for Eth and stEth API
  slug: lido-apr-for-eth-and-steth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lido/refs/heads/main/openapi/lido-apr-for-eth-and-steth-api-openapi.yml
- filename: lido-estimate-api-openapi.yml
  format: yaml
  label: Lido Estimate API
  slug: lido-estimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lido/refs/heads/main/openapi/lido-estimate-api-openapi.yml
- filename: lido-nft-api-openapi.yml
  format: yaml
  label: Lido NFT API
  slug: lido-nft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lido/refs/heads/main/openapi/lido-nft-api-openapi.yml
- filename: lido-request-time-api-openapi.yml
  format: yaml
  label: Lido Request Time API
  slug: lido-request-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lido/refs/heads/main/openapi/lido-request-time-api-openapi.yml
- filename: lido-rewards-api-openapi.yml
  format: yaml
  label: Lido Rewards API
  slug: lido-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lido/refs/heads/main/openapi/lido-rewards-api-openapi.yml
- filename: lido-swap-rate-for-steth-and-wsteth-api-openapi.yml
  format: yaml
  label: Lido Swap rate for stETH and wstETH API
  slug: lido-swap-rate-for-steth-and-wsteth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lido/refs/heads/main/openapi/lido-swap-rate-for-steth-and-wsteth-api-openapi.yml
- filename: lido-validators-api-openapi.yml
  format: yaml
  label: Lido Validators API
  slug: lido-validators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lido/refs/heads/main/openapi/lido-validators-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lido.fi
  spf: true
hosts:
- cert_expires: Aug 20 16:14:58 2026 GMT
  host: lido.fi
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 08:11:18 2026 GMT
  host: docs.lido.fi
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Lido Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lido, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lido
provider_slug: lido
slug: lido-domain-security
source_filename: lido-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lido.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 16:14:58 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.lido.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 08:11:18 2026 GMT\n  hsts: false\ndomains:\n- domain: lido.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lido/refs/heads/main/security/lido-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Liquid Staking
- Ethereum
- Staking
- DeFi
- stETH
- wstETH
- Validator
- Node Operators
- DAO
- Governance
- LDO
- Oracle
- Open Source
- Web3
- Smart Contracts
- Distributed Validator Technology
- Community Staking Module
---
