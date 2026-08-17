---
api_key_in: []
api_specs:
- filename: orthogonal-account-api-openapi.yml
  format: yaml
  label: Orthogonal Account API
  slug: orthogonal-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orthogonal/refs/heads/main/openapi/orthogonal-account-api-openapi.yml
- filename: orthogonal-discovery-api-openapi.yml
  format: yaml
  label: Orthogonal Discovery API
  slug: orthogonal-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orthogonal/refs/heads/main/openapi/orthogonal-discovery-api-openapi.yml
- filename: orthogonal-run-api-openapi.yml
  format: yaml
  label: Orthogonal Run API
  slug: orthogonal-run-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orthogonal/refs/heads/main/openapi/orthogonal-run-api-openapi.yml
- filename: orthogonal-marketplace-openapi.json
  format: json
  label: Orthogonal API Marketplace
  slug: orthogonal-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orthogonal/refs/heads/main/openapi/_original/orthogonal-marketplace-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Orthogonal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orthogonal declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Orthogonal
provider_slug: orthogonal
scheme_count: 2
schemes:
- applies_to:
  - REST API (api.orthogonal.com)
  - CLI (@orth/cli)
  - SDKs (@orth/sdk, orth)
  env_var: ORTHOGONAL_API_KEY
  format: 'Authorization: Bearer orth_live_...'
  header: Authorization
  id: bearerAuth
  in: header
  key_prefixes:
  - mode: live
    note: production, billable
    prefix: orth_live_
  - mode: test
    note: testing, no charges
    prefix: orth_test_
  scheme: bearer
  type: http
- applies_to:
  - Hosted MCP server (mcp.orthogonal.com)
  authorization_endpoint: https://clerk.orthogonal.com/oauth/authorize
  flow: authorization_code
  id: oauth2
  issuer: https://clerk.orthogonal.com
  jwks_uri: https://clerk.orthogonal.com/.well-known/jwks.json
  pkce: S256
  registration_endpoint: https://mcp.orthogonal.com/oauth/register
  revocation_endpoint: https://clerk.orthogonal.com/oauth/token/revoke
  scopes:
  - openid
  - profile
  - email
  - public_metadata
  - private_metadata
  - offline_access
  - user:org:read
  token_endpoint: https://clerk.orthogonal.com/oauth/token
  type: oauth2
slug: orthogonal-authentication
source_filename: orthogonal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.orthogonal.com/authentication.md + live oauth-authorization-server metadata\nsummary: >-\n  The REST API and CLI authenticate with an API key passed as an HTTP bearer\n  token. The hosted MCP server authenticates users via OAuth 2.0 (authorization\n  code + PKCE) fronted by Clerk.\nschemes:\n- id: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer orth_live_...'\n  key_prefixes:\n  - prefix: orth_live_\n    mode: live\n    note: production, billable\n  - prefix: orth_test_\n    mode: test\n    note: testing, no charges\n  env_var: ORTHOGONAL_API_KEY\n  applies_to:\n  - REST API (api.orthogonal.com)\n  - CLI (@orth/cli)\n  - SDKs (@orth/sdk, orth)\n- id: oauth2\n  type: oauth2\n  flow: authorization_code\n  pkce: S256\n  issuer: https://clerk.orthogonal.com\n  authorization_endpoint: https://clerk.orthogonal.com/oauth/authorize\n  token_endpoint: https://clerk.orthogonal.com/oauth/token\n\
  \  revocation_endpoint: https://clerk.orthogonal.com/oauth/token/revoke\n  registration_endpoint: https://mcp.orthogonal.com/oauth/register\n  jwks_uri: https://clerk.orthogonal.com/.well-known/jwks.json\n  applies_to:\n  - Hosted MCP server (mcp.orthogonal.com)\n  scopes:\n  - openid\n  - profile\n  - email\n  - public_metadata\n  - private_metadata\n  - offline_access\n  - user:org:read\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orthogonal/refs/heads/main/authentication/orthogonal-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI Agents
- API Discovery
- API Marketplace
- Agent Payments
- MCP
- Data Enrichment
- Crypto
- Stablecoins
---
