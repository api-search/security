---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Modcloth Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: Modcloth secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: Modcloth
provider_slug: modcloth
scheme_count: 2
schemes:
- authorization_endpoint: https://account.modcloth.com/authentication/oauth/authorize
  code_challenge_methods:
  - S256
  end_session_endpoint: https://account.modcloth.com/authentication/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/55906042027
  jwks_uri: https://account.modcloth.com/authentication/.well-known/jwks.json
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://modcloth.com/.well-known/openid-configuration
  response_types:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  source: well-known/modcloth-openid-configuration.json
  token_endpoint: https://account.modcloth.com/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
- endpoint: https://modcloth.com/api/ucp/mcp
  name: ucp-agent-commerce
  note: UCP shopping service. Catalog/cart operations are open; checkout completion requires contemporaneous buyer approval (human-in-the-loop).
  source: well-known/modcloth-ucp.json
  transport: mcp
  type: application
slug: modcloth-authentication
source_filename: modcloth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://modcloth.com/.well-known/openid-configuration\ndocs: https://modcloth.com/.well-known/oauth-authorization-server\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, refreshToken, jwt-bearer]\n  pkce: S256\n  notes: >-\n    Two distinct auth surfaces. (1) Agent commerce over UCP/MCP at\n    /api/ucp/mcp — public catalog/cart tools, buyer-approved checkout, agent\n    identity via a UCP profile URI. (2) Customer-account OAuth 2.0 / OpenID\n    Connect provided by Shopify (issuer https://shopify.com/authentication/55906042027)\n    for authenticated shopper sessions and the Customer Account API/MCP.\n    Read-only storefront JSON (products.json, collections) needs no auth.\nschemes:\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://modcloth.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/55906042027\n  authorization_endpoint:\
  \ https://account.modcloth.com/authentication/oauth/authorize\n  token_endpoint: https://account.modcloth.com/authentication/oauth/token\n  jwks_uri: https://account.modcloth.com/authentication/.well-known/jwks.json\n  end_session_endpoint: https://account.modcloth.com/authentication/logout\n  grant_types: [authorization_code, refresh_token, \"urn:ietf:params:oauth:grant-type:jwt-bearer\"]\n  response_types: [code]\n  token_endpoint_auth_methods: [client_secret_basic]\n  code_challenge_methods: [S256]\n  id_token_signing_alg: [RS256]\n  scopes_supported: [openid, email, \"customer-account-api:full\", \"customer-account-mcp-api:full\"]\n  source: well-known/modcloth-openid-configuration.json\n- name: ucp-agent-commerce\n  type: application\n  transport: mcp\n  endpoint: https://modcloth.com/api/ucp/mcp\n  note: >-\n    UCP shopping service. Catalog/cart operations are open; checkout\n    completion requires contemporaneous buyer approval (human-in-the-loop).\n  source: well-known/modcloth-ucp.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modcloth/refs/heads/main/authentication/modcloth-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Retail
- E-commerce
- Fashion
- Apparel
- Shopify
- Agentic Commerce
- MCP
---
