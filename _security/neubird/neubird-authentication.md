---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Neubird Authentication
name_suffix: Authentication
oauth_flows: []
overview: Neubird secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Neubird
provider_slug: neubird
scheme_count: 2
schemes:
- description: Email + password submitted to the NeuBird login API (or via X-NeuBird-Email / X-NeuBird-Password headers on the remote MCP server) are exchanged for a JWT bearer token.
  name: emailPasswordLogin
  parameters:
  - NEUBIRD_EMAIL
  - NEUBIRD_PASSWORD
  scheme: basic-credentials
  sources:
  - https://docs.neubird.ai/mcp/getting-started/installation/
  type: http
- bearerFormat: JWT
  description: 'Authorization: Bearer <token>. Tokens are JWTs issued by the NeuBird login API and validated through Auth0.'
  identity_provider: Auth0
  name: bearerJwt
  scheme: bearer
  sources:
  - https://docs.neubird.ai/mcp/getting-started/installation/
  type: http
slug: neubird-authentication
source_filename: neubird-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.neubird.ai/mcp/getting-started/installation/\ndocs: https://docs.neubird.ai/mcp/overview/\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  identity_provider: Auth0\n  notes: >-\n    No public OpenAPI was found, so this profile is derived from NeuBird's\n    documented authentication surface (login API + MCP server credentials) rather\n    than from a securitySchemes block.\nschemes:\n  - name: emailPasswordLogin\n    type: http\n    scheme: basic-credentials\n    description: >-\n      Email + password submitted to the NeuBird login API (or via\n      X-NeuBird-Email / X-NeuBird-Password headers on the remote MCP server) are\n      exchanged for a JWT bearer token.\n    parameters: [NEUBIRD_EMAIL, NEUBIRD_PASSWORD]\n    sources: [https://docs.neubird.ai/mcp/getting-started/installation/]\n  - name: bearerJwt\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Authorization:\
  \ Bearer <token>. Tokens are JWTs issued by the NeuBird login\n      API and validated through Auth0.\n    identity_provider: Auth0\n    sources: [https://docs.neubird.ai/mcp/getting-started/installation/]\nconnection_credentials:\n  # Per-integration credentials configured against connected data sources.\n  - provider: aws\n    credential: IAM role ARN + external ID\n  - provider: datadog\n    credential: API key + application key\nbase_url: https://api.neubird.ai\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neubird/refs/heads/main/authentication/neubird-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- AI SRE
- Incident Response
- Observability
- DevOps
- AIOps
- Root Cause Analysis
- Model Context Protocol
- Agentic AI
---
