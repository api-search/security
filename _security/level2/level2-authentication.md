---
api_key_in:
- query
api_specs:
- filename: level2-strategy-builder-openapi.yml
  format: yaml
  label: Level2 Strategy Builder API
  slug: strategy-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/openapi/level2-strategy-builder-openapi.yml
- filename: level2-tradestation-integration-openapi.yml
  format: yaml
  label: Level2 TradeStation Integration API
  slug: tradestation-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/openapi/level2-tradestation-integration-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Level2 Authentication
name_suffix: Authentication
oauth_flows: []
overview: level2 secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: level2
provider_slug: level2
scheme_count: 2
schemes:
- description: API key passed as a path parameter in the URL. Obtain your API key from the Level2 platform dashboard.
  in: query
  name: apiKeyPath
  parameter: api_key
  sources:
  - openapi/level2-strategy-builder-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: Bearer token authentication for broker API access. Tokens are issued to broker partners during the integration onboarding process.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/level2-tradestation-integration-openapi.yml
  type: http
slug: level2-authentication
source_filename: level2-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/level2-strategy-builder-openapi.yml, openapi/level2-tradestation-integration-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyPath\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key passed as a path parameter in the URL. Obtain your API key from the Level2\n    platform dashboard.\n  sources:\n  - openapi/level2-strategy-builder-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token authentication for broker API access. Tokens are issued to broker\n    partners during the integration onboarding process.\n  sources:\n  - openapi/level2-tradestation-integration-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/authentication/level2-authentication.yml
summary_line: apiKey/http · 2 schemes
tags: []
---
