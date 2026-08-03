---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- custom-header
description: ''
kind: authentication
layout: security
method: probed
name: Bombas Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: Bombas secures its APIs with oauth2, openIdConnect, and custom-header across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: Bombas
provider_slug: bombas
scheme_count: 3
schemes:
- description: URL to the calling platform's UCP profile document. Required on every UCP Shopping Service call; an anonymous call returns JSON-RPC error -32001 "UCP discovery failed" with data.code invalid_profile_url.
  format: uri
  in: header
  json_rpc_param: meta.ucp-agent.profile
  name: ucp-agent
  parameter_name: UCP-Agent
  required: true
  sources:
  - mcp/bombas-ucp-shopping-2026-04-08.openrpc.json
  type: custom-header
- authorizationUrl: https://shopify.com/authentication/11195850/oauth/authorize
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
  end_session_endpoint: https://shopify.com/authentication/11195850/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/11195850
  jwks_uri: https://shopify.com/authentication/11195850/.well-known/jwks.json
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://shop.bombas.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/bombas-openid-configuration.json
  subject_types_supported:
  - public
  tokenUrl: https://shopify.com/authentication/11195850/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- identical_to: shopify-customer-account-oidc
  metadata_url: https://shop.bombas.com/.well-known/oauth-authorization-server
  name: shopify-oauth-authorization-server
  rfc: RFC 8414
  sources:
  - well-known/bombas-oauth-authorization-server.json
  type: oauth2
slug: bombas-authentication
source_filename: bombas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: https://shop.bombas.com/.well-known/openid-configuration\ndocs: https://shop.bombas.com/agents.md\nsummary:\n  types: [oauth2, openIdConnect, custom-header]\n  oauth2_flows: [authorizationCode, refreshToken, jwt-bearer]\n  pkce: [S256]\n  api_key_in: []\n  note: >-\n    Bombas publishes no first-party developer API and issues no API keys. Two\n    distinct auth models were observed on the storefront host. (1) The UCP /\n    MCP commerce endpoint is not OAuth-gated for discovery; it requires a\n    UCP-Agent identity header carrying the calling platform's own UCP profile\n    URI, and it defers payment authorization to the buyer. (2) Shopify customer\n    accounts on the same host publish full OAuth 2.0 / OpenID Connect discovery.\nschemes:\n- name: ucp-agent\n  type: custom-header\n  in: header\n  parameter_name: UCP-Agent\n  json_rpc_param: meta.ucp-agent.profile\n  required: true\n  format: uri\n  description: >-\n    URL to\
  \ the calling platform's UCP profile document. Required on every UCP\n    Shopping Service call; an anonymous call returns JSON-RPC error -32001\n    \"UCP discovery failed\" with data.code invalid_profile_url.\n  sources: [mcp/bombas-ucp-shopping-2026-04-08.openrpc.json]\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://shop.bombas.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/11195850\n  authorizationUrl: https://shopify.com/authentication/11195850/oauth/authorize\n  tokenUrl: https://shopify.com/authentication/11195850/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/11195850/logout\n  jwks_uri: https://shopify.com/authentication/11195850/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  code_challenge_methods_supported:\
  \ [S256]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  sources: [well-known/bombas-openid-configuration.json]\n- name: shopify-oauth-authorization-server\n  type: oauth2\n  rfc: RFC 8414\n  metadata_url: https://shop.bombas.com/.well-known/oauth-authorization-server\n  identical_to: shopify-customer-account-oidc\n  sources: [well-known/bombas-oauth-authorization-server.json]\nprotected_resource:\n  rfc: RFC 9728\n  metadata_url: https://shop.bombas.com/.well-known/oauth-protected-resource\n  resource: https://shop.bombas.com\n  authorization_servers: [https://shopify.com/authentication/11195850]\n  bearer_methods_supported: [header]\n  sources: [well-known/bombas-oauth-protected-resource.json]\nnot_found:\n- {path: /.well-known/security.txt, host: shop.bombas.com, status: 404}\n\
  - {note: 'no api.bombas.com or developer.bombas.com host resolves in DNS'}\nx-evidence:\n  fetched: '2026-07-31'\n  urls:\n  - {url: 'https://shop.bombas.com/.well-known/openid-configuration', http_status: 200}\n  - {url: 'https://shop.bombas.com/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://shop.bombas.com/.well-known/oauth-protected-resource', http_status: 200}\n  - {url: 'https://shop.bombas.com/api/ucp/mcp', http_status: 422, note: 'anonymous tools/list rejected'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bombas/refs/heads/main/authentication/bombas-authentication.yml
summary_line: oauth2/openIdConnect/custom-header · 3 schemes
tags:
- Company
- Retail
- Ecommerce
- Apparel
- Direct to Consumer
- Commerce
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
---
