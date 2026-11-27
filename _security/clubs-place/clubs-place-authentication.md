---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: CLUBS Authentication
name_suffix: Authentication
oauth_flows: []
overview: CLUBS declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: CLUBS
provider_slug: clubs-place
scheme_count: 3
schemes:
- applies_to:
  - https://clubs.place/api/mcp
  - https://clubs.place/api/nippo/mcp
  bearer_methods:
  - header
  description: OAuth 2.1 authorization code with PKCE (S256) and Dynamic Client Registration, public clients (token_endpoint_auth_methods_supported none). Advertised by RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata for both MCP resources.
  flows:
    authorizationCode:
      authorizationUrl: https://clubs.place/oauth/authorize
      pkce: S256
      refresh: true
      registrationUrl: https://clubs.place/api/nippo/oauth/register
      tokenUrl: https://clubs.place/api/nippo/oauth/token
  issuer: https://clubs.place
  name: clubs-oauth
  scopes:
  - nippo:agent:read
  - nippo:report:write
  - offline_access
  type: oauth2
- applies_to:
  - https://clubs.place/api/nippo/mcp
  description: The MCP Registry entry place.clubs/nippo v1.0.1 states that, in addition to OAuth 2.1+PKCE+DCR, a fixed Bearer header is supported ("OAuth 2.1+PKCE+DCR に加え Bearer 固定ヘッダー認証対応").
  name: fixed-bearer
  scheme: bearer
  source: https://registry.modelcontextprotocol.io/v0/servers?search=place.clubs
  type: http
- description: The @clubs.place/cli README states the connections screen issues a connection code valid for 10 minutes and single use, which init exchanges on the spot for an integration token stored in ~/.clubs-nippo/.env ("接続コードは 10 分・1 回限り有効で、init がその場で連携トークンに引き換える").
  name: cli-connection-code
  source: https://unpkg.com/@clubs.place/cli/README.md
  type: other
slug: clubs-place-authentication
source_filename: clubs-place-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: CLUBS authentication\ngenerated: '2026-11-04'\nmethod: probed\nsource: https://clubs.place/.well-known/oauth-authorization-server\ndocs: https://clubs.place/.well-known/oauth-protected-resource/api/nippo/mcp\nschemes:\n- name: clubs-oauth\n  type: oauth2\n  description: OAuth 2.1 authorization code with PKCE (S256) and Dynamic Client Registration, public clients (token_endpoint_auth_methods_supported none). Advertised by RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata for both MCP resources.\n  issuer: https://clubs.place\n  flows:\n    authorizationCode:\n      authorizationUrl: https://clubs.place/oauth/authorize\n      tokenUrl: https://clubs.place/api/nippo/oauth/token\n      registrationUrl: https://clubs.place/api/nippo/oauth/register\n      refresh: true\n      pkce: S256\n  scopes: [nippo:agent:read, nippo:report:write, offline_access]\n  bearer_methods: [header]\n  applies_to:\n  - https://clubs.place/api/mcp\n  - https://clubs.place/api/nippo/mcp\n\
  - name: fixed-bearer\n  type: http\n  scheme: bearer\n  description: The MCP Registry entry place.clubs/nippo v1.0.1 states that, in addition to OAuth 2.1+PKCE+DCR, a fixed Bearer header is supported (\"OAuth 2.1+PKCE+DCR に加え Bearer 固定ヘッダー認証対応\").\n  source: https://registry.modelcontextprotocol.io/v0/servers?search=place.clubs\n  applies_to:\n  - https://clubs.place/api/nippo/mcp\n- name: cli-connection-code\n  type: other\n  description: The @clubs.place/cli README states the connections screen issues a connection code valid for 10 minutes and single use, which init exchanges on the spot for an integration token stored in ~/.clubs-nippo/.env (\"接続コードは 10 分・1 回限り有効で、init がその場で連携トークンに引き換える\").\n  source: https://unpkg.com/@clubs.place/cli/README.md\nnotes: Discovery documents were fetched with GET only; no authorization, token or registration endpoint was called.\n"
source_yaml_url: https://artifacts.apis.io/clubs-place/authentication/clubs-place-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Artificial Intelligence
- MCP
- Productivity
- Notes
- Reporting
- Japan
---
