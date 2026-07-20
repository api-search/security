---
api_key_in: []
api_specs:
- filename: alpic-openapi-original.json
  format: json
  label: Alpic API
  slug: alpic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/openapi/alpic-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Alpic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alpic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Alpic
provider_slug: alpic
scheme_count: 1
schemes:
- description: Bearer token for authentication. Use an API key from the API Keys page in team settings, or an OAuth access token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/alpic-openapi-original.json
  type: http
slug: alpic-authentication
source_filename: alpic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/alpic-openapi-original.json\ndocs: https://docs.alpic.ai/api-reference\nagentic_auth:\n  register_uri: https://api.alpic.ai/agent/auth\n  skill: https://alpic.ai/auth.md\n  assertion_type: urn:ietf:params:oauth:token-type:id-jag\n  credential_type: api_key\n  notes: Agents can self-register for a non-expiring API key via identity assertion (ID-JAG); see /.well-known/oauth-authorization-server agent_auth block.\noidc:\n  authorization_servers:\n    - https://cognito-idp.us-east-1.amazonaws.com/us-east-1_GWVpeD5h1\n    - https://api.alpic.ai/\n  scopes_supported: [openid, email, profile]\n  source: well-known/alpic-oauth-protected-resource.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token for authentication. Use an API key from the API Keys page in team\n    settings, or an OAuth access token.\n  sources:\n  - openapi/alpic-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/authentication/alpic-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai/Ml
- MCP
- Model Context Protocol
- Cloud Platform
- Developer Tools
- Deployment
- ChatGPT Apps
- Agentic
---
