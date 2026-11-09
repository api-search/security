---
anonymous_access: false
api_key_in: []
api_specs:
- filename: arbitron-app-account-api-openapi.yml
  format: yaml
  label: Arbitron Account API
  slug: arbitron-app-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arbitron-app/openapi/arbitron-app-account-api-openapi.yml
- filename: arbitron-app-funding-api-openapi.yml
  format: yaml
  label: Arbitron Funding API
  slug: arbitron-app-funding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arbitron-app/openapi/arbitron-app-funding-api-openapi.yml
- filename: arbitron-app-platform-api-openapi.yml
  format: yaml
  label: Arbitron Platform API
  slug: arbitron-app-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arbitron-app/openapi/arbitron-app-platform-api-openapi.yml
- filename: arbitron-app-reference-data-api-openapi.yml
  format: yaml
  label: Arbitron Reference data API
  slug: arbitron-app-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arbitron-app/openapi/arbitron-app-reference-data-api-openapi.yml
- filename: arbitron-app-spreads-api-openapi.yml
  format: yaml
  label: Arbitron Spreads API
  slug: arbitron-app-spreads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arbitron-app/openapi/arbitron-app-spreads-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Arbitron App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arbitron declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Arbitron
provider_slug: arbitron-app
scheme_count: 2
schemes:
- description: Agent API keys passed as Bearer token with prefix ar_agent_
  name: Authorization
  scheme: bearer
  type: http
- description: Agent API keys passed via X-Api-Key header with prefix ar_agent_
  in: header
  name: X-Api-Key
  type: apiKey
slug: arbitron-app-authentication
source_filename: arbitron-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://arbitron.app/developers#authentication\nschemes:\n  - type: http\n    scheme: bearer\n    name: Authorization\n    description: Agent API keys passed as Bearer token with prefix ar_agent_\n  - type: apiKey\n    in: header\n    name: X-Api-Key\n    description: Agent API keys passed via X-Api-Key header with prefix ar_agent_\n"
source_yaml_url: https://artifacts.apis.io/arbitron-app/authentication/arbitron-app-authentication.yml
summary_line: 2 schemes
tags:
- Cryptocurrency
- Arbitrage
- Finance
- Platform
---
