---
api_key_in:
- cookie
- header
api_specs:
- filename: euler-accounts-api-openapi.yml
  format: yaml
  label: Euler Finance Accounts API
  slug: euler-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/openapi/euler-accounts-api-openapi.yml
- filename: euler-apys-api-openapi.yml
  format: yaml
  label: Euler Finance APYs API
  slug: euler-apys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/openapi/euler-apys-api-openapi.yml
- filename: euler-auth-api-openapi.yml
  format: yaml
  label: Euler Finance Auth API
  slug: euler-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/openapi/euler-auth-api-openapi.yml
- filename: euler-chains-api-openapi.yml
  format: yaml
  label: Euler Finance Chains API
  slug: euler-chains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/openapi/euler-chains-api-openapi.yml
- filename: euler-curator-api-openapi.yml
  format: yaml
  label: Euler Finance Curator API
  slug: euler-curator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/openapi/euler-curator-api-openapi.yml
- filename: euler-earn-api-openapi.yml
  format: yaml
  label: Euler Finance Earn API
  slug: euler-earn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/openapi/euler-earn-api-openapi.yml
- filename: euler-entities-api-openapi.yml
  format: yaml
  label: Euler Finance Entities API
  slug: euler-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/openapi/euler-entities-api-openapi.yml
- filename: euler-evc-api-openapi.yml
  format: yaml
  label: Euler Finance EVC API
  slug: euler-evc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/openapi/euler-evc-api-openapi.yml
- filename: euler-feeflow-api-openapi.yml
  format: yaml
  label: Euler Finance FeeFlow API
  slug: euler-feeflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/openapi/euler-feeflow-api-openapi.yml
- filename: euler-graphql-api-openapi.yml
  format: yaml
  label: Euler Finance GraphQL API
  slug: euler-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/openapi/euler-graphql-api-openapi.yml
- filename: euler-health-api-openapi.yml
  format: yaml
  label: Euler Finance Health API
  slug: euler-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/openapi/euler-health-api-openapi.yml
- filename: euler-liquidations-api-openapi.yml
  format: yaml
  label: Euler Finance Liquidations API
  slug: euler-liquidations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/openapi/euler-liquidations-api-openapi.yml
- filename: euler-oracles-api-openapi.yml
  format: yaml
  label: Euler Finance Oracles API
  slug: euler-oracles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/openapi/euler-oracles-api-openapi.yml
- filename: euler-prices-api-openapi.yml
  format: yaml
  label: Euler Finance Prices API
  slug: euler-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/openapi/euler-prices-api-openapi.yml
- filename: euler-protocol-api-openapi.yml
  format: yaml
  label: Euler Finance Protocol API
  slug: euler-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/openapi/euler-protocol-api-openapi.yml
- filename: euler-publicallocator-api-openapi.yml
  format: yaml
  label: Euler Finance PublicAllocator API
  slug: euler-publicallocator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/openapi/euler-publicallocator-api-openapi.yml
- filename: euler-rewards-api-openapi.yml
  format: yaml
  label: Euler Finance Rewards API
  slug: euler-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/openapi/euler-rewards-api-openapi.yml
- filename: euler-termsofuse-api-openapi.yml
  format: yaml
  label: Euler Finance TermsOfUse API
  slug: euler-termsofuse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/openapi/euler-termsofuse-api-openapi.yml
- filename: euler-tokens-api-openapi.yml
  format: yaml
  label: Euler Finance Tokens API
  slug: euler-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/openapi/euler-tokens-api-openapi.yml
- filename: euler-usage-api-openapi.yml
  format: yaml
  label: Euler Finance Usage API
  slug: euler-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/openapi/euler-usage-api-openapi.yml
- filename: euler-vaults-api-openapi.yml
  format: yaml
  label: Euler Finance Vaults API
  slug: euler-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/openapi/euler-vaults-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Euler Authentication
name_suffix: Authentication
oauth_flows: []
overview: Euler Finance secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Euler Finance
provider_slug: euler
scheme_count: 5
schemes:
- description: API key authentication (optional; higher rate limits).
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/euler-v3-data-api.json
  type: apiKey
- bearerFormat: API key
  description: 'Alternative to X-API-Key using Authorization: Bearer <key>'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/euler-v3-data-api.json
  type: http
- description: Admin secret (server-to-server) for API key management.
  in: header
  name: AdminSecret
  parameter: X-Admin-Secret
  sources:
  - openapi/euler-v3-data-api.json
  type: apiKey
- description: Signed, httpOnly platform-operator browser session cookie.
  in: cookie
  name: PlatformSession
  parameter: euler_platform_session
  sources:
  - openapi/euler-v3-data-api.json
  type: apiKey
- description: Double-submit CSRF token required for unsafe cookie-authenticated methods.
  in: header
  name: PlatformCsrf
  parameter: X-CSRF-Token
  sources:
  - openapi/euler-v3-data-api.json
  type: apiKey
slug: euler-authentication
source_filename: euler-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/euler-v3-data-api.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key authentication (optional; higher rate limits).\n  sources:\n  - openapi/euler-v3-data-api.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  description: 'Alternative to X-API-Key using Authorization: Bearer <key>'\n  sources:\n  - openapi/euler-v3-data-api.json\n- name: AdminSecret\n  type: apiKey\n  in: header\n  parameter: X-Admin-Secret\n  description: Admin secret (server-to-server) for API key management.\n  sources:\n  - openapi/euler-v3-data-api.json\n- name: PlatformSession\n  type: apiKey\n  in: cookie\n  parameter: euler_platform_session\n  description: Signed, httpOnly platform-operator browser session cookie.\n  sources:\n  - openapi/euler-v3-data-api.json\n- name:\
  \ PlatformCsrf\n  type: apiKey\n  in: header\n  parameter: X-CSRF-Token\n  description: Double-submit CSRF token required for unsafe cookie-authenticated methods.\n  sources:\n  - openapi/euler-v3-data-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/euler/refs/heads/main/authentication/euler-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- DeFi
- Lending
- Borrowing
- Finance
- Ethereum
- Blockchain
- Vaults
- Liquidation
- Interest Rates
- Permissionless
---
