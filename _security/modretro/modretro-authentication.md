---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
- http
description: ''
kind: authentication
layout: security
method: probed
name: Modretro Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- urn:ietf:params:oauth:grant-type:jwt-bearer
overview: ModRetro secures its APIs with openIdConnect, oauth2, and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and urn:ietf:params:oauth:grant-type:jwt-bearer flow(s).
provider_name: ModRetro
provider_slug: modretro
scheme_count: 3
schemes:
- authorization_endpoint: https://orders.modretro.com/authentication/oauth/authorize
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
  end_session_endpoint: https://orders.modretro.com/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/82920341806
  jwks_uri: https://orders.modretro.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://modretro.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/modretro-openid-configuration.json
  token_endpoint: https://orders.modretro.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
- applies_to:
  - get_order
  - create_checkout
  - update_checkout
  - complete_checkout
  - cancel_checkout
  bearerFormat: JWT
  docs: https://shopify.dev/docs/agents/get-started/authentication
  evidence: 'POST tools/call get_order without a token returned HTTP 403 and JSON-RPC -32000 "AuthenticationRequired: Unauthorized: A valid JWT is required to call get_order."'
  name: ShopifyAgentJWT
  scheme: bearer
  sources:
  - mcp/modretro-mcp.yml
  type: http
- evidence: A tools/call without a resolvable profile URI returns HTTP 422 and JSON-RPC -32001 "UCP discovery failed" with data.code invalid_profile_url.
  mechanism: meta.ucp-agent.profile (fetchable agent-profile URI on every tools/call)
  name: UCPAgentProfile
  required: true
  sources:
  - mcp/modretro-mcp-tools.json
  type: other
slug: modretro-authentication
source_filename: modretro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://modretro.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/agents/get-started/authentication\nnote: >-\n  ModRetro publishes no OpenAPI, so this profile is built from the two authentication surfaces the\n  company actually serves: the OIDC / RFC 8414 discovery documents at modretro.com/.well-known/ and\n  the live authentication behaviour observed on the UCP MCP endpoint. Both are shop-scoped to\n  ModRetro (issuer https://shopify.com/authentication/82920341806; endpoints on orders.modretro.com).\n\nsummary:\n  types: [openIdConnect, oauth2, http]\n  oauth2_flows: [authorizationCode, refreshToken, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  pkce: [S256]\n  api_key_in: []\n  anonymous_surfaces:\n    - 'MCP initialize and tools/list (HTTP 200, no credentials)'\n    - 'Storefront product/collection JSON (GET /products.json, /collections/{handle}/products.json)'\n    - 'Atom blog feed (/blogs/blog.atom)'\n\
  \nschemes:\n  - name: ShopifyCustomerAccountOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://modretro.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/82920341806\n    authorization_endpoint: https://orders.modretro.com/authentication/oauth/authorize\n    token_endpoint: https://orders.modretro.com/authentication/oauth/token\n    end_session_endpoint: https://orders.modretro.com/authentication/logout\n    jwks_uri: https://orders.modretro.com/authentication/.well-known/jwks.json\n    response_types_supported: [code]\n    grant_types_supported: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n    token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n    code_challenge_methods_supported: [S256]\n    id_token_signing_alg_values_supported: [RS256]\n    claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n    scopes_supported: [openid, email, 'customer-account-api:full',\
  \ 'customer-account-mcp-api:full']\n    sources: [well-known/modretro-openid-configuration.json]\n  - name: ShopifyAgentJWT\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    applies_to: [get_order, create_checkout, update_checkout, complete_checkout, cancel_checkout]\n    docs: https://shopify.dev/docs/agents/get-started/authentication\n    evidence: >-\n      POST tools/call get_order without a token returned HTTP 403 and JSON-RPC -32000\n      \"AuthenticationRequired: Unauthorized: A valid JWT is required to call get_order.\"\n    sources: [mcp/modretro-mcp.yml]\n  - name: UCPAgentProfile\n    type: other\n    mechanism: 'meta.ucp-agent.profile (fetchable agent-profile URI on every tools/call)'\n    required: true\n    evidence: >-\n      A tools/call without a resolvable profile URI returns HTTP 422 and JSON-RPC -32001\n      \"UCP discovery failed\" with data.code invalid_profile_url.\n    sources: [mcp/modretro-mcp-tools.json]\n\nx-evidence:\n  - {url: 'https://modretro.com/.well-known/openid-configuration',\
  \ http_status: 200, fetched: '2026-08-26'}\n  - {url: 'https://modretro.com/.well-known/oauth-authorization-server', http_status: 200, fetched: '2026-08-26'}\n  - {url: 'https://orders.modretro.com/authentication/.well-known/jwks.json', http_status: 200, fetched: '2026-08-26'}\n  - {url: 'https://modretro.com/api/ucp/mcp', http_status: 403, fetched: '2026-08-26', note: 'AuthenticationRequired on get_order'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modretro/refs/heads/main/authentication/modretro-authentication.yml
summary_line: openIdConnect/oauth2/http · 3 schemes
tags:
- Company
- Consumer Electronics
- Gaming
- Retro Gaming
- Hardware
- E-Commerce
- Agentic Commerce
- Model Context Protocol
- Universal Commerce Protocol
- Open Source Hardware
---
