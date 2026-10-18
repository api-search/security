---
api_specs:
- filename: reservoir-accounts-api-openapi.yml
  format: yaml
  label: Reservoir Accounts API
  slug: reservoir-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-accounts-api-openapi.yml
- filename: reservoir-activity-api-openapi.yml
  format: yaml
  label: Reservoir Activity API
  slug: reservoir-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-activity-api-openapi.yml
- filename: reservoir-attributes-api-openapi.yml
  format: yaml
  label: Reservoir Attributes API
  slug: reservoir-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-attributes-api-openapi.yml
- filename: reservoir-chain-api-openapi.yml
  format: yaml
  label: Reservoir Chain API
  slug: reservoir-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-chain-api-openapi.yml
- filename: reservoir-collections-api-openapi.yml
  format: yaml
  label: Reservoir Collections API
  slug: reservoir-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-collections-api-openapi.yml
- filename: reservoir-events-api-openapi.yml
  format: yaml
  label: Reservoir Events API
  slug: reservoir-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-events-api-openapi.yml
- filename: reservoir-manage-orders-api-openapi.yml
  format: yaml
  label: Reservoir Manage Orders API
  slug: reservoir-manage-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-manage-orders-api-openapi.yml
- filename: reservoir-management-api-openapi.yml
  format: yaml
  label: Reservoir Management API
  slug: reservoir-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-management-api-openapi.yml
- filename: reservoir-marketplace-api-openapi.yml
  format: yaml
  label: Reservoir Marketplace API
  slug: reservoir-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-marketplace-api-openapi.yml
- filename: reservoir-misc-api-openapi.yml
  format: yaml
  label: Reservoir Misc API
  slug: reservoir-misc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-misc-api-openapi.yml
- filename: reservoir-orders-api-openapi.yml
  format: yaml
  label: Reservoir Orders API
  slug: reservoir-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-orders-api-openapi.yml
- filename: reservoir-owners-api-openapi.yml
  format: yaml
  label: Reservoir Owners API
  slug: reservoir-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-owners-api-openapi.yml
- filename: reservoir-redirects-api-openapi.yml
  format: yaml
  label: Reservoir Redirects API
  slug: reservoir-redirects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-redirects-api-openapi.yml
- filename: reservoir-sales-api-openapi.yml
  format: yaml
  label: Reservoir Sales API
  slug: reservoir-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-sales-api-openapi.yml
- filename: reservoir-sources-api-openapi.yml
  format: yaml
  label: Reservoir Sources API
  slug: reservoir-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-sources-api-openapi.yml
- filename: reservoir-stats-api-openapi.yml
  format: yaml
  label: Reservoir Stats API
  slug: reservoir-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-stats-api-openapi.yml
- filename: reservoir-tokens-api-openapi.yml
  format: yaml
  label: Reservoir Tokens API
  slug: reservoir-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-tokens-api-openapi.yml
- filename: reservoir-transfers-api-openapi.yml
  format: yaml
  label: Reservoir Transfers API
  slug: reservoir-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-transfers-api-openapi.yml
- filename: reservoir-x-deprecated-api-openapi.yml
  format: yaml
  label: Reservoir X Deprecated API
  slug: reservoir-x-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-x-deprecated-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: reservoir.dev
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: reservoir.tools
  spf: true
hosts:
- host: reservoir.dev
  https: false
- host: api.reservoir.tools
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Reservoir Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reservoir, probed live across 2 host(s) and 2 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Reservoir
provider_slug: reservoir
slug: reservoir-domain-security
source_filename: reservoir-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reservoir.dev\n  https: false\n- host: api.reservoir.tools\n  https: false\ndomains:\n- domain: reservoir.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: reservoir.tools\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/security/reservoir-domain-security.yml
summary_line: DMARC
tags:
- NFT
- Blockchain
- Marketplace
- Ethereum
- EVM
- Liquidity
- Order Book
- Web3
- DeFi
- Trading
- Data API
---
