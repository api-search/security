---
api_key_in: []
api_specs:
- filename: dynamic-labs-openapi.yml
  format: yaml
  label: Dynamic Users API
  slug: dynamic-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-openapi.yml
- filename: dynamic-labs-openapi.yml
  format: yaml
  label: Dynamic Wallets API
  slug: dynamic-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-openapi.yml
- filename: dynamic-labs-openapi.yml
  format: yaml
  label: Dynamic Embedded Wallets API
  slug: dynamic-embedded-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-openapi.yml
- filename: dynamic-labs-openapi.yml
  format: yaml
  label: Dynamic Environments API
  slug: dynamic-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-openapi.yml
- filename: dynamic-labs-openapi.yml
  format: yaml
  label: Dynamic API Tokens API
  slug: dynamic-api-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-openapi.yml
- filename: dynamic-labs-openapi.yml
  format: yaml
  label: Dynamic Webhooks API
  slug: dynamic-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-openapi.yml
- filename: dynamic-labs-openapi.yml
  format: yaml
  label: Dynamic Token Verification API
  slug: dynamic-token-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-openapi.yml
- filename: dynamic-labs-openapi.yml
  format: yaml
  label: Dynamic Allowlists API
  slug: dynamic-allowlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-openapi.yml
- filename: dynamic-labs-openapi.yml
  format: yaml
  label: Dynamic Analytics API
  slug: dynamic-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dynamic Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dynamic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dynamic
provider_slug: dynamic-labs
scheme_count: 1
schemes:
- bearerFormat: dyn_token
  description: 'Environment-scoped API token with a dyn_ prefix for admin endpoints, or a user JWT from the client SDK for SDK endpoints. Sent as Authorization: Bearer <token>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dynamic-labs-openapi.yml
  type: http
slug: dynamic-labs-authentication
source_filename: dynamic-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dynamic-labs-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: dyn_token\n  description: 'Environment-scoped API token with a dyn_ prefix for admin endpoints, or a user\n    JWT from the client SDK for SDK endpoints. Sent as Authorization: Bearer <token>.'\n  sources:\n  - openapi/dynamic-labs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/authentication/dynamic-labs-authentication.yml
summary_line: http · 1 scheme
tags:
- Web3
- Authentication
- Embedded Wallets
- Wallets
- MPC
- Onboarding
- Crypto
---
