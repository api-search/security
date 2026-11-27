---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Departi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Departi declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Departi
provider_slug: departi-eu
scheme_count: 3
schemes:
- description: Anonymous access works for general queries.
  endpoint: https://mcp.departi.eu/v3
  name: anonymous
  type: none
- description: Full OAuth 2.1 with PKCE (S256). Claude handles the handshake automatically
  dynamic_client_registration: true
  endpoint: https://mcp.departi.eu/v3/oauth
  flows:
  - authorizationCode
  metadata:
    authorization_server: /.well-known/oauth-authorization-server
    protected_resource: /.well-known/oauth-protected-resource/v3/oauth
  name: oauth21
  pkce: S256
  scopes:
  - departi:read
  token_lifetime: Tokens are scoped to departi:read with 1-hour access tokens and 30-day refresh tokens with rotation.
  type: oauth2
- description: 'For personalized results, generate an API token from your Departi account settings and pass it as Authorization: Bearer mcp_... .'
  endpoint: https://mcp.departi.eu/v3
  name: bearer-token
  scheme: bearer
  token_prefix: mcp_
  type: http
slug: departi-eu-authentication
source_filename: departi-eu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://departi.eu/developers/mcp\ndocs: https://departi.eu/developers/mcp\nname: Departi authentication\nnote: No OpenAPI is published; the profile is read from the MCP integration guide. Public MCP tools at https://mcp.departi.eu/v3 need no authentication.\nschemes:\n- name: anonymous\n  type: none\n  endpoint: https://mcp.departi.eu/v3\n  description: \"Anonymous access works for general queries.\"\n- name: oauth21\n  type: oauth2\n  flows: [authorizationCode]\n  pkce: S256\n  endpoint: https://mcp.departi.eu/v3/oauth\n  scopes: [departi:read]\n  description: \"Full OAuth 2.1 with PKCE (S256). Claude handles the handshake automatically\"\n  token_lifetime: \"Tokens are scoped to departi:read with 1-hour access tokens and 30-day refresh tokens with rotation.\"\n  dynamic_client_registration: true\n  metadata:\n    protected_resource: /.well-known/oauth-protected-resource/v3/oauth\n    authorization_server: /.well-known/oauth-authorization-server\n\
  - name: bearer-token\n  type: http\n  scheme: bearer\n  endpoint: https://mcp.departi.eu/v3\n  token_prefix: mcp_\n  description: \"For personalized results, generate an API token from your Departi account settings and pass it as Authorization: Bearer mcp_... .\"\n"
source_yaml_url: https://artifacts.apis.io/departi-eu/authentication/departi-eu-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Travel
- Digital Nomads
- Accommodation
- Visa
- MCP
- AI Concierge
- Europe
---
