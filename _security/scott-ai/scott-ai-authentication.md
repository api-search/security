---
api_key_in: []
api_specs:
- filename: scott-ai-openapi-original.json
  format: json
  label: Scott One-Shot API
  slug: scott-one-shot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scott-ai/refs/heads/main/openapi/scott-ai-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Scott Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scott Ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scott Ai
provider_slug: scott-ai
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/scott-ai-openapi-original.json
  type: http
slug: scott-ai-authentication
source_filename: scott-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/scott-ai-openapi-original.json\ndocs: https://docs.tryscott.ai/getting-started/concepts.md\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  token_format: jwt-rs256\ndetails: >-\n  All authenticated operations use an HTTP bearer JWT (Authorization: Bearer\n  <jwt>). Session tokens are minted by exchanging a Stytch OAuth token at\n  POST /auth/oauth/exchange (the exchange endpoint is itself unauthenticated and\n  is the authentication mechanism). JWTs are signed RS256 and verifiable against\n  https://api.tryscott.ai/.well-known/jwks.json (kid traffic-token-v1).\n  Short-lived workspace-scoped agent tokens are minted via\n  POST /agent-loop/workspaces/{workspace_id}/access-token and redeemed by\n  sandboxes via the internal handoff-code endpoint. There is no OAuth2/OIDC\n  securityScheme and no API-key scheme.\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n\
  \  - openapi/scott-ai-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scott-ai/refs/heads/main/authentication/scott-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Coding Agents
- AI
- Developer Tools
- Collaboration
- Agentic Workflow
- Model Context Protocol
- Software Design
---
