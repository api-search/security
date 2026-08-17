---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Spate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spate declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Spate
provider_slug: spate
scheme_count: 1
schemes:
- applies_to:
  - endpoint: https://api.spate.nyc/mcp
    enforcement: 'tools/call returns JSON-RPC error -32001 "Missing Authorization: Bearer token" without a token. initialize and tools/list are NOT gated and answer anonymously.'
    surface: MCP
  flows:
  - authorization_endpoint: https://api.spate.nyc/mcp/oauth/authorize
    flow: authorization_code
    pkce:
      methods:
      - plain
      - S256
      note: '`plain` is advertised alongside S256. OAuth 2.1 and the MCP authorization spec require S256; advertising `plain` weakens the PKCE guarantee for any client that negotiates it.'
      supported: true
    refresh: true
    scopes:
    - mcp
    token_endpoint: https://api.spate.nyc/mcp/oauth/token
    token_endpoint_auth_methods_supported:
    - none
  format: Bearer <access_token>
  header: Authorization
  id: spate_mcp_oauth
  in: header
  type: oauth2
slug: spate-authentication
source_filename: spate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://api.spate.nyc/.well-known/oauth-authorization-server\ndocs: https://help.spate.nyc/en/article/api-overview\nnote: >-\n  Derived from the RFC 8414 authorization-server metadata and the RFC 9728\n  protected-resource metadata Spate serves anonymously on api.spate.nyc, plus\n  the live JSON-RPC challenge returned by the MCP endpoint. Spate publishes no\n  OpenAPI, so there is no securitySchemes block to derive from — this profile\n  is built entirely from probed discovery documents and the help-center API\n  Overview article.\n\nschemes:\n- id: spate_mcp_oauth\n  type: oauth2\n  in: header\n  header: Authorization\n  format: Bearer <access_token>\n  flows:\n  - flow: authorization_code\n    authorization_endpoint: https://api.spate.nyc/mcp/oauth/authorize\n    token_endpoint: https://api.spate.nyc/mcp/oauth/token\n    refresh: true\n    pkce:\n      supported: true\n      methods: [plain, S256]\n      note: >-\n        `plain`\
  \ is advertised alongside S256. OAuth 2.1 and the MCP\n        authorization spec require S256; advertising `plain` weakens the\n        PKCE guarantee for any client that negotiates it.\n    token_endpoint_auth_methods_supported: [none]\n    scopes: [mcp]\n  applies_to:\n  - surface: MCP\n    endpoint: https://api.spate.nyc/mcp\n    enforcement: >-\n      tools/call returns JSON-RPC error -32001 \"Missing Authorization: Bearer\n      token\" without a token. initialize and tools/list are NOT gated and\n      answer anonymously.\n\nanonymous_surface:\n- endpoint: https://api.spate.nyc/mcp\n  methods: [initialize, tools/list]\n  note: Tool discovery is public; tool invocation is not.\n- endpoint: https://api.spate.nyc/.well-known/oauth-protected-resource\n- endpoint: https://api.spate.nyc/.well-known/oauth-authorization-server\n- endpoint: https://api.spate.nyc/.well-known/openid-configuration\n\napi_keys:\n  issued: false\n  evidence: >-\n    Spate's API Overview help article states plainly\
  \ that Spate \"does not\n    provide direct API keys\" and that \"API integrations are manually\n    configured by our technical team to ensure proper access and security.\"\n  source: https://help.spate.nyc/en/article/api-overview\n\naccess_requirements:\n- Minimum 5 seats on a Spate subscription\n- API access is a paid add-on, not included in a standard subscription\n- A named technical point of contact for setup\n- Onboarding routed through the Customer Success Manager or support@spate.nyc\n\ngaps:\n- No dynamic client registration endpoint advertised (RFC 7591 absent from\n  the authorization-server metadata), so an agent cannot self-register.\n- id_token_signing_alg_values_supported is [\"none\"] in the OpenID\n  configuration, which is not a usable OIDC signing posture; the document\n  reads as MCP OAuth metadata rather than a real OpenID Provider.\n- No published scope reference beyond the single coarse `mcp` scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spate/refs/heads/main/authentication/spate-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Enterprise Saas
- Market Intelligence
- Trend Forecasting
- Consumer Insights
- Social Listening
- Analytics
- Beauty
- MCP
- AI Agents
- Trend Data
- Consumer Packaged Goods
---
