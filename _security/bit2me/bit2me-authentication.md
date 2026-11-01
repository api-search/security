---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bit2me-account-api-openapi.yml
  format: yaml
  label: Bit2Me Account API
  slug: bit2me-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bit2me/openapi/bit2me-account-api-openapi.yml
- filename: bit2me-account-deprecated-methods-api-openapi.yml
  format: yaml
  label: Bit2Me Account Deprecated Methods API
  slug: bit2me-account-deprecated-methods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bit2me/openapi/bit2me-account-deprecated-methods-api-openapi.yml
- filename: bit2me-auth-api-openapi.yml
  format: yaml
  label: Bit2Me Auth API
  slug: bit2me-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bit2me/openapi/bit2me-auth-api-openapi.yml
- filename: bit2me-blockchain-manager-api-openapi.yml
  format: yaml
  label: Bit2Me Blockchain Manager API
  slug: bit2me-blockchain-manager-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bit2me/openapi/bit2me-blockchain-manager-api-openapi.yml
- filename: bit2me-brokerage-api-openapi.yml
  format: yaml
  label: Bit2Me Brokerage API
  slug: bit2me-brokerage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bit2me/openapi/bit2me-brokerage-api-openapi.yml
- filename: bit2me-compliance-api-openapi.yml
  format: yaml
  label: Bit2Me Compliance API
  slug: bit2me-compliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bit2me/openapi/bit2me-compliance-api-openapi.yml
- filename: bit2me-currency-api-openapi.yml
  format: yaml
  label: Bit2Me Currency API
  slug: bit2me-currency-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bit2me/openapi/bit2me-currency-api-openapi.yml
- filename: bit2me-earn-api-openapi.yml
  format: yaml
  label: Bit2Me Earn API
  slug: bit2me-earn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bit2me/openapi/bit2me-earn-api-openapi.yml
- filename: bit2me-loan-api-openapi.yml
  format: yaml
  label: Bit2Me Loan API
  slug: bit2me-loan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bit2me/openapi/bit2me-loan-api-openapi.yml
- filename: bit2me-misc-api-openapi.yml
  format: yaml
  label: Bit2Me Misc API
  slug: bit2me-misc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bit2me/openapi/bit2me-misc-api-openapi.yml
- filename: bit2me-pay-api-openapi.yml
  format: yaml
  label: Bit2Me Pay API
  slug: bit2me-pay-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bit2me/openapi/bit2me-pay-api-openapi.yml
- filename: bit2me-teller-api-openapi.yml
  format: yaml
  label: Bit2Me Teller API
  slug: bit2me-teller-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bit2me/openapi/bit2me-teller-api-openapi.yml
- filename: bit2me-trading-api-openapi.yml
  format: yaml
  label: Bit2Me Trading API
  slug: bit2me-trading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bit2me/openapi/bit2me-trading-api-openapi.yml
- filename: bit2me-verifier-api-openapi.yml
  format: yaml
  label: Bit2Me Verifier API
  slug: bit2me-verifier-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bit2me/openapi/bit2me-verifier-api-openapi.yml
- filename: bit2me-verifier-deprecated-methods-api-openapi.yml
  format: yaml
  label: Bit2Me Verifier Deprecated Methods API
  slug: bit2me-verifier-deprecated-methods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bit2me/openapi/bit2me-verifier-deprecated-methods-api-openapi.yml
- filename: bit2me-wallet-api-openapi.yml
  format: yaml
  label: Bit2Me Wallet API
  slug: bit2me-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bit2me/openapi/bit2me-wallet-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Bit2Me Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bit2Me declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Bit2Me
provider_slug: bit2me
scheme_count: 5
schemes:
- description: Public API key
  in: header
  name: X-Api-Key
  type: apiKey
- description: Basic auth with base64 username:password
  in: header
  name: Authorization
  type: apiKey
- description: Custom API key for specific endpoints
  in: header
  name: Authorization
  type: apiKey
- description: JWT token (Bearer)
  in: header
  name: Authorization
  type: apiKey
- description: Pre-auth token (Bearer) for two-step verification
  in: header
  name: Authorization
  type: apiKey
slug: bit2me-authentication
source_filename: bit2me-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: derived\nsource: openapi/bit2me-openapi.json\nschemes:\n  - type: apiKey\n    name: X-Api-Key\n    in: header\n    description: \"Public API key\"\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Basic auth with base64 username:password\"\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Custom API key for specific endpoints\"\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"JWT token (Bearer)\"\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Pre-auth token (Bearer) for two-step verification\"\n"
source_yaml_url: https://artifacts.apis.io/bit2me/authentication/bit2me-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Cryptocurrency
- Fintech
- Exchange
- Payments
- API
---
