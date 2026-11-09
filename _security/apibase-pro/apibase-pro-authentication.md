---
anonymous_access: false
api_key_in: []
api_specs:
- filename: apibase-pro-tools-api-openapi.yml
  format: yaml
  label: APIbase Tools API
  slug: apibase-pro-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apibase-pro/openapi/apibase-pro-tools-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Apibase Pro Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIbase declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: APIbase
provider_slug: apibase-pro
scheme_count: 1
schemes:
- description: OAuth2 client credentials flow; token is same as API key.
  flow: client_credentials
  tokenUrl: https://apibase.pro/.well-known/oauth-token
  type: oauth2
slug: apibase-pro-authentication
source_filename: apibase-pro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://apibase.pro/auth.md\nschemes:\n  - type: oauth2\n    flow: client_credentials\n    tokenUrl: https://apibase.pro/.well-known/oauth-token\n    description: OAuth2 client credentials flow; token is same as API key.\n"
source_yaml_url: https://artifacts.apis.io/apibase-pro/authentication/apibase-pro-authentication.yml
summary_line: 1 scheme
tags:
- Gateways
- Artificial Intelligence
- MCP
- Payments
---
