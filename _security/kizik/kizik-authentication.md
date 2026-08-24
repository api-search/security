---
api_key_in: []
auth_types: []
description: 'Kizik exposes two distinct authentication postures: the agent commerce surface is anonymous at discovery time, and customer identity is OpenID Connect.'
kind: authentication
layout: security
method: probed
name: Kizik Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kizik declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Kizik
provider_slug: kizik
scheme_count: 4
schemes:
- description: 'MCP tools/list is served anonymously. Probed 2026-08-23: HTTP 200, no WWW-Authenticate header, no OAuth challenge, no API key required to enumerate the 13 tools and their input schemas.'
  evidence:
    http_status: 200
    url: https://kizik.com/api/ucp/mcp
  id: none
  surface: https://kizik.com/api/ucp/mcp
  type: none
- description: 'Every tool invocation requires meta.ucp-agent.profile — a URI pointing at the calling agent''s own published UCP agent profile. This is caller identification rather than authorization: the agent asserts who it is by publishing a resolvable profile document. Omitting it returns JSON-RPC error -32001 with data.code invalid_profile_url.'
  evidence:
    probe: tools/call search_catalog with empty arguments
    response: '{"code":-32001,"message":"UCP discovery failed","data":{"code":"invalid_profile_url"}}'
  id: ucp-agent-profile
  required: true
  surface: https://kizik.com/api/ucp/mcp
  type: caller-identity
- authorization_endpoint: https://shopify.com/authentication/22811461/oauth/authorize
  claims:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  code_challenge_methods:
  - S256
  description: Shopify customer accounts for the Kizik store, discoverable at /.well-known/openid-configuration on kizik.com. Authorization code flow with PKCE (S256), refresh tokens, and a JWT bearer grant.
  end_session_endpoint: https://shopify.com/authentication/22811461/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: openid-connect
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/22811461
  jwks_uri: https://shopify.com/authentication/22811461/.well-known/jwks.json
  openid_configuration: https://kizik.com/.well-known/openid-configuration
  response_types:
  - code
  scopes_artifact: scopes/kizik-scopes.yml
  surface: customer accounts
  token_endpoint: https://shopify.com/authentication/22811461/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
- description: Product JSON documents are served without credentials.
  id: read-only-storefront
  surface: https://kizik.com/products.json
  type: none
slug: kizik-authentication
source_filename: kizik-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: https://kizik.com/.well-known/openid-configuration + probed https://kizik.com/api/ucp/mcp\ndocs: https://kizik.com/agents.md\ndescription: >-\n  Kizik exposes two distinct authentication postures: the agent commerce surface is anonymous at\n  discovery time, and customer identity is OpenID Connect.\nschemes:\n- id: none\n  type: none\n  surface: https://kizik.com/api/ucp/mcp\n  description: >-\n    MCP tools/list is served anonymously. Probed 2026-08-23: HTTP 200, no WWW-Authenticate header, no\n    OAuth challenge, no API key required to enumerate the 13 tools and their input schemas.\n  evidence:\n    url: https://kizik.com/api/ucp/mcp\n    http_status: 200\n- id: ucp-agent-profile\n  type: caller-identity\n  surface: https://kizik.com/api/ucp/mcp\n  description: >-\n    Every tool invocation requires meta.ucp-agent.profile — a URI pointing at the calling agent's own\n    published UCP agent profile. This is caller identification\
  \ rather than authorization: the agent\n    asserts who it is by publishing a resolvable profile document. Omitting it returns JSON-RPC error\n    -32001 with data.code invalid_profile_url.\n  required: true\n  evidence:\n    probe: 'tools/call search_catalog with empty arguments'\n    response: '{\"code\":-32001,\"message\":\"UCP discovery failed\",\"data\":{\"code\":\"invalid_profile_url\"}}'\n- id: openid-connect\n  type: openIdConnect\n  surface: customer accounts\n  description: >-\n    Shopify customer accounts for the Kizik store, discoverable at /.well-known/openid-configuration on\n    kizik.com. Authorization code flow with PKCE (S256), refresh tokens, and a JWT bearer grant.\n  issuer: https://shopify.com/authentication/22811461\n  openid_configuration: https://kizik.com/.well-known/openid-configuration\n  authorization_endpoint: https://shopify.com/authentication/22811461/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/22811461/oauth/token\n  end_session_endpoint:\
  \ https://shopify.com/authentication/22811461/logout\n  jwks_uri: https://shopify.com/authentication/22811461/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  response_types: [code]\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg: [RS256]\n  claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  scopes_artifact: scopes/kizik-scopes.yml\n- id: read-only-storefront\n  type: none\n  surface: https://kizik.com/products.json\n  description: Product JSON documents are served without credentials.\npayment_authorization:\n  human_in_the_loop: required\n  note: >-\n    Payment completion is not an authentication scheme Kizik grants to agents at all. Both robots.txt and\n    /agents.md require an explicit, contemporaneous human approval step before any checkout completes.\nnotes:\n- No API keys, no bearer tokens\
  \ and no mutual TLS are used on the public agent surface.\n- The OIDC issuer is a Shopify-operated host, but the discovery document is served from kizik.com and is\n  scoped to Kizik's shop (22811461); it authenticates Kizik customers, not Shopify staff.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kizik/refs/heads/main/authentication/kizik-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Retail
- E-Commerce
- Footwear
- Consumer Goods
- Agent Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- Direct to Consumer
---
