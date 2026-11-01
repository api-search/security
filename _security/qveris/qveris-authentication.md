---
anonymous_access: false
api_key_in: []
api_specs:
- filename: qveris-agent-lifecycle-api-openapi.yml
  format: yaml
  label: QVeris Agent Lifecycle API
  slug: qveris-agent-lifecycle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qveris/openapi/qveris-agent-lifecycle-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Qveris Authentication
name_suffix: Authentication
oauth_flows: []
overview: QVeris declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: QVeris
provider_slug: qveris
scheme_count: 2
schemes:
- description: Bearer token passed as 'Bearer <API_KEY>'.
  in: header
  name: Authorization
  type: apiKey
- description: OAuth2 password flow for obtaining access tokens.
  flow: password
  tokenUrl: /api/v1/auth/login
  type: oauth2
slug: qveris-authentication
source_filename: qveris-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://qveris.ai/docs/python-sdk.md\nschemes:\n  - type: \"apiKey\"\n    name: \"Authorization\"\n    in: \"header\"\n    description: \"Bearer token passed as 'Bearer <API_KEY>'.\"\n  - type: \"oauth2\"\n    flow: \"password\"\n    tokenUrl: \"/api/v1/auth/login\"\n    description: \"OAuth2 password flow for obtaining access tokens.\"\n"
source_yaml_url: https://artifacts.apis.io/qveris/authentication/qveris-authentication.yml
summary_line: 2 schemes
tags:
- AI
- Data
- Platform
- DeveloperTools
- MCP
---
