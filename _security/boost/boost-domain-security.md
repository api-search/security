---
api_specs:
- filename: boost-action-api-openapi.yml
  format: yaml
  label: Boost Action API
  slug: boost-action-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost/refs/heads/main/openapi/boost-action-api-openapi.yml
- filename: boost-action-template-api-openapi.yml
  format: yaml
  label: Boost Action Template API
  slug: boost-action-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost/refs/heads/main/openapi/boost-action-template-api-openapi.yml
- filename: boost-blocklist-api-openapi.yml
  format: yaml
  label: Boost Blocklist API
  slug: boost-blocklist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost/refs/heads/main/openapi/boost-blocklist-api-openapi.yml
- filename: boost-boost-api-openapi.yml
  format: yaml
  label: Boost Boost API
  slug: boost-boost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost/refs/heads/main/openapi/boost-boost-api-openapi.yml
- filename: boost-budget-api-openapi.yml
  format: yaml
  label: Boost Budget API
  slug: boost-budget-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost/refs/heads/main/openapi/boost-budget-api-openapi.yml
- filename: boost-contract-api-openapi.yml
  format: yaml
  label: Boost Contract API
  slug: boost-contract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost/refs/heads/main/openapi/boost-contract-api-openapi.yml
- filename: boost-rewardkit-api-openapi.yml
  format: yaml
  label: Boost RewardKit API
  slug: boost-rewardkit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost/refs/heads/main/openapi/boost-rewardkit-api-openapi.yml
- filename: boost-rewardkittrending-api-openapi.yml
  format: yaml
  label: Boost RewardKitTrending API
  slug: boost-rewardkittrending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost/refs/heads/main/openapi/boost-rewardkittrending-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: boost.xyz
  spf: true
hosts:
- cert_expires: Sep 27 07:50:56 2026 GMT
  host: boost.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boost, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Boost
provider_slug: boost
slug: boost-domain-security
source_filename: boost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boost.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 07:50:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: boost.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boost/refs/heads/main/security/boost-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Web3
- Incentives
- Rewards
- Blockchain
- DeFi
- Onchain
- EVM
---
