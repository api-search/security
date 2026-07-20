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
name: Jedify Authentication
name_suffix: Authentication
oauth_flows:
- browser-login
overview: Jedify secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the browser-login flow(s).
provider_name: Jedify
provider_slug: jedify
scheme_count: 3
schemes:
- created_at: https://app.jedify.com/settings/api-keys
  description: Required on every REST API request to https://be.jedify.com/api. Keys are created in the Jedify app at app.jedify.com/settings/api-keys and are bound to the creating user's identity and permissions. Published/hosted apps use a single shared key, so all viewers see data at that key's permission level.
  in: header
  name: apiKeyHeader
  parameter_name: X-API-Key
  sources:
  - docs.jedify.com/api-reference/overview
  type: apiKey
- description: Interactive OAuth sign-in used by desktop MCP clients (Claude Desktop, Cursor) via the @jedify/mcp-auth proxy. Sessions refresh automatically. Identity is handled by Descope (observed in the app.jedify.com client bundle).
  identity_provider: Descope
  name: browserLogin
  scheme: browser-login
  sources:
  - docs.jedify.com/mcp/authentication
  type: oauth2
- description: MCP proxy alternative to browser login; provide JEDIFY_API_KEY (requires @jedify/mcp-auth v1.1.0+). Skips browser login for headless environments.
  in: header
  name: mcpApiKey
  sources:
  - docs.jedify.com/mcp/authentication
  type: apiKey
slug: jedify-authentication
source_filename: jedify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.jedify.com/api-reference/overview\ndocs: https://docs.jedify.com/mcp/authentication\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [browser-login]\nschemes:\n  - name: apiKeyHeader\n    type: apiKey\n    in: header\n    parameter_name: X-API-Key\n    description: >-\n      Required on every REST API request to https://be.jedify.com/api. Keys are\n      created in the Jedify app at app.jedify.com/settings/api-keys and are bound\n      to the creating user's identity and permissions. Published/hosted apps use a\n      single shared key, so all viewers see data at that key's permission level.\n    created_at: https://app.jedify.com/settings/api-keys\n    sources: [docs.jedify.com/api-reference/overview]\n  - name: browserLogin\n    type: oauth2\n    scheme: browser-login\n    description: >-\n      Interactive OAuth sign-in used by desktop MCP clients (Claude Desktop, Cursor)\n     \
  \ via the @jedify/mcp-auth proxy. Sessions refresh automatically. Identity is\n      handled by Descope (observed in the app.jedify.com client bundle).\n    identity_provider: Descope\n    sources: [docs.jedify.com/mcp/authentication]\n  - name: mcpApiKey\n    type: apiKey\n    in: header\n    description: >-\n      MCP proxy alternative to browser login; provide JEDIFY_API_KEY (requires\n      @jedify/mcp-auth v1.1.0+). Skips browser login for headless environments.\n    sources: [docs.jedify.com/mcp/authentication]\nenterprise_sso:\n  supported: true\n  methods: [SAML, Azure AD]\n  rbac: true\n  docs:\n    sso_setup: https://docs.jedify.com/settings/sso-setup\n    azure_ad_sso: https://docs.jedify.com/settings/azure-ad-sso\n    rbac: https://docs.jedify.com/settings/rbac\n    idp_groups: https://docs.jedify.com/settings/idp-groups\nnotes: >-\n  No OpenAPI securitySchemes were harvestable (the published openapi.json is the\n  default Mintlify Plant Store sample, not Jedify's API), so\
  \ this profile was\n  searched from the docs rather than derived.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jedify/refs/heads/main/authentication/jedify-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Artificial Intelligence
- Data Analytics
- Business Intelligence
- Semantic Layer
- Context Layer
- Data Agents
- MCP
- Enterprise AI
- Natural Language Query
---
