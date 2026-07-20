---
api_key_in: []
api_specs:
- filename: julep-beauty-storefront-openapi.yml
  format: yaml
  label: Julep Storefront Read-Only JSON API
  slug: storefront
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/julep-beauty/refs/heads/main/openapi/julep-beauty-storefront-openapi.yml
auth_types: []
description: Julep's storefront has two distinct authentication postures. The public read-only catalog surface requires no credentials at all. The customer-account surface is a full OpenID Connect deployment (Shopify Customer Accounts) whose discovery document is served on Julep's own domain, with the interactive endpoints branded on account.julep.com.
kind: authentication
layout: security
method: searched
name: Julep Beauty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Julep Beauty declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Julep Beauty
provider_slug: julep-beauty
scheme_count: 3
schemes:
- applies_to: Public storefront JSON (products.json, collections/*/products.json, products/{handle}.json, cart.js, search)
  description: The provider explicitly documents this surface as "Read-Only Browsing (No Authentication Required)" in /agents.md. Verified anonymously on 2026-07-19.
  evidence: https://www.julep.com/agents.md
  id: none
  type: none
- applies_to: Customer account (order history, profile, saved addresses)
  claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  code_challenge_methods_supported:
  - S256
  description: OpenID Connect authorization-code flow with PKCE. Discovery is also exposed as RFC 8414 authorization-server metadata at /.well-known/oauth-authorization-server (byte-identical at time of probe).
  endpoints:
    authorization: https://account.julep.com/authentication/oauth/authorize
    end_session: https://account.julep.com/authentication/logout
    jwks: https://account.julep.com/authentication/.well-known/jwks.json
    token: https://account.julep.com/authentication/oauth/token
  files:
  - well-known/julep-beauty-openid-configuration.json
  - well-known/julep-beauty-oauth-authorization-server.json
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: customer-account-oidc
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/2228781091
  openIdConnectUrl: https://www.julep.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes: scopes/julep-beauty-scopes.yml
  subject_types_supported:
  - public
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- applies_to: UCP/MCP commerce endpoint (POST /api/ucp/mcp)
  description: 'The MCP endpoint does not accept anonymous callers. Probing tools/list without an agent identity returns JSON-RPC error -32001 "UCP discovery failed" with code invalid_profile_url and the message "Unable to fetch agent profile: Missing profile uri" — i.e. the caller must present a resolvable UCP agent profile URI. Payment additionally requires explicit, contemporaneous buyer approval.'
  evidence: https://www.julep.com/.well-known/ucp
  id: ucp-agent-profile
  probed: '2026-07-19'
  type: other
slug: julep-beauty-authentication
source_filename: julep-beauty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.julep.com/.well-known/openid-configuration\nname: Julep authentication profile\ndescription: >-\n  Julep's storefront has two distinct authentication postures. The public read-only\n  catalog surface requires no credentials at all. The customer-account surface is a\n  full OpenID Connect deployment (Shopify Customer Accounts) whose discovery document\n  is served on Julep's own domain, with the interactive endpoints branded on\n  account.julep.com.\ndocs: https://www.julep.com/agents.md\nschemes:\n- id: none\n  type: none\n  applies_to: Public storefront JSON (products.json, collections/*/products.json, products/{handle}.json, cart.js, search)\n  description: >-\n    The provider explicitly documents this surface as \"Read-Only Browsing (No\n    Authentication Required)\" in /agents.md. Verified anonymously on 2026-07-19.\n  evidence: https://www.julep.com/agents.md\n- id: customer-account-oidc\n  type: openIdConnect\n\
  \  openIdConnectUrl: https://www.julep.com/.well-known/openid-configuration\n  applies_to: Customer account (order history, profile, saved addresses)\n  description: >-\n    OpenID Connect authorization-code flow with PKCE. Discovery is also exposed as\n    RFC 8414 authorization-server metadata at /.well-known/oauth-authorization-server\n    (byte-identical at time of probe).\n  issuer: https://shopify.com/authentication/2228781091\n  endpoints:\n    authorization: https://account.julep.com/authentication/oauth/authorize\n    token: https://account.julep.com/authentication/oauth/token\n    end_session: https://account.julep.com/authentication/logout\n    jwks: https://account.julep.com/authentication/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n \
  \ id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  scopes: scopes/julep-beauty-scopes.yml\n  files:\n  - well-known/julep-beauty-openid-configuration.json\n  - well-known/julep-beauty-oauth-authorization-server.json\n- id: ucp-agent-profile\n  type: other\n  applies_to: UCP/MCP commerce endpoint (POST /api/ucp/mcp)\n  description: >-\n    The MCP endpoint does not accept anonymous callers. Probing tools/list without an\n    agent identity returns JSON-RPC error -32001 \"UCP discovery failed\" with code\n    invalid_profile_url and the message \"Unable to fetch agent profile: Missing profile\n    uri\" — i.e. the caller must present a resolvable UCP agent profile URI. Payment\n    additionally requires explicit, contemporaneous buyer approval.\n  evidence: https://www.julep.com/.well-known/ucp\n  probed: '2026-07-19'\nnotes:\n- Julep publishes no developer portal, no API\
  \ keys, and no partner/server-to-server\n  credential program of its own; all machine access is either anonymous storefront JSON\n  or platform-mediated (Shopify Customer Accounts OIDC, UCP agent profiles).\n- No RFC 9116 security.txt is published (404 on 2026-07-19).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/julep-beauty/refs/heads/main/authentication/julep-beauty-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Beauty
- Cosmetics
- Skincare
- Retail
- E-Commerce
- Direct to Consumer
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
---
