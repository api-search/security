---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: intentdocs-com-cli-api-openapi.yml
  format: yaml
  label: intentdocs-com CLI API
  slug: intentdocs-com-cli-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intentdocs-com/openapi/intentdocs-com-cli-api-openapi.yml
- filename: intentdocs-com-mcp-api-openapi.yml
  format: yaml
  label: intentdocs-com MCP API
  slug: intentdocs-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intentdocs-com/openapi/intentdocs-com-mcp-api-openapi.yml
- filename: intentdocs-com-oauth-api-openapi.yml
  format: yaml
  label: intentdocs-com OAuth API
  slug: intentdocs-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intentdocs-com/openapi/intentdocs-com-oauth-api-openapi.yml
- filename: intentdocs-com-sync-api-openapi.yml
  format: yaml
  label: intentdocs-com Sync API
  slug: intentdocs-com-sync-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intentdocs-com/openapi/intentdocs-com-sync-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Intentdocs Com Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: intentdocs-com secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: intentdocs-com
provider_slug: intentdocs-com
scheme_count: 2
schemes:
- description: OAuth 2.1 bearer token. Obtain via /api/oauth/authorize → /api/oauth/token flow, or use intent_cli_* tokens from /api/cli/auth.
  flows:
  - authorizationUrl: https://intentdocs.com/api/oauth/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://intentdocs.com/api/oauth/token
  name: bearerAuth
  sources:
  - openapi/intentdocs-com-openapi.json
  type: oauth2
- description: Clerk session cookie (browser auth only)
  in: cookie
  name: clerkAuth
  parameter: __session
  sources:
  - openapi/intentdocs-com-openapi.json
  type: apiKey
slug: intentdocs-com-authentication
source_filename: intentdocs-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/intentdocs-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - cookie\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://intentdocs.com/api/oauth/authorize\n    tokenUrl: https://intentdocs.com/api/oauth/token\n    scopes: 6\n  description: OAuth 2.1 bearer token. Obtain via /api/oauth/authorize → /api/oauth/token flow,\n    or use intent_cli_* tokens from /api/cli/auth.\n  sources:\n  - openapi/intentdocs-com-openapi.json\n- name: clerkAuth\n  type: apiKey\n  in: cookie\n  parameter: __session\n  description: Clerk session cookie (browser auth only)\n  sources:\n  - openapi/intentdocs-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/intentdocs-com/authentication/intentdocs-com-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- AI
- Spec-Driven
- Platform
- Automation
- Low-Code
---
