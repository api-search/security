---
anonymous_access: true
api_key_in: []
auth_types:
- none
- oauth2
- openIdConnect
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: Underdog Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Underdog secures its APIs with none, oauth2, openIdConnect, and http across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Underdog
provider_slug: underdog
scheme_count: 5
schemes:
- applies_to:
  - https://underdog.shop/api/ucp/mcp (initialize, tools/list)
  - https://underdog.shop/api/mcp
  - https://underdog.shop/api/2026-01/graphql.json
  - https://underdog.shop/products.json
  evidence: probed 2026-09-16, HTTP 200 with no Authorization header
  name: anonymous-discovery
  type: none
- description: Agent profile URI the merchant fetches for UCP capability negotiation; required on every UCP tool.
  evidence: mcp/underdog-ucp-mcp-tools.json (meta.required includes ucp-agent); tools/call with an unreachable profile returned HTTP 422, code -32001
  location: JSON-RPC params.arguments.meta.ucp-agent.profile
  name: ucp-agent-profile
  type: none
- applies_to:
  - get_order
  bearerFormat: JWT
  docs: https://shopify.dev/docs/agents/get-started/authentication
  evidence: tools/call get_order returned HTTP 403, JSON-RPC -32000 AuthenticationRequired, 2026-09-16
  name: shopify-agent-jwt
  scheme: bearer
  type: http
- authorization_servers:
  - https://account.underdog.shop
  - https://shopify.com/authentication/69142905142
  bearer_methods_supported:
  - header
  flows:
  - authorizationUrl: https://account.underdog.shop/authentication/oauth/authorize
    code_challenge_methods_supported:
    - S256
    endSessionEndpoint: https://account.underdog.shop/authentication/logout
    flow: authorizationCode
    grant_types_supported:
    - authorization_code
    - refresh_token
    - urn:ietf:params:oauth:grant-type:jwt-bearer
    issuer: https://shopify.com/authentication/69142905142
    jwksUri: https://account.underdog.shop/authentication/.well-known/jwks.json
    scopes:
    - openid
    - email
    - customer-account-api:full
    - customer-account-mcp-api:full
    tokenUrl: https://account.underdog.shop/authentication/oauth/token
    token_endpoint_auth_methods_supported:
    - client_secret_basic
    - client_secret_post
  name: shopify-customer-account-oauth2
  protected_resources:
  - https://underdog.shop
  - https://account.underdog.shop
  scheme: bearer
  sources:
  - well-known/underdog-openid-configuration.json
  - well-known/underdog-oauth-authorization-server.json
  - well-known/underdog-oauth-protected-resource.json
  - well-known/underdog-account-oauth-protected-resource.json
  type: oauth2
- claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  id_token_signing_alg_values_supported:
  - RS256
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://underdog.shop/.well-known/openid-configuration
  sources:
  - well-known/underdog-openid-configuration.json
  subject_types_supported:
  - public
  type: openIdConnect
slug: underdog-authentication
source_filename: underdog-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: probed\nsource: >-\n  https://underdog.shop/.well-known/openid-configuration,\n  https://underdog.shop/.well-known/oauth-authorization-server,\n  https://underdog.shop/.well-known/oauth-protected-resource,\n  https://account.underdog.shop/.well-known/oauth-protected-resource,\n  https://underdog.shop/api/ucp/mcp and https://underdog.shop/api/2026-01/graphql.json (anonymous probes)\nnote: >-\n  Underdog runs no developer programme and issues no API keys. Three auth postures exist\n  on its host and should not be conflated. (1) Discovery on the agent/storefront surfaces is\n  anonymous: MCP initialize and tools/list on /api/ucp/mcp and /api/mcp, Storefront GraphQL\n  introspection and product/shop queries, and /products.json all answered HTTP 200 with no\n  credentials on 2026-09-16. (2) UCP tools/call requires the calling agent to identify\n  itself with meta.ucp-agent.profile, a reachable UCP agent profile URI (an unreachable\n  profile returned\
  \ -32001 \"UCP discovery failed\"), and get_order returned -32000\n  AuthenticationRequired \"A valid JWT is required\", pointing at\n  https://shopify.dev/docs/agents/get-started/authentication. Payment additionally requires\n  contemporaneous human buyer approval (agents.md). (3) Shopper accounts use OAuth 2.0\n  authorization code + PKCE against Shopify customer accounts, discovered from metadata\n  served on Underdog's own hosts (issuer shopify.com/authentication/69142905142).\ndocs: https://underdog.shop/agents.md\nsummary:\n  types: [none, oauth2, openIdConnect, http]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  agent_surface_auth: none (discovery); UCP agent profile + JWT for some tool calls\n  human_approval_required_for: [complete_checkout]\nschemes:\n- name: anonymous-discovery\n  type: none\n  applies_to:\n  - https://underdog.shop/api/ucp/mcp (initialize, tools/list)\n  - https://underdog.shop/api/mcp\n  - https://underdog.shop/api/2026-01/graphql.json\n  - https://underdog.shop/products.json\n\
  \  evidence: probed 2026-09-16, HTTP 200 with no Authorization header\n- name: ucp-agent-profile\n  type: none\n  location: JSON-RPC params.arguments.meta.ucp-agent.profile\n  description: Agent profile URI the merchant fetches for UCP capability negotiation; required on every UCP tool.\n  evidence: mcp/underdog-ucp-mcp-tools.json (meta.required includes ucp-agent); tools/call with an unreachable profile returned HTTP 422, code -32001\n- name: shopify-agent-jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applies_to: [get_order]\n  evidence: tools/call get_order returned HTTP 403, JSON-RPC -32000 AuthenticationRequired, 2026-09-16\n  docs: https://shopify.dev/docs/agents/get-started/authentication\n- name: shopify-customer-account-oauth2\n  type: oauth2\n  scheme: bearer\n  bearer_methods_supported: [header]\n  flows:\n  - flow: authorizationCode\n    issuer: https://shopify.com/authentication/69142905142\n    authorizationUrl: https://account.underdog.shop/authentication/oauth/authorize\n\
  \    tokenUrl: https://account.underdog.shop/authentication/oauth/token\n    jwksUri: https://account.underdog.shop/authentication/.well-known/jwks.json\n    endSessionEndpoint: https://account.underdog.shop/authentication/logout\n    code_challenge_methods_supported: [S256]\n    token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n    grant_types_supported: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n    scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  protected_resources: [https://underdog.shop, https://account.underdog.shop]\n  authorization_servers: [https://account.underdog.shop, https://shopify.com/authentication/69142905142]\n  sources:\n  - well-known/underdog-openid-configuration.json\n  - well-known/underdog-oauth-authorization-server.json\n  - well-known/underdog-oauth-protected-resource.json\n  - well-known/underdog-account-oauth-protected-resource.json\n- name: shopify-customer-account-oidc\n\
  \  type: openIdConnect\n  openIdConnectUrl: https://underdog.shop/.well-known/openid-configuration\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  sources: [well-known/underdog-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/underdog/refs/heads/main/authentication/underdog-authentication.yml
summary_line: none/oauth2/openIdConnect/http · 5 schemes
tags:
- Company
- Climate Tech
- Circular Economy
- Refurbished Electronics
- Home Appliances
- Retail
- E-Commerce
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- GraphQL
- France
---
