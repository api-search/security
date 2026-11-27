---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cardealscore-com-explain-api-openapi.yml
  format: yaml
  label: DealScore Explain API
  slug: cardealscore-com-explain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cardealscore-com/openapi/cardealscore-com-explain-api-openapi.yml
- filename: cardealscore-com-health-api-openapi.yml
  format: yaml
  label: DealScore Health API
  slug: cardealscore-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cardealscore-com/openapi/cardealscore-com-health-api-openapi.yml
- filename: cardealscore-com-quote-check-api-openapi.yml
  format: yaml
  label: DealScore Quote Check API
  slug: cardealscore-com-quote-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cardealscore-com/openapi/cardealscore-com-quote-check-api-openapi.yml
- filename: cardealscore-com-score-api-openapi.yml
  format: yaml
  label: DealScore Score API
  slug: cardealscore-com-score-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cardealscore-com/openapi/cardealscore-com-score-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: DealScore Authentication
name_suffix: Authentication
oauth_flows: []
overview: DealScore declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DealScore
provider_slug: cardealscore-com
scheme_count: 1
schemes:
- authorizationUrl: https://cardealscore.com/oauth/authorize
  description: OAuth 2.1 with PKCE for agents; API keys also supported.
  flow: authorizationCode
  scopes: {}
  tokenUrl: https://cardealscore.com/oauth/token
  type: oauth2
slug: cardealscore-com-authentication
source_filename: cardealscore-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://cardealscore.com/auth.md\nschemes:\n  - type: oauth2\n    flow: authorizationCode\n    description: OAuth 2.1 with PKCE for agents; API keys also supported.\n    tokenUrl: https://cardealscore.com/oauth/token\n    authorizationUrl: https://cardealscore.com/oauth/authorize\n    scopes: {}\n"
source_yaml_url: https://artifacts.apis.io/cardealscore-com/authentication/cardealscore-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- UsedCar
- Artificial Intelligence
- Pricing
- MCP
---
