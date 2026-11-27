---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: codebase-design-account-api-openapi.yml
  format: yaml
  label: Codebase Account API
  slug: codebase-design-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-account-api-openapi.yml
- filename: codebase-design-admin-api-openapi.yml
  format: yaml
  label: Codebase Admin API
  slug: codebase-design-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-admin-api-openapi.yml
- filename: codebase-design-api-keys-api-openapi.yml
  format: yaml
  label: Codebase API Keys API
  slug: codebase-design-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-api-keys-api-openapi.yml
- filename: codebase-design-billing-api-openapi.yml
  format: yaml
  label: Codebase Billing API
  slug: codebase-design-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-billing-api-openapi.yml
- filename: codebase-design-builds-api-openapi.yml
  format: yaml
  label: Codebase Builds API
  slug: codebase-design-builds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-builds-api-openapi.yml
- filename: codebase-design-community-api-openapi.yml
  format: yaml
  label: Codebase Community API
  slug: codebase-design-community-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-community-api-openapi.yml
- filename: codebase-design-credits-api-openapi.yml
  format: yaml
  label: Codebase Credits API
  slug: codebase-design-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-credits-api-openapi.yml
- filename: codebase-design-deploys-api-openapi.yml
  format: yaml
  label: Codebase Deploys API
  slug: codebase-design-deploys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-deploys-api-openapi.yml
- filename: codebase-design-gallery-api-openapi.yml
  format: yaml
  label: Codebase Gallery API
  slug: codebase-design-gallery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-gallery-api-openapi.yml
- filename: codebase-design-health-api-openapi.yml
  format: yaml
  label: Codebase Health API
  slug: codebase-design-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-health-api-openapi.yml
- filename: codebase-design-inference-api-openapi.yml
  format: yaml
  label: Codebase Inference API
  slug: codebase-design-inference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-inference-api-openapi.yml
- filename: codebase-design-platform-api-openapi.yml
  format: yaml
  label: Codebase Platform API
  slug: codebase-design-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-platform-api-openapi.yml
- filename: codebase-design-projects-api-openapi.yml
  format: yaml
  label: Codebase Projects API
  slug: codebase-design-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-projects-api-openapi.yml
- filename: codebase-design-prompts-api-openapi.yml
  format: yaml
  label: Codebase Prompts API
  slug: codebase-design-prompts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-prompts-api-openapi.yml
- filename: codebase-design-sessions-api-openapi.yml
  format: yaml
  label: Codebase Sessions API
  slug: codebase-design-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebase-design/openapi/codebase-design-sessions-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Codebase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Codebase secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Codebase
provider_slug: codebase-design
scheme_count: 2
schemes:
- description: Revocable API key (cb_live_... or cb_test_...). Created, scoped, given an expiry and an optional credit spending limit, rotated and revoked in Settings -> API keys; shown once.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/codebase-design-openapi.yml
  - https://codebase.design/agents
  type: apiKey
- bearerFormat: JWT
  description: 'OAuth2 access token. Docs: "OAuth supports browser-based account authorization and device-code login for terminal-style clients"; the CLI uses browser OAuth with PKCE; MCP connectors (claude.ai, ChatGPT) use OAuth with PKCE and dynamic client registration. The same API key is also accepted as a Bearer token on the MCP endpoint.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/codebase-design-openapi.yml
  - https://codebase.design/docs/api
  - https://codebase.design/llms.txt
  type: http
slug: codebase-design-authentication
source_filename: codebase-design-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://codebase.design/docs/api\ndocs: https://codebase.design/docs/api\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Revocable API key (cb_live_... or cb_test_...). Created, scoped, given an expiry and an optional\n    credit spending limit, rotated and revoked in Settings -> API keys; shown once.\n  sources:\n  - openapi/codebase-design-openapi.yml\n  - https://codebase.design/agents\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'OAuth2 access token. Docs: \"OAuth supports browser-based account authorization and device-code login\n    for terminal-style clients\"; the CLI uses browser OAuth with PKCE; MCP connectors (claude.ai, ChatGPT) use OAuth\n    with PKCE and dynamic client registration. The same API key is also accepted as a Bearer token on the MCP endpoint.'\n\
  \  sources:\n  - openapi/codebase-design-openapi.yml\n  - https://codebase.design/docs/api\n  - https://codebase.design/llms.txt\nunauthenticated_payment:\n  description: POST /api/v1/builds without credentials answers 402 with a PAYMENT-REQUIRED header (x402 v2, USDC\n    on Base mainnet); paying it returns x402.apiKey for a wallet-keyed account.\n  source: https://codebase.design/llms.txt\nkey_check: GET /api/v1/whoami confirms the key and its scopes (documented on /agents; not called by this pipeline).\nrelated_docs:\n- https://codebase.design/agents\n- https://codebase.design/llms.txt\n"
source_yaml_url: https://artifacts.apis.io/codebase-design/authentication/codebase-design-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- AI App Builder
- Code Generation
- Developer Tools
- Open-Weight Models
- CLI
- MCP
- Web3
---
