---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eliza-openapi.yaml
  format: yaml
  label: Eliza AI Framework API
  slug: eliza-ai-framework-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/symbaiex-com/openapi/eliza-openapi.yaml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Symbaiex Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: symbaiex-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: symbaiex-com
provider_slug: symbaiex-com
scheme_count: 2
schemes:
- description: Owner-approved Ed25519 challenge-response authentication.
  type: ed25519
- description: 'WorkOS Connect OAuth flow with resource https://www.symbaiex.com/api/agent/mcp. Scopes: evidence.'
  type: oauth2
slug: symbaiex-com-authentication
source_filename: symbaiex-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://www.symbaiex.com/auth.md\nschemes:\n  - type: \"ed25519\"\n    description: \"Owner-approved Ed25519 challenge-response authentication.\"\n  - type: \"oauth2\"\n    description: \"WorkOS Connect OAuth flow with resource https://www.symbaiex.com/api/agent/mcp. Scopes: evidence.\"\n"
source_yaml_url: https://artifacts.apis.io/symbaiex-com/authentication/symbaiex-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Research
- OpenAPI
- PublicData
---
