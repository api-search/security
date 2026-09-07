---
anonymous_access: true
api_key_in: []
auth_types:
- none
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Acefouraccessories Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Acefour Accessories secures its APIs with none, openIdConnect, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Acefour Accessories
provider_slug: acefouraccessories
scheme_count: 3
schemes:
- caller_identification:
    detail: Every tool inputSchema requires meta.ucp-agent.profile, an agent profile URI used for UCP agent discovery. It identifies the calling agent but is not a credential and is not verified as one.
    format: uri
    parameter: meta.ucp-agent.profile
    required: true
  detail: tools/list and the catalog tools answered with no Authorization header (HTTP 200). No API key, bearer token or client registration is required to call the agent surface.
  endpoint: https://uppercase.co.in/api/ucp/mcp
  name: ucp-mcp-anonymous
  plane: agent commerce (UCP shopping MCP)
  type: none
  verified: probed
- authorization_endpoint: https://shopify.com/authentication/67539140858/oauth/authorize
  code_challenge_methods_supported:
  - S256
  detail: Discovery is served from the company's own host but the issuer, keys and consent screens are Shopify's, scoped to shop id 67539140858. See scopes/acefouraccessories-scopes.yml.
  end_session_endpoint: https://shopify.com/authentication/67539140858/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/67539140858
  jwks_uri: https://shopify.com/authentication/67539140858/.well-known/jwks.json
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://uppercase.co.in/.well-known/openid-configuration
  plane: buyer identity / customer accounts
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  token_endpoint: https://shopify.com/authentication/67539140858/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  verified: probed
- detail: RFC 9728 metadata at /.well-known/oauth-protected-resource names resource https://uppercase.co.in with bearer_methods_supported ["header"], pointing at the Shopify issuer as the sole authorization server. No bearer token was needed for any call this pass actually made.
  name: ucp-protected-resource
  plane: resource metadata
  type: oauth2
  verified: probed
slug: acefouraccessories-authentication
source_filename: acefouraccessories-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: >-\n  https://uppercase.co.in/api/ucp/mcp (anonymous tools/list, HTTP 200),\n  https://uppercase.co.in/.well-known/openid-configuration,\n  https://uppercase.co.in/.well-known/oauth-protected-resource\nnote: >-\n  There is no OpenAPI to derive securitySchemes from, so this profile was probed directly against the\n  live surfaces. Two distinct auth planes exist and they are not the same thing: the agent commerce\n  plane is anonymous, and the buyer/customer-account plane is OIDC on a Shopify-operated issuer.\nsummary:\n  types: [none, openIdConnect, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: ucp-mcp-anonymous\n  plane: agent commerce (UCP shopping MCP)\n  type: none\n  endpoint: https://uppercase.co.in/api/ucp/mcp\n  detail: >-\n    tools/list and the catalog tools answered with no Authorization header (HTTP 200). No API key,\n    bearer token or client registration is required to call the\
  \ agent surface.\n  caller_identification:\n    required: true\n    parameter: meta.ucp-agent.profile\n    format: uri\n    detail: >-\n      Every tool inputSchema requires meta.ucp-agent.profile, an agent profile URI used for UCP\n      agent discovery. It identifies the calling agent but is not a credential and is not verified\n      as one.\n  verified: probed\n- name: shopify-customer-account-oidc\n  plane: buyer identity / customer accounts\n  type: openIdConnect\n  openIdConnectUrl: https://uppercase.co.in/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/67539140858\n  authorization_endpoint: https://shopify.com/authentication/67539140858/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/67539140858/oauth/token\n  jwks_uri: https://shopify.com/authentication/67539140858/.well-known/jwks.json\n  end_session_endpoint: https://shopify.com/authentication/67539140858/logout\n  id_token_signing_alg_values_supported: [RS256]\n  code_challenge_methods_supported:\
  \ [S256]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  scopes_supported:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  detail: >-\n    Discovery is served from the company's own host but the issuer, keys and consent screens are\n    Shopify's, scoped to shop id 67539140858. See scopes/acefouraccessories-scopes.yml.\n  verified: probed\n- name: ucp-protected-resource\n  plane: resource metadata\n  type: oauth2\n  detail: >-\n    RFC 9728 metadata at /.well-known/oauth-protected-resource names\n    resource https://uppercase.co.in with bearer_methods_supported [\"header\"], pointing at the\n    Shopify issuer as the sole authorization server. No bearer token was needed for any call this\n    pass actually made.\n  verified: probed\npayment_authorization:\n  detail: >-\n    Payment is\
  \ authorized out of band by the buyer, not by an API credential. /llms.txt states\n    agents must not complete payment without explicit buyer consent, and points agents that cannot\n    obtain contemporaneous approval at Shop Pay instead.\n  handlers: [com.google.pay, dev.shopify.card]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acefouraccessories/refs/heads/main/authentication/acefouraccessories-authentication.yml
summary_line: none/openIdConnect/oauth2 · 3 schemes
tags:
- Company
- Retail
- E-Commerce
- Consumer Goods
- Travel
- Luggage
- Direct to Consumer
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- India
---
