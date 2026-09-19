---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication profile for the surfaces reachable from the G2 Track record. G2 Track is operated by BetterCloud (acquired 2024-03-12, sold as BetterCloud Spend Optimization); there is no G2 Track-specific authentication surface, so what is recorded here is the operator's. Two distinct schemes are in play and they are not interchangeable.
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: G2 Track Authentication
name_suffix: Authentication
oauth_flows: []
overview: G2 Track declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: G2 Track
provider_slug: g2-track
scheme_count: 2
schemes:
- applies_to: https://api.bettercloud.com/api
  description: The BetterCloud platform API authenticates with a tenant-issued API token. The published contract exposes GET /v1/tokens/lookup (operationId ValidateApiToken) purely to check a token is valid. The published OpenAPI declares NO components.securitySchemes and no top-level security[], so the scheme is documented in prose and in the token-lookup operation rather than in the contract itself - a real gap in the operator's spec.
  evidence:
  - body: '{"message":"No API key found in request"}'
    status: 401
    url: https://api.bettercloud.com/api/graphql
  - body: '{"message":"No API key found in request"}'
    status: 401
    url: https://api.bettercloud.com/api-docs
  gated: true
  id: bettercloud-api-token
  in: header
  name: Authorization
  type: apiKey
- applies_to: https://www.bettercloud.com/wp-json/mcp/mcp-oauth-server
  authorization_endpoint: https://www.bettercloud.com/oauth/authorize
  description: An OAuth 2.0 authorization server published at the operator's web host per RFC 8414, protecting the MCP resource described in mcp/g2-track-mcp.yml. Public client (token_endpoint_auth_methods "none") with mandatory PKCE S256, authorization_code + refresh_token grants, a single scope `mcp`, and client registration by client_id metadata document rather than RFC 7591 DCR.
  evidence:
  - status: 200
    url: https://www.bettercloud.com/.well-known/oauth-authorization-server
  - status: 200
    url: https://www.bettercloud.com/.well-known/oauth-protected-resource
  flow: authorization_code
  id: bettercloud-site-mcp-oauth
  pkce:
  - S256
  revocation_endpoint: https://www.bettercloud.com/oauth/revoke
  scopes:
  - description: The only scope the authorization server advertises.
    id: mcp
  token_endpoint: https://www.bettercloud.com/oauth/token
  type: oauth2
slug: g2-track-authentication
source_filename: g2-track-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: >-\n  https://www.bettercloud.com/.well-known/oauth-authorization-server +\n  https://developer.bettercloud.com/assets/docs/BetterCloudAPI.OpenApi3.json (operator's published\n  contract, read but not copied into this repo - see note)\nprovider: G2 Track\nproviderId: g2-track\ndescription: >-\n  Authentication profile for the surfaces reachable from the G2 Track record. G2 Track is operated\n  by BetterCloud (acquired 2024-03-12, sold as BetterCloud Spend Optimization); there is no G2\n  Track-specific authentication surface, so what is recorded here is the operator's. Two distinct\n  schemes are in play and they are not interchangeable.\nschemes:\n- id: bettercloud-api-token\n  type: apiKey\n  in: header\n  name: Authorization\n  applies_to: https://api.bettercloud.com/api\n  description: >-\n    The BetterCloud platform API authenticates with a tenant-issued API token. The published\n    contract exposes GET /v1/tokens/lookup\
  \ (operationId ValidateApiToken) purely to check a token is\n    valid. The published OpenAPI declares NO components.securitySchemes and no top-level security[],\n    so the scheme is documented in prose and in the token-lookup operation rather than in the\n    contract itself - a real gap in the operator's spec.\n  evidence:\n  - url: https://api.bettercloud.com/api/graphql\n    status: 401\n    body: '{\"message\":\"No API key found in request\"}'\n  - url: https://api.bettercloud.com/api-docs\n    status: 401\n    body: '{\"message\":\"No API key found in request\"}'\n  gated: true\n- id: bettercloud-site-mcp-oauth\n  type: oauth2\n  flow: authorization_code\n  applies_to: https://www.bettercloud.com/wp-json/mcp/mcp-oauth-server\n  description: >-\n    An OAuth 2.0 authorization server published at the operator's web host per RFC 8414, protecting\n    the MCP resource described in mcp/g2-track-mcp.yml. Public client (token_endpoint_auth_methods\n    \"none\") with mandatory PKCE S256,\
  \ authorization_code + refresh_token grants, a single scope\n    `mcp`, and client registration by client_id metadata document rather than RFC 7591 DCR.\n  authorization_endpoint: https://www.bettercloud.com/oauth/authorize\n  token_endpoint: https://www.bettercloud.com/oauth/token\n  revocation_endpoint: https://www.bettercloud.com/oauth/revoke\n  scopes:\n  - id: mcp\n    description: The only scope the authorization server advertises.\n  pkce:\n  - S256\n  evidence:\n  - url: https://www.bettercloud.com/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://www.bettercloud.com/.well-known/oauth-protected-resource\n    status: 200\nopenid_connect: false\nmutual_tls: false\nnote: >-\n  The BetterCloud OpenAPI 3.0.0 that documents the api-token scheme lives at\n  https://developer.bettercloud.com/assets/docs/BetterCloudAPI.OpenApi3.json and says of itself\n  info.title \"BetterCloud API\", servers https://api.bettercloud.com/api. It is the OPERATOR's\n  contract and\
  \ covers the platform (authentication, error docs, GraphQL reporting, automation) - it\n  carries no Spend Optimization / G2 Track operations - so it belongs to all/bettercloud/ and was\n  deliberately NOT copied into this product record.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/g2-track/refs/heads/main/authentication/g2-track-authentication.yml
summary_line: 2 schemes
tags:
- Contract Management
- SaaS Management
- Spend Optimization
- Shadow IT
- License Management
- Software Asset Management
- IT Operations
---
