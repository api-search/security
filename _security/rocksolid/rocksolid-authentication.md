---
api_key_in: []
api_specs:
- filename: rocksolid-vaults-openapi.yml
  format: yaml
  label: RockSolid Vaults API
  slug: rocksolid-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocksolid/refs/heads/main/openapi/rocksolid-vaults-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Rocksolid Authentication
name_suffix: Authentication
oauth_flows: []
overview: RockSolid declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: RockSolid
provider_slug: rocksolid
scheme_count: 0
schemes: []
slug: rocksolid-authentication
source_filename: rocksolid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.rocksolid.network/integration/api\ndocs: https://docs.rocksolid.network/integration/api\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The RockSolid Vaults API is a public, read-only data API. It declares no\n    authentication scheme (no API key, bearer token, or OAuth) in its published\n    documentation or its live responses. Access is instead restricted at the\n    browser layer by a CORS allow list. State-changing operations (deposit,\n    withdraw/redeem) are performed on-chain against the ERC-7540 vault smart\n    contracts and authenticated by wallet signature, not by this HTTP API.\nschemes: []\ncors_allowed_origins:\n- '*.rocketpool.net'\n- '*.rocksolid.network'\n- 'http://localhost:3000'\n- 'http://localhost:8788'\n- 'http://localhost:8787'\nonchain_auth:\n  model: wallet-signature\n  standard: ERC-7540 / ERC-4626\n  docs: https://docs.rocksolid.network/integration/smart-contracts\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rocksolid/refs/heads/main/authentication/rocksolid-authentication.yml
summary_line: 0 schemes
tags:
- Company
- DeFi
- Decentralized Finance
- Liquid Vaults
- Yield
- Staking
- Web3
- Blockchain
---
