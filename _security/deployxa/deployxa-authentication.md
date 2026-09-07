---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: deployxa-openapi-original.json
  format: json
  label: Deployxa Platform
  slug: deployxa-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deployxa/refs/heads/main/openapi/deployxa-openapi-original.json
auth_types:
- http-bearer
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Deployxa Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Deployxa secures its APIs with http-bearer and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Deployxa
provider_slug: deployxa
scheme_count: 3
schemes:
- description: 'API key from the dashboard sent as "Authorization: Bearer <key>" for API and MCP requests.'
  name: apiKeyBearer
  scheme: bearer
  sources:
  - https://deployxa.com/llms.txt
  type: http
- flows:
  - authorizationUrl: https://deployxa.com/login
    flow: authorizationCode
    pkce_required: true
    registration_endpoint: https://deployxa.com/api/auth/extension/start
    tokenUrl: https://deployxa.com/api/auth/token
  name: oauthAgent
  sources:
  - https://deployxa.com/auth.md
  - https://deployxa.com/.well-known/oauth-authorization-server
  type: oauth2
- flows:
  - authorizationUrl: https://mcp.deployxa.com/oauth/authorize
    flow: authorizationCode
    pkce_required: true
    registration_endpoint: https://mcp.deployxa.com/oauth/register
    scopes: 8
    tokenUrl: https://mcp.deployxa.com/oauth/token
  name: mcpOAuth
  sources:
  - https://mcp.deployxa.com/.well-known/oauth-authorization-server
  type: oauth2
slug: deployxa-authentication
source_filename: deployxa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://deployxa.com/auth.md\ndocs: https://deployxa.com/auth.md\nnote: >-\n  The published OpenAPI declares no securitySchemes, so this profile is searched\n  from the provider's agent-auth document (auth.md, saved verbatim as\n  deployxa-auth.md) and the RFC 8414 / RFC 9728 well-known metadata on\n  deployxa.com and mcp.deployxa.com. Two credential paths: API keys created in\n  the dashboard (https://deployxa.com/dashboard/api-keys) used as bearer keys per\n  llms.txt, and an OAuth 2.0 authorization-code + PKCE flow for agents with\n  dynamic registration.\nsummary:\n  types: [http-bearer, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: apiKeyBearer\n    type: http\n    scheme: bearer\n    description: 'API key from the dashboard sent as \"Authorization: Bearer <key>\" for API and MCP requests.'\n    sources: [https://deployxa.com/llms.txt]\n  - name: oauthAgent\n    type: oauth2\n\
  \    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://deployxa.com/login\n        tokenUrl: https://deployxa.com/api/auth/token\n        pkce_required: true\n        registration_endpoint: https://deployxa.com/api/auth/extension/start\n    sources:\n      - https://deployxa.com/auth.md\n      - https://deployxa.com/.well-known/oauth-authorization-server\n  - name: mcpOAuth\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.deployxa.com/oauth/authorize\n        tokenUrl: https://mcp.deployxa.com/oauth/token\n        pkce_required: true\n        registration_endpoint: https://mcp.deployxa.com/oauth/register\n        scopes: 8\n    sources:\n      - https://mcp.deployxa.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deployxa/refs/heads/main/authentication/deployxa-authentication.yml
summary_line: http-bearer/oauth2 · 3 schemes
tags:
- platform-as-a-service
- cloud-deployment
- devops
- ci-cd
- containers-docker
- edge-hosting
- managed-databases
- ai-ops
- developer-tools
---
