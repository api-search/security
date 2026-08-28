---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: M Gemi Authentication
name_suffix: Authentication
oauth_flows: []
overview: M.Gemi declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: M.Gemi
provider_slug: m-gemi
scheme_count: 2
schemes:
- description: Every UCP MCP tool declares a required `meta.ucp-agent.profile` field - a URI pointing at the calling agent's UCP profile document. It is a discovery/identity handle, not a secret. tools/list and initialize succeed without it; a tools/call without it returns JSON-RPC error -32001 "UCP discovery failed" with data.code invalid_profile_url.
  id: ucp-agent-profile
  in: request-body
  observed: probed 2026-08-25
  parameter: meta.ucp-agent.profile
  surface: https://mgemi.com/api/ucp/mcp
  type: other
- authorization_endpoint: https://shopify.com/authentication/13666484283/oauth/authorize
  description: Shopify Customer Account API OIDC discovery, served on M.Gemi's own store host and scoped to M.Gemi's shop tenant. Governs customer sign-in at https://mgemi.com/account/login.
  end_session_endpoint: https://shopify.com/authentication/13666484283/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify-customer-account-oidc
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/13666484283
  jwks_uri: https://shopify.com/authentication/13666484283/.well-known/jwks.json
  openid_connect_url: https://mgemi.com/.well-known/openid-configuration
  pkce:
  - S256
  response_types:
  - code
  scopes: scopes/m-gemi-scopes.yml
  surface: https://mgemi.com/.well-known/openid-configuration
  token_endpoint: https://shopify.com/authentication/13666484283/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
slug: m-gemi-authentication
source_filename: m-gemi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://mgemi.com/.well-known/openid-configuration + live probes of https://mgemi.com/api/ucp/mcp\ndocs: https://mgemi.com/agents.md\nsummary: >-\n  M.Gemi publishes no API-key program. Two distinct auth models are observable on the\n  store host: an anonymous/profile-scoped model on the UCP MCP commerce endpoint, and a\n  Shopify Customer Account OpenID Connect model for customer identity.\nschemes:\n- id: ucp-agent-profile\n  type: other\n  surface: https://mgemi.com/api/ucp/mcp\n  in: request-body\n  parameter: meta.ucp-agent.profile\n  description: >-\n    Every UCP MCP tool declares a required `meta.ucp-agent.profile` field - a URI pointing\n    at the calling agent's UCP profile document. It is a discovery/identity handle, not a\n    secret. tools/list and initialize succeed without it; a tools/call without it returns\n    JSON-RPC error -32001 \"UCP discovery failed\" with data.code invalid_profile_url.\n  observed: probed\
  \ 2026-08-25\n- id: shopify-customer-account-oidc\n  type: openIdConnect\n  surface: https://mgemi.com/.well-known/openid-configuration\n  openid_connect_url: https://mgemi.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/13666484283\n  authorization_endpoint: https://shopify.com/authentication/13666484283/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/13666484283/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/13666484283/logout\n  jwks_uri: https://shopify.com/authentication/13666484283/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types:\n  - code\n  pkce:\n  - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg:\n  - RS256\n  scopes: scopes/m-gemi-scopes.yml\n  description: >-\n    Shopify Customer Account API OIDC discovery, served on M.Gemi's own store\
  \ host and\n    scoped to M.Gemi's shop tenant. Governs customer sign-in at\n    https://mgemi.com/account/login.\nbuyer_approval:\n  required: true\n  scope: checkout completion\n  statement: >-\n    \"Checkout requires human approval. Agents must not complete payment without explicit\n    buyer consent.\"\n  source: https://mgemi.com/llms.txt\nno_api_keys:\n  finding: true\n  note: >-\n    No developer portal, no key issuance page and no API-key header were found on any\n    M.Gemi host. The commerce surface is reached through UCP agent profiles and buyer\n    approval rather than issued credentials.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/m-gemi/refs/heads/main/authentication/m-gemi-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Retail
- E-Commerce
- Fashion
- Footwear
- Direct to Consumer
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
- Catalog
- Checkout
---
