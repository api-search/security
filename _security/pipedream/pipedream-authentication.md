---
api_key_in: []
api_specs:
- filename: pipedream-openapi.yml
  format: yaml
  label: Pipedream REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-openapi.yml
- filename: pipedream-openapi.yml
  format: yaml
  label: Pipedream Connect
  slug: connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-openapi.yml
- filename: pipedream-mcp-openapi.yml
  format: yaml
  label: Pipedream MCP Server
  slug: mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-mcp-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Pipedream Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Pipedream secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Pipedream
provider_slug: pipedream
scheme_count: 2
schemes:
- bearerFormat: OAuth access token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pipedream-mcp-openapi.yml
  - openapi/pipedream-openapi.yml
  type: http
- description: A short-lived OAuth access token for server-side requests. Generate one via the Generate OAuth Token flow or automatically when initializing the SDK client.
  flows:
  - flow: clientCredentials
    scopes: 16
    tokenUrl: https://api.pipedream.com/v1/oauth/token
  name: OAuth2
  sources:
  - openapi/pipedream-openapi.yml
  type: oauth2
slug: pipedream-authentication
source_filename: pipedream-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pipedream-mcp-openapi.yml, openapi/pipedream-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth access token\n  sources:\n  - openapi/pipedream-mcp-openapi.yml\n  - openapi/pipedream-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.pipedream.com/v1/oauth/token\n    scopes: 16\n  description: A short-lived OAuth access token for server-side requests. Generate one via the\n    Generate OAuth Token flow or automatically when initializing the SDK client.\n  sources:\n  - openapi/pipedream-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/authentication/pipedream-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- ProCode_API_Composition
- Workflows
- Connect
- MCP
- Embedded Integrations
- Managed Auth
- AI Agents
---
