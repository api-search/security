---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Adwhiz Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: adwhiz-ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: adwhiz-ai
provider_slug: adwhiz-ai
scheme_count: 2
schemes:
- description: 'Bearer API key for MCP API calls. Format: ''Bearer {api_key}''.'
  in: header
  name: Authorization
  type: apiKey
- description: OAuth 2.0 with PKCE for MCP connections. Uses Authorization Code flow with short-lived access tokens.
  flow: authorizationCode
  pkce: true
  type: oauth2
slug: adwhiz-ai-authentication
source_filename: adwhiz-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://www.adwhiz.ai/docs/security\nschemes:\n  - type: \"apiKey\"\n    name: \"Authorization\"\n    in: \"header\"\n    description: \"Bearer API key for MCP API calls. Format: 'Bearer {api_key}'.\"\n  - type: \"oauth2\"\n    flow: \"authorizationCode\"\n    pkce: true\n    description: \"OAuth 2.0 with PKCE for MCP connections. Uses Authorization Code flow with short-lived access tokens.\"\n"
source_yaml_url: https://artifacts.apis.io/adwhiz-ai/authentication/adwhiz-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Advertising
- Google Ads
- Meta Ads
- Marketing
---
