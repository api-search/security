---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Codenow Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CodeNOW secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CodeNOW
provider_slug: codenow
scheme_count: 2
schemes:
- description: Pass your unique CodeNOW API key in the X-Codenow-Api-Key request header. Keys are obtained from the CodeNOW user profile and their permissions are tied to the user's Role-Based Access Control (RBAC) settings. Keys can be regenerated from account settings.
  docs: https://docs.codenow.com/api/overview/authentication/
  in: header
  name: ApiKeyAuth
  parameter_name: X-Codenow-Api-Key
  sources:
  - docs
  type: apiKey
- applies_to: mcp-server
  description: OAuth 2.0 is the recommended authentication method for the CodeNOW MCP server (browser-based login with JWT token refresh). The REST API itself is authenticated with the X-Codenow-Api-Key header.
  docs: https://docs.codenow.com/api/overview/mcp-server/
  name: OAuth2
  sources:
  - docs
  type: oauth2
slug: codenow-authentication
source_filename: codenow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.codenow.com/api/overview/authentication/\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter_name: X-Codenow-Api-Key\n    description: >-\n      Pass your unique CodeNOW API key in the X-Codenow-Api-Key request header.\n      Keys are obtained from the CodeNOW user profile and their permissions are\n      tied to the user's Role-Based Access Control (RBAC) settings. Keys can be\n      regenerated from account settings.\n    docs: https://docs.codenow.com/api/overview/authentication/\n    sources: [docs]\n  - name: OAuth2\n    type: oauth2\n    description: >-\n      OAuth 2.0 is the recommended authentication method for the CodeNOW MCP\n      server (browser-based login with JWT token refresh). The REST API itself\n      is authenticated with the X-Codenow-Api-Key header.\n    applies_to:\
  \ mcp-server\n    docs: https://docs.codenow.com/api/overview/mcp-server/\n    sources: [docs]\nnotes:\n  - The REST API base URL is https://api.codenow.com/.\n  - API key permissions inherit the calling user's RBAC role.\n  - No public OpenAPI/Swagger document was found to derive schemes mechanically; this profile is captured from the published authentication documentation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codenow/refs/heads/main/authentication/codenow-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- DevOps
- Software Delivery
- Platform Engineering
- Governance
- AI Agents
- CI/CD
- Deployment
- Kubernetes
- Model Context Protocol
---
