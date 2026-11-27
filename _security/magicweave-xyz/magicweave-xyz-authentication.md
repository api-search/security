---
anonymous_access: false
api_key_in: []
api_specs:
- filename: magicweave-xyz-openapi-generated.yml
  format: yaml
  label: Magicweave API
  slug: magicweave-xyz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magicweave-xyz/openapi/_ae-authored/magicweave-xyz-openapi-generated.yml
auth_types: []
description: Authentication — Magicweave Docs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Magicweave Authentication
name_suffix: Authentication
oauth_flows: []
overview: Magicweave declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Magicweave
provider_slug: magicweave-xyz
scheme_count: 2
schemes:
- evidence: 'you exchange them for a player token once, at /v1/auth/token , then send Authorization: Bearer <access_token> on every other endpoint.'
  header: Authorization
  how_to_obtain: Exchange client_id and client_secret in the JSON body of POST /v1/auth/token for an access token.
  location: header
  name: Bearer
  token_url: /v1/auth/token
  type: http-bearer
- authorize_url: https://mcp.magicweave.xyz/mcp
  evidence: How an MCP client gets a token — the hosted connector at https://mcp.magicweave.xyz/mcp, signed in through OAuth.
  how_to_obtain: Use the hosted connector OAuth flow to obtain a token.
  name: OAuth2
  token_url: https://mcp.magicweave.xyz/mcp
  type: oauth2
slug: magicweave-xyz-authentication
source_filename: magicweave-xyz-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.magicweave.xyz/auth/
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.magicweave.xyz/auth/\nsources:\n- https://docs.magicweave.xyz/auth/\n- https://docs.magicweave.xyz/auth/signing-in/\n- https://docs.magicweave.xyz/auth/tiers-and-scopes/\n- https://docs.magicweave.xyz/concepts/environments-and-credentials/\ndescription: Authentication — Magicweave Docs\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'you exchange them for a player token once, at /v1/auth/token , then send Authorization: Bearer <access_token> on every other endpoint.'\n  location: header\n  header: Authorization\n  token_url: /v1/auth/token\n  how_to_obtain: Exchange client_id and client_secret in the JSON body of POST /v1/auth/token for an access token.\n- type: oauth2\n  name: OAuth2\n  evidence: How an MCP client gets a token — the hosted connector at https://mcp.magicweave.xyz/mcp, signed in through OAuth.\n  token_url: https://mcp.magicweave.xyz/mcp\n\
  \  authorize_url: https://mcp.magicweave.xyz/mcp\n  how_to_obtain: Use the hosted connector OAuth flow to obtain a token.\ndocs: https://docs.magicweave.xyz/auth/\n"
source_yaml_url: https://artifacts.apis.io/magicweave-xyz/authentication/magicweave-xyz-authentication.yml
summary_line: 2 schemes
tags:
- Gaming
- Backend
- Artificial Intelligence
- Platform
- Economy
---
