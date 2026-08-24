---
api_key_in: []
auth_types:
- none
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Hero Bread Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Hero Bread secures its APIs with none, http, oauth2, and openIdConnect across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Hero Bread
provider_slug: hero-bread
scheme_count: 5
schemes:
- applies_to:
  - POST https://shop.hero.co/api/ucp/mcp — initialize
  - POST https://shop.hero.co/api/ucp/mcp — tools/list
  - POST https://shop.hero.co/api/mcp — tools/list
  evidence: 'probed 2026-08-22: HTTP 200 with no Authorization header, 13 tools returned'
  name: mcp-anonymous-discovery
  type: none
- description: Every tools/call must carry a resolvable UCP agent profile URI in meta.ucp-agent.profile. A missing or unreachable profile fails discovery before authentication is even evaluated.
  evidence: 'probed 2026-08-22: omitting it returns -32001 UCP discovery failed / invalid_profile_url'
  in: request-body
  name: ucp-agent-profile
  parameter: meta.ucp-agent.profile
  required: true
  scheme: none
  type: http
- bearerFormat: JWT
  description: Transactional MCP tool calls require a Shopify-issued agent JWT. The server names the instructions in the error payload itself.
  docs: https://shopify.dev/docs/agents/get-started/authentication
  evidence: 'probed 2026-08-22: tools/call without a token returns -32000 "AuthenticationRequired" — "Unauthorized: A valid JWT is required to call <tool>."'
  name: shopify-agent-jwt
  scheme: bearer
  type: http
- discovery: well-known/hero-bread-oauth-authorization-server.json
  flows:
  - authorizationUrl: https://shopify.com/authentication/56010965185/oauth/authorize
    flow: authorizationCode
    scopes:
      customer-account-api:full: Full access to the customer account API
      customer-account-mcp-api:full: Full access to the customer account MCP API
      email: Buyer email address
      openid: OpenID Connect authentication
    tokenUrl: https://shopify.com/authentication/56010965185/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  name: shopify-customer-accounts-oauth2
  pkce: S256
  source: https://shop.hero.co/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
- discovery: well-known/hero-bread-openid-configuration.json
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/56010965185
  jwks_uri: https://shopify.com/authentication/56010965185/.well-known/jwks.json
  name: shopify-customer-accounts-oidc
  openIdConnectUrl: https://shop.hero.co/.well-known/openid-configuration
  type: openIdConnect
slug: hero-bread-authentication
source_filename: hero-bread-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://shop.hero.co/.well-known/oauth-authorization-server\ndocs: https://shopify.dev/docs/agents/get-started/authentication\nnote: >-\n  Hero Bread publishes no OpenAPI, so this profile is built from live probes of the discovery\n  documents and MCP endpoint on shop.hero.co rather than from securitySchemes. Two distinct auth\n  postures are in play: the MCP commerce surface (anonymous discovery, JWT-bearing agent calls) and\n  Shopify customer accounts (OAuth 2.0 / OIDC).\nsummary:\n  types: [none, http, oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: mcp-anonymous-discovery\n  type: none\n  applies_to:\n  - 'POST https://shop.hero.co/api/ucp/mcp — initialize'\n  - 'POST https://shop.hero.co/api/ucp/mcp — tools/list'\n  - 'POST https://shop.hero.co/api/mcp — tools/list'\n  evidence: 'probed 2026-08-22: HTTP 200 with no Authorization header, 13 tools returned'\n- name: ucp-agent-profile\n\
  \  type: http\n  scheme: none\n  in: request-body\n  parameter: meta.ucp-agent.profile\n  required: true\n  description: >-\n    Every tools/call must carry a resolvable UCP agent profile URI in meta.ucp-agent.profile. A\n    missing or unreachable profile fails discovery before authentication is even evaluated.\n  evidence: 'probed 2026-08-22: omitting it returns -32001 UCP discovery failed / invalid_profile_url'\n- name: shopify-agent-jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Transactional MCP tool calls require a Shopify-issued agent JWT. The server names the\n    instructions in the error payload itself.\n  docs: https://shopify.dev/docs/agents/get-started/authentication\n  evidence: >-\n    probed 2026-08-22: tools/call without a token returns -32000 \"AuthenticationRequired\" —\n    \"Unauthorized: A valid JWT is required to call <tool>.\"\n- name: shopify-customer-accounts-oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://shopify.com/authentication/56010965185/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/56010965185/oauth/token\n    scopes:\n      openid: OpenID Connect authentication\n      email: Buyer email address\n      customer-account-api:full: Full access to the customer account API\n      customer-account-mcp-api:full: Full access to the customer account MCP API\n  pkce: S256\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  discovery: well-known/hero-bread-oauth-authorization-server.json\n  source: https://shop.hero.co/.well-known/oauth-authorization-server\n- name: shopify-customer-accounts-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://shop.hero.co/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/56010965185\n  jwks_uri: https://shopify.com/authentication/56010965185/.well-known/jwks.json\n  id_token_signing_alg_values_supported:\
  \ [RS256]\n  discovery: well-known/hero-bread-openid-configuration.json\nprotected_resource:\n  resource: https://shop.hero.co\n  authorization_servers: [https://shopify.com/authentication/56010965185]\n  bearer_methods_supported: [header]\n  source: https://shop.hero.co/.well-known/oauth-protected-resource\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hero-bread/refs/heads/main/authentication/hero-bread-authentication.yml
summary_line: none/http/oauth2/openIdConnect · 5 schemes
tags:
- Company
- Food and Beverage
- Consumer Packaged Goods
- Retail
- E-Commerce
- Agent Commerce
- Model Context Protocol
- Universal Commerce Protocol
- Shopify
- Direct to Consumer
---
