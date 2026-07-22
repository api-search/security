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
name: Trellis Research Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Trellis Research secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Trellis Research
provider_slug: trellis-research
scheme_count: 2
schemes:
- applies_to: Trellis REST Data API (V2)
  in: header
  name: apiKeyAuth
  parameter: Authorization
  provisioning: Generated from Trellis account Settings page
  source: https://support.trellis.law/trellis-api
  type: apiKey
- applies_to: Trellis Law MCP server (mcp.trellis.law)
  authorization_endpoint: https://mcp.trellis.law/oauth/authorize
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://mcp.trellis.law
  name: oauth2
  notes: OAuth 2.0 (RFC 8414 + RFC 9728 discovery published at mcp.trellis.law); PKCE S256 and dynamic client registration; no API keys exposed to the MCP client.
  pkce: S256
  registration_endpoint: https://mcp.trellis.law/oauth/register
  scopes:
  - mcp
  source: https://support.trellis.law/trellis-law-mcp-technical-documentation
  token_endpoint: https://mcp.trellis.law/oauth/token
  type: oauth2
slug: trellis-research-authentication
source_filename: trellis-research-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://support.trellis.law/trellis-api\ndocs: https://support.trellis.law/trellis-api\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    The Trellis REST Data API (V2, introduced May 2024) authenticates with a\n    unique API key sent in the Authorization header. The API key is generated\n    from the Trellis account Settings page (bottom-left of the app). Keys are\n    private, must not be shared publicly, and all requests should be made\n    server-side. The separate remote MCP server (mcp.trellis.law) authenticates\n    with OAuth 2.0 so that no API key is exposed to the client.\nschemes:\n  - name: apiKeyAuth\n    type: apiKey\n    in: header\n    parameter: Authorization\n    applies_to: Trellis REST Data API (V2)\n    source: https://support.trellis.law/trellis-api\n    provisioning: Generated from Trellis account Settings page\n  - name: oauth2\n    type:\
  \ oauth2\n    applies_to: Trellis Law MCP server (mcp.trellis.law)\n    source: https://support.trellis.law/trellis-law-mcp-technical-documentation\n    issuer: https://mcp.trellis.law\n    authorization_endpoint: https://mcp.trellis.law/oauth/authorize\n    token_endpoint: https://mcp.trellis.law/oauth/token\n    registration_endpoint: https://mcp.trellis.law/oauth/register\n    grant_types: [authorization_code, refresh_token]\n    pkce: S256\n    scopes: [mcp]\n    notes: >-\n      OAuth 2.0 (RFC 8414 + RFC 9728 discovery published at mcp.trellis.law);\n      PKCE S256 and dynamic client registration; no API keys exposed to the\n      MCP client.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trellis-research/refs/heads/main/authentication/trellis-research-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Legal
- Legal Research
- Court Records
- Litigation Analytics
- Judicial Analytics
- Legal Data
- API
- MCP
---
