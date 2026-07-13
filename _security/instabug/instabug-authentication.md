---
api_key_in: []
api_specs:
- filename: instabug-mcp-server-openapi.yml
  format: yaml
  label: Luciq MCP Server
  slug: mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instabug/refs/heads/main/openapi/instabug-mcp-server-openapi.yml
- filename: instabug-webhooks-asyncapi.yml
  format: yaml
  label: Luciq Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/instabug/refs/heads/main/asyncapi/instabug-webhooks-asyncapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Instabug Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Instabug (Luciq) secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Instabug (Luciq)
provider_slug: instabug
scheme_count: 2
schemes:
- description: OAuth 2.0 with Dynamic Client Registration. The Luciq MCP server advertises its authorization and token endpoints to MCP clients that register dynamically — no pre-shared client ID/secret is required.
  flows:
  - authorizationUrl: https://api.luciq.ai/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.luciq.ai/oauth/token
  name: oauth2
  sources:
  - openapi/instabug-mcp-server-openapi.yml
  type: oauth2
- bearerFormat: token
  description: 'Personal Access Token generated from the Luciq dashboard under Account Management > Luciq MCP. Pass as `Authorization: Bearer <pat>`.'
  name: personalAccessToken
  scheme: bearer
  sources:
  - openapi/instabug-mcp-server-openapi.yml
  type: http
slug: instabug-authentication
source_filename: instabug-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/instabug-mcp-server-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.luciq.ai/oauth/authorize\n    tokenUrl: https://api.luciq.ai/oauth/token\n    scopes: 1\n  description: OAuth 2.0 with Dynamic Client Registration. The Luciq MCP server advertises its\n    authorization and token endpoints to MCP clients that register dynamically — no pre-shared\n    client ID/secret is required.\n  sources:\n  - openapi/instabug-mcp-server-openapi.yml\n- name: personalAccessToken\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  description: 'Personal Access Token generated from the Luciq dashboard under Account Management\n    > Luciq MCP. Pass as `Authorization: Bearer <pat>`.'\n  sources:\n  - openapi/instabug-mcp-server-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instabug/refs/heads/main/authentication/instabug-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Agentic AI
- APM
- Application Performance Monitoring
- Bug Reporting
- Crash Reporting
- MCP
- Mobile
- Mobile Observability
- Observability
- Session Replay
---
