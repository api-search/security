---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cut-pro-openapi-generated.yml
  format: yaml
  label: Cut.Pro API
  slug: cut-pro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cut-pro/openapi/_ae-authored/cut-pro-openapi-generated.yml
auth_types: []
description: Authentication methods for Cut.Pro as documented.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Cut Pro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cut.Pro declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Cut.Pro
provider_slug: cut-pro
scheme_count: 3
schemes:
- evidence: 'Use o header `X-Api-Key`:'
  header: X-Api-Key
  how_to_obtain: Create a key in the Cut.Pro Studio UI (https://cut.pro/studio/me/api-keys) and copy it once.
  location: header
  name: X-Api-Key
  type: apiKey
- evidence: 'Ou `Authorization: Bearer`, se o seu cliente HTTP já monta esse header:'
  header: Authorization
  how_to_obtain: Create a key in the Cut.Pro Studio UI (https://cut.pro/studio/me/api-keys) and copy it once.
  location: header
  name: Authorization
  type: apiKey
- authorize_url: https://mcp.cut.pro/authorize
  evidence: '`https://mcp.cut.pro` is a Streamable HTTP MCP server exposing the v1 API as tools. It runs a full OAuth 2.1 authorization server with PKCE and **dynamic client registration**, so a client can register itself:'
  flows:
  - authorization_code
  - refresh_token
  how_to_obtain: Register dynamically via the MCP server (https://mcp.cut.pro/register) and complete the consent flow to receive an OAuth 2.1 access token.
  name: MCP server
  scopes:
  - cutpro
  type: oauth2
slug: cut-pro-authentication
source_filename: cut-pro-authentication.yml
source_heading: Authentication Profile
source_url: https://cut.pro/docs/authentication
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://cut.pro/docs/authentication\nsources:\n- https://cut.pro/docs/authentication\n- https://cut.pro/docs/authentication.md\n- https://cut.pro/auth.md\ndescription: Authentication methods for Cut.Pro as documented.\nschemes:\n- type: apiKey\n  name: X-Api-Key\n  evidence: 'Use o header `X-Api-Key`:'\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Create a key in the Cut.Pro Studio UI (https://cut.pro/studio/me/api-keys) and copy it once.\n- type: apiKey\n  name: Authorization\n  evidence: 'Ou `Authorization: Bearer`, se o seu cliente HTTP já monta esse header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the Cut.Pro Studio UI (https://cut.pro/studio/me/api-keys) and copy it once.\n- type: oauth2\n  name: MCP server\n  evidence: '`https://mcp.cut.pro` is a Streamable HTTP MCP server exposing the v1 API as tools. It runs a full OAuth\
  \ 2.1 authorization server\n    with PKCE and **dynamic client registration**, so a client can register itself:'\n  flows:\n  - authorization_code\n  - refresh_token\n  authorize_url: https://mcp.cut.pro/authorize\n  scopes:\n  - cutpro\n  how_to_obtain: Register dynamically via the MCP server (https://mcp.cut.pro/register) and complete the consent flow to receive an OAuth 2.1\n    access token.\ndocs: https://cut.pro/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/cut-pro/authentication/cut-pro-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Artificial Intelligence
- Video
- Clipping
- Social Media
- Brazil
---
