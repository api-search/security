---
api_specs:
- filename: lido-finance-apr-for-eth-and-steth-api-openapi.yml
  format: yaml
  label: Lido Finance APR for Eth and stEth API
  slug: lido-finance-apr-for-eth-and-steth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lido-finance/refs/heads/main/openapi/lido-finance-apr-for-eth-and-steth-api-openapi.yml
- filename: lido-finance-estimate-api-openapi.yml
  format: yaml
  label: Lido Finance Estimate API
  slug: lido-finance-estimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lido-finance/refs/heads/main/openapi/lido-finance-estimate-api-openapi.yml
- filename: lido-finance-nft-api-openapi.yml
  format: yaml
  label: Lido Finance NFT API
  slug: lido-finance-nft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lido-finance/refs/heads/main/openapi/lido-finance-nft-api-openapi.yml
- filename: lido-finance-request-time-api-openapi.yml
  format: yaml
  label: Lido Finance Request Time API
  slug: lido-finance-request-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lido-finance/refs/heads/main/openapi/lido-finance-request-time-api-openapi.yml
- filename: lido-finance-rewards-api-openapi.yml
  format: yaml
  label: Lido Finance Rewards API
  slug: lido-finance-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lido-finance/refs/heads/main/openapi/lido-finance-rewards-api-openapi.yml
- filename: lido-finance-swap-rate-for-steth-and-wsteth-api-openapi.yml
  format: yaml
  label: Lido Finance Swap rate for stETH and wstETH API
  slug: lido-finance-swap-rate-for-steth-and-wsteth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lido-finance/refs/heads/main/openapi/lido-finance-swap-rate-for-steth-and-wsteth-api-openapi.yml
- filename: lido-finance-validators-api-openapi.yml
  format: yaml
  label: Lido Finance Validators API
  slug: lido-finance-validators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lido-finance/refs/heads/main/openapi/lido-finance-validators-api-openapi.yml
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
- cert_expires: Aug 20 16:14:58 2026 GMT
  host: eth-api.lido.fi
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lido Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lido Finance, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lido Finance
provider_slug: lido-finance
slug: lido-finance-domain-security
source_filename: lido-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lido.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 16:14:58 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.lido.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 08:11:18 2026 GMT\n  hsts: false\n- host: eth-api.lido.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 16:14:58 2026 GMT\n  hsts: null\ndomains:\n- domain: lido.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lido-finance/refs/heads/main/security/lido-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Blockchain
- Ethereum
- Liquid Staking
- DeFi
- Cryptocurrency
- Staking
- Web3
- Financial-Services
- GraphQL
---
