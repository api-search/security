---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CreativeScope Authentication
name_suffix: Authentication
oauth_flows: []
overview: CreativeScope declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CreativeScope
provider_slug: creativescope-ai
scheme_count: 2
schemes:
- client_id_metadata_document_supported: true
  description: Protected by OAuth. Short-lived tokens renew automatically, nothing is copied into config files, and you can revoke access from your account.
  dynamic_client_registration: https://api.creativescope.ai/oauth/register
  flows:
    authorizationCode:
      authorizationUrl: https://api.creativescope.ai/oauth/authorize
      refreshUrl: https://api.creativescope.ai/oauth/token
      scopes:
        mcp:use: Use the CreativeScope MCP server under your account
      tokenUrl: https://api.creativescope.ai/oauth/token
  name: oauth2
  pkce: S256
  revocation_endpoint: https://api.creativescope.ai/oauth/revoke
  token_endpoint_auth_methods:
  - none
  type: oauth2
- description: Headless agents, CI pipelines, mcp-remote and clients without OAuth support can use a free API key. See the API key page.
  format: Bearer YOUR_API_KEY
  header: Authorization
  in: header
  key_prefix: cs_live_
  key_prefix_source: https://github.com/creativescope/creativescope-mcp/blob/main/README.md
  name: apiKey
  scheme: bearer
  type: http
slug: creativescope-ai-authentication
source_filename: creativescope-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- https://www.creativescope.ai/mcp\n- https://www.creativescope.ai/mcp-api-key\n- https://api.creativescope.ai/.well-known/oauth-authorization-server\n- https://mcp.creativescope.ai/.well-known/oauth-protected-resource\ndocs: https://www.creativescope.ai/mcp\nnote: Applies to the remote MCP server https://mcp.creativescope.ai/mcp; no REST API is published. Authorization-server and protected-resource metadata were read with GET on 2026-11-04 (HTTP 200); no token, register or authorize endpoint was called.\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n    authorizationCode:\n      authorizationUrl: https://api.creativescope.ai/oauth/authorize\n      tokenUrl: https://api.creativescope.ai/oauth/token\n      refreshUrl: https://api.creativescope.ai/oauth/token\n      scopes:\n        mcp:use: Use the CreativeScope MCP server under your account\n  pkce: S256\n  token_endpoint_auth_methods: [none]\n  revocation_endpoint:\
  \ https://api.creativescope.ai/oauth/revoke\n  dynamic_client_registration: https://api.creativescope.ai/oauth/register\n  client_id_metadata_document_supported: true\n  description: \"Protected by OAuth. Short-lived tokens renew automatically, nothing is copied into config files, and you can revoke access from your account.\"\n- name: apiKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer YOUR_API_KEY'\n  key_prefix: cs_live_\n  key_prefix_source: https://github.com/creativescope/creativescope-mcp/blob/main/README.md\n  description: \"Headless agents, CI pipelines, mcp-remote and clients without OAuth support can use a free API key. See the API key page.\"\n"
source_yaml_url: https://artifacts.apis.io/creativescope-ai/authentication/creativescope-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Mobile Games
- Advertising
- Ad Intelligence
- User Acquisition
- Creative Analytics
- MCP
- AI Agents
---
