---
api_key_in: []
auth_types:
- none
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Flying Embers Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwtBearer
overview: Flying Embers secures its APIs with none, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwtBearer flow(s).
provider_name: Flying Embers
provider_slug: flying-embers
scheme_count: 2
schemes:
- description: 'No Authorization header is required to POST JSON-RPC to the UCP shopping MCP endpoint. Verified: an anonymous tools/list returned HTTP 200 with 13 tools.'
  name: ucp-mcp-anonymous
  required_request_metadata:
  - description: Agent profile URI used for UCP agent discovery. Required on every tool call.
    field: meta.ucp-agent.profile
    type: string (uri)
  - description: Required on complete_checkout only.
    field: meta.idempotency-key
    type: string
  sources:
  - mcp/flying-embers-mcp-tools-list.json
  surface: https://www.flyingembers.com/api/ucp/mcp
  type: none
- authorization_endpoint: https://shopify.com/authentication/35263676475/oauth/authorize
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
  description: Customer-account authentication for the storefront. The discovery document is served from the merchant's own domain; the issuer is the Shopify platform IdP scoped to this merchant's shop id (35263676475).
  end_session_endpoint: https://shopify.com/authentication/35263676475/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/35263676475
  jwks_uri: https://shopify.com/authentication/35263676475/.well-known/jwks.json
  login_page: https://www.flyingembers.com/account/login
  name: shopify-customer-accounts-oidc
  openIdConnectUrl: https://www.flyingembers.com/.well-known/openid-configuration
  pkce_methods:
  - S256
  response_types:
  - code
  sources:
  - well-known/flying-embers-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/35263676475/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: flying-embers-authentication
source_filename: flying-embers-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: https://www.flyingembers.com/.well-known/openid-configuration\ndocs: https://www.flyingembers.com/llms.txt\nsummary:\n  types: [none, oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken, jwtBearer]\n  note: >-\n    Two distinct surfaces with two distinct auth postures. The agent-facing UCP/MCP\n    commerce endpoint is ANONYMOUS — tools/list and read-only catalog calls succeed with\n    no credential. Customer account access uses OIDC/OAuth 2.0 with PKCE against a\n    store-scoped issuer. Payment on complete_checkout is gated by an out-of-band human\n    approval requirement, not by an API credential.\n\nschemes:\n  - name: ucp-mcp-anonymous\n    type: none\n    surface: https://www.flyingembers.com/api/ucp/mcp\n    description: >-\n      No Authorization header is required to POST JSON-RPC to the UCP shopping MCP\n      endpoint. Verified: an anonymous tools/list returned HTTP 200 with\
  \ 13 tools.\n    required_request_metadata:\n      - field: meta.ucp-agent.profile\n        type: string (uri)\n        description: Agent profile URI used for UCP agent discovery. Required on every tool call.\n      - field: meta.idempotency-key\n        type: string\n        description: Required on complete_checkout only.\n    sources: [mcp/flying-embers-mcp-tools-list.json]\n\n  - name: shopify-customer-accounts-oidc\n    type: openIdConnect\n    openIdConnectUrl: https://www.flyingembers.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/35263676475\n    authorization_endpoint: https://shopify.com/authentication/35263676475/oauth/authorize\n    token_endpoint: https://shopify.com/authentication/35263676475/oauth/token\n    end_session_endpoint: https://shopify.com/authentication/35263676475/logout\n    jwks_uri: https://shopify.com/authentication/35263676475/.well-known/jwks.json\n    grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n\
  \    response_types: [code]\n    token_endpoint_auth_methods: [client_secret_basic]\n    pkce_methods: [S256]\n    id_token_signing_alg: [RS256]\n    claims: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n    login_page: https://www.flyingembers.com/account/login\n    description: >-\n      Customer-account authentication for the storefront. The discovery document is served\n      from the merchant's own domain; the issuer is the Shopify platform IdP scoped to this\n      merchant's shop id (35263676475).\n    sources: [well-known/flying-embers-openid-configuration.json]\n\npayment_authorization:\n  model: human-in-the-loop\n  rule: >-\n    The merchant's own /llms.txt and /robots.txt state that agents must not complete\n    checkout, payment or order placement without an explicit, contemporaneous human\n    approval step. Buyer approval is the authorization gate on complete_checkout.\n  alternative: https://shop.app/SKILL.md\n  sources:\n    - https://www.flyingembers.com/llms.txt\n\
  \    - https://www.flyingembers.com/robots.txt\n\nx-evidence:\n  - {url: 'https://www.flyingembers.com/.well-known/openid-configuration', http_status: 200}\n  - {url: 'https://www.flyingembers.com/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://www.flyingembers.com/api/ucp/mcp', http_status: 200, note: anonymous POST tools/list}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flying-embers/refs/heads/main/authentication/flying-embers-authentication.yml
summary_line: none/oauth2/openIdConnect · 2 schemes
tags:
- Company
- Commerce
- E-Commerce
- Retail
- Beverages
- Consumer Packaged Goods
- Agentic Commerce
- MCP
- Shopify
- Direct to Consumer
---
