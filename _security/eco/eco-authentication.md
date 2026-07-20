---
api_key_in: []
api_specs:
- filename: eco-routes-openapi-original.json
  format: json
  label: Eco Routes API
  slug: eco-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eco/refs/heads/main/openapi/eco-routes-openapi-original.json
auth_types:
- none
description: 'The Eco Routes REST API (quote and intent endpoints) requires NO authentication. There are no securitySchemes declared in the OpenAPI and no API keys, tokens, or OAuth flows. Callers pass a dAppID identifier in the request body purely for attribution. Authorization instead lives at the onchain layer: solver registration/update uses signed requests, and all value movement is executed via EVM/SVM wallet signatures against non-custodial per-intent CREATE2 vault contracts. There is no account or credential provisioning surface.'
kind: authentication
layout: security
method: searched
name: Eco Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eco secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Eco
provider_slug: eco
scheme_count: 0
schemes: []
slug: eco-authentication
source_filename: eco-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.eco.com/api-reference/introduction\ndocs: https://docs.eco.com/api-reference/introduction\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  model: no-auth-with-attribution\ndescription: >-\n  The Eco Routes REST API (quote and intent endpoints) requires NO authentication.\n  There are no securitySchemes declared in the OpenAPI and no API keys, tokens, or\n  OAuth flows. Callers pass a dAppID identifier in the request body purely for\n  attribution. Authorization instead lives at the onchain layer: solver\n  registration/update uses signed requests, and all value movement is executed via\n  EVM/SVM wallet signatures against non-custodial per-intent CREATE2 vault\n  contracts. There is no account or credential provisioning surface.\nschemes: []\nonchain_authorization:\n  - mechanism: dAppID\n    location: request body\n    purpose: attribution only (not access control)\n  - mechanism: signed solver\
  \ requests\n    purpose: solver registration and quote submission\n  - mechanism: wallet signatures (EVM / SVM)\n    purpose: authorizing intent funding and settlement against vault contracts\n  - mechanism: Permit3 / Permit2\n    purpose: bounded token approvals and gasless intent authorization\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eco/refs/heads/main/authentication/eco-authentication.yml
summary_line: none · 0 schemes
tags:
- Company
- Stablecoin
- Cryptocurrency
- Payments
- Blockchain
- Cross-Chain
- DeFi
- Web3
- Infrastructure
- Financial Services
---
