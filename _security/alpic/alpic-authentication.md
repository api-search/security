---
api_key_in: []
api_specs:
- filename: alpic-analytics-api-openapi.yml
  format: yaml
  label: Alpic analytics API
  slug: alpic-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/openapi/alpic-analytics-api-openapi.yml
- filename: alpic-beacon-api-openapi.yml
  format: yaml
  label: Alpic beacon API
  slug: alpic-beacon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/openapi/alpic-beacon-api-openapi.yml
- filename: alpic-deployments-api-openapi.yml
  format: yaml
  label: Alpic deployments API
  slug: alpic-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/openapi/alpic-deployments-api-openapi.yml
- filename: alpic-distribution-api-openapi.yml
  format: yaml
  label: Alpic distribution API
  slug: alpic-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/openapi/alpic-distribution-api-openapi.yml
- filename: alpic-environments-api-openapi.yml
  format: yaml
  label: Alpic environments API
  slug: alpic-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/openapi/alpic-environments-api-openapi.yml
- filename: alpic-projects-api-openapi.yml
  format: yaml
  label: Alpic projects API
  slug: alpic-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/openapi/alpic-projects-api-openapi.yml
- filename: alpic-teams-api-openapi.yml
  format: yaml
  label: Alpic teams API
  slug: alpic-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/openapi/alpic-teams-api-openapi.yml
- filename: alpic-tunnels-api-openapi.yml
  format: yaml
  label: Alpic tunnels API
  slug: alpic-tunnels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/openapi/alpic-tunnels-api-openapi.yml
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
- Ai Ml
- MCP
- Cloud Platform
- Developer Tools
- Deployment
- ChatGPT Apps
- Agentic
---
