---
api_key_in:
- header
api_specs:
- filename: gauntlet-openapi-original.json
  format: json
  label: Gauntlet API
  slug: gauntlet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gauntlet/refs/heads/main/openapi/gauntlet-openapi-original.json
auth_types:
- http
description: The Gauntlet REST API (api.gauntlet.xyz) authenticates every request with a partner-provisioned API key passed as an HTTP Bearer token. The published OpenAPI does not declare securitySchemes, so this profile is captured from the docs Auth & Credentials page; 401 responses are documented across the spec.
kind: authentication
layout: security
method: searched
name: Gauntlet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gauntlet secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gauntlet
provider_slug: gauntlet
scheme_count: 1
schemes:
- description: Partner-provisioned API key. After partner approval Gauntlet provisions an API key for your organization. Keys are server-side only — never expose in client-side code, public repos, or version control. Docs recommend separate keys for development, staging, and production, and rotating production credentials every 90 days.
  format: 'Authorization: Bearer <API_KEY>'
  header: Authorization
  name: bearerAuth
  provisioning: Partner approval, then Gauntlet provisions a key (docs.gauntlet.xyz/onboarding/sign-up)
  scheme: bearer
  sources:
  - https://docs.gauntlet.xyz/onboarding/credentials
  test_live_separation: none-documented
  type: http
slug: gauntlet-authentication
source_filename: gauntlet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.gauntlet.xyz/onboarding/credentials\ndescription: >-\n  The Gauntlet REST API (api.gauntlet.xyz) authenticates every request with a\n  partner-provisioned API key passed as an HTTP Bearer token. The published\n  OpenAPI does not declare securitySchemes, so this profile is captured from the\n  docs Auth & Credentials page; 401 responses are documented across the spec.\ndocs: https://docs.gauntlet.xyz/onboarding/credentials\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    header: Authorization\n    format: \"Authorization: Bearer <API_KEY>\"\n    description: >-\n      Partner-provisioned API key. After partner approval Gauntlet provisions an\n      API key for your organization. Keys are server-side only — never expose in\n      client-side code, public repos, or version control. Docs recommend separate\n      keys\
  \ for development, staging, and production, and rotating production\n      credentials every 90 days.\n    provisioning: Partner approval, then Gauntlet provisions a key (docs.gauntlet.xyz/onboarding/sign-up)\n    test_live_separation: none-documented\n    sources: [https://docs.gauntlet.xyz/onboarding/credentials]\nnotes: >-\n  On-chain deposit/withdraw flows via @gauntlet-xyz/sdk are authorized by the user's\n  wallet signature (viem), not the API key; the API key authorizes read access to\n  vault/position/analytics data.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gauntlet/refs/heads/main/authentication/gauntlet-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Crypto Data
- DeFi
- Risk Management
- Yield
- Vaults
- Blockchain
- Web3
- Financial Modeling
---
