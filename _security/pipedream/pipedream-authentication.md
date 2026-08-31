---
api_key_in: []
api_specs:
- filename: pipedream-accounts-api-openapi.yml
  format: yaml
  label: Pipedream Accounts API
  slug: pipedream-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-accounts-api-openapi.yml
- filename: pipedream-actions-api-openapi.yml
  format: yaml
  label: Pipedream Actions API
  slug: pipedream-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-actions-api-openapi.yml
- filename: pipedream-app-categories-api-openapi.yml
  format: yaml
  label: Pipedream App Categories API
  slug: pipedream-app-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-app-categories-api-openapi.yml
- filename: pipedream-apps-api-openapi.yml
  format: yaml
  label: Pipedream Apps API
  slug: pipedream-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-apps-api-openapi.yml
- filename: pipedream-components-api-openapi.yml
  format: yaml
  label: Pipedream Components API
  slug: pipedream-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-components-api-openapi.yml
- filename: pipedream-deployed-triggers-api-openapi.yml
  format: yaml
  label: Pipedream Deployed Triggers API
  slug: pipedream-deployed-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-deployed-triggers-api-openapi.yml
- filename: pipedream-file-stash-api-openapi.yml
  format: yaml
  label: Pipedream File Stash API
  slug: pipedream-file-stash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-file-stash-api-openapi.yml
- filename: pipedream-mcp-api-openapi.yml
  format: yaml
  label: Pipedream MCP API
  slug: pipedream-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-mcp-api-openapi.yml
- filename: pipedream-oauth-api-openapi.yml
  format: yaml
  label: Pipedream OAuth API
  slug: pipedream-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-oauth-api-openapi.yml
- filename: pipedream-projects-api-openapi.yml
  format: yaml
  label: Pipedream Projects API
  slug: pipedream-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-projects-api-openapi.yml
- filename: pipedream-proxy-api-openapi.yml
  format: yaml
  label: Pipedream Proxy API
  slug: pipedream-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-proxy-api-openapi.yml
- filename: pipedream-tokens-api-openapi.yml
  format: yaml
  label: Pipedream Tokens API
  slug: pipedream-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-tokens-api-openapi.yml
- filename: pipedream-triggers-api-openapi.yml
  format: yaml
  label: Pipedream Triggers API
  slug: pipedream-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-triggers-api-openapi.yml
- filename: pipedream-usage-api-openapi.yml
  format: yaml
  label: Pipedream Usage API
  slug: pipedream-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-usage-api-openapi.yml
- filename: pipedream-users-api-openapi.yml
  format: yaml
  label: Pipedream Users API
  slug: pipedream-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-users-api-openapi.yml
- filename: pipedream-webhooks-api-openapi.yml
  format: yaml
  label: Pipedream Webhooks API
  slug: pipedream-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-webhooks-api-openapi.yml
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
