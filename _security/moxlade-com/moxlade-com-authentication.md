---
anonymous_access: false
api_key_in: []
api_specs:
- filename: moxlade-com-ext-api-openapi.yml
  format: yaml
  label: Moxlade Ext API
  slug: moxlade-com-ext-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moxlade-com/openapi/moxlade-com-ext-api-openapi.yml
- filename: moxlade-com-mcp-api-openapi.yml
  format: yaml
  label: Moxlade MCP API
  slug: moxlade-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moxlade-com/openapi/moxlade-com-mcp-api-openapi.yml
auth_types: []
description: Authentication methods for Moxlade API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Moxlade Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moxlade declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Moxlade
provider_slug: moxlade-com
scheme_count: 2
schemes:
- evidence: 'Send it as `Authorization: Bearer mxt_…`.'
  header: Authorization
  how_to_obtain: Mint a token via the /connect endpoint; the token is shown once at mint and must be sent in the Authorization header.
  location: header
  name: Bearer Token
  type: http-bearer
- evidence: This endpoint is also an OAuth 2.1 resource server, so a client that speaks the MCP authorization spec can connect from the URL alone.
  how_to_obtain: Clients register themselves (RFC 7591) and use the MCP authorization spec with PKCE; no client id or secret is required.
  name: OAuth 2.1
  type: oauth2
slug: moxlade-com-authentication
source_filename: moxlade-com-authentication.yml
source_heading: Authentication Profile
source_url: https://buyer.moxlade.com/docs/auth
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://buyer.moxlade.com/docs/auth\nsources:\n- https://buyer.moxlade.com/docs/auth\n- https://buyer.moxlade.com/docs/auth.md\n- https://buyer.moxlade.com/docs/quickstart\n- https://buyer.moxlade.com/docs/quickstart.md\ndescription: Authentication methods for Moxlade API\nschemes:\n- type: http-bearer\n  name: Bearer Token\n  evidence: 'Send it as `Authorization: Bearer mxt_…`.'\n  location: header\n  header: Authorization\n  how_to_obtain: Mint a token via the /connect endpoint; the token is shown once at mint and must be sent in the Authorization header.\n- type: oauth2\n  name: OAuth 2.1\n  evidence: This endpoint is also an OAuth 2.1 resource server, so a client that speaks the MCP authorization spec can connect from the URL alone.\n  how_to_obtain: Clients register themselves (RFC 7591) and use the MCP authorization spec with PKCE; no client id or secret is required.\ndocs:\
  \ https://buyer.moxlade.com/docs/auth\n"
source_yaml_url: https://artifacts.apis.io/moxlade-com/authentication/moxlade-com-authentication.yml
summary_line: 2 schemes
tags:
- Upwork data
- Freelancer data
- Buyer Intelligence
- Data Marketplace
- Apify actors
---
