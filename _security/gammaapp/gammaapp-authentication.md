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
name: Gammaapp Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Gamma.app secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Gamma.app
provider_slug: gammaapp
scheme_count: 2
schemes:
- in: header
  key_prefix: sk-gamma-
  name: ApiKeyAuth
  notes: All REST requests require an API key in the case-sensitive X-API-KEY header. Keys start with sk-gamma-. Invalid/missing keys return 401 "Invalid API key".
  parameter_name: X-API-KEY
  plans:
  - Pro
  - Ultra
  - Teams
  - Business
  provisioning: https://gamma.app/settings/api-keys
  surface: REST API (https://public-api.gamma.app/v1.0)
  type: apiKey
- authorization_server: https://auth.gamma.app
  dynamic_client_registration: true
  name: OAuth2
  notes: The hosted MCP server (and the ChatGPT/Claude connectors it powers) uses OAuth 2.0 Bearer tokens with Dynamic Client Registration. Available on all plans.
  protected_resource_metadata: https://mcp.gamma.app/.well-known/oauth-protected-resource
  scheme: bearer
  scopes:
  - generate
  - gamma:read
  specs:
  - RFC 9728
  - RFC 7591
  surface: Gamma MCP server (https://mcp.gamma.app/mcp)
  type: oauth2
slug: gammaapp-authentication
source_filename: gammaapp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://developers.gamma.app/get-started/understanding-the-api-options ,\n  https://developers.gamma.app/reference/error-codes ,\n  https://developers.gamma.app/mcp/mcp-tools-reference\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: X-API-KEY\n  key_prefix: sk-gamma-\n  surface: REST API (https://public-api.gamma.app/v1.0)\n  plans: [Pro, Ultra, Teams, Business]\n  provisioning: https://gamma.app/settings/api-keys\n  notes: >-\n    All REST requests require an API key in the case-sensitive X-API-KEY header.\n    Keys start with sk-gamma-. Invalid/missing keys return 401 \"Invalid API key\".\n- name: OAuth2\n  type: oauth2\n  scheme: bearer\n  surface: Gamma MCP server (https://mcp.gamma.app/mcp)\n  authorization_server: https://auth.gamma.app\n  protected_resource_metadata: https://mcp.gamma.app/.well-known/oauth-protected-resource\n\
  \  dynamic_client_registration: true\n  specs: [RFC 9728, RFC 7591]\n  scopes: [generate, 'gamma:read']\n  notes: >-\n    The hosted MCP server (and the ChatGPT/Claude connectors it powers) uses\n    OAuth 2.0 Bearer tokens with Dynamic Client Registration. Available on all\n    plans.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gammaapp/refs/heads/main/authentication/gammaapp-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- Presentations
- Documents
- Content Generation
- Generative AI
- Productivity
- MCP
- Websites
- Social Media
---
