---
api_key_in: []
api_specs:
- filename: cometeer-storefront-openapi.yml
  format: yaml
  label: Cometeer Storefront (read-only)
  slug: storefront
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometeer/refs/heads/main/openapi/cometeer-storefront-openapi.yml
auth_types:
- none
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Cometeer Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: Cometeer secures its APIs with none, openIdConnect, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: Cometeer
provider_slug: cometeer
scheme_count: 3
schemes:
- authorization_endpoint: https://shopify.com/authentication/74101293355/oauth/authorize
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
  end_session_endpoint: https://shopify.com/authentication/74101293355/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/74101293355
  jwks_uri: https://shopify.com/authentication/74101293355/.well-known/jwks.json
  name: CometeerCustomerAccountOIDC
  openIdConnectUrl: https://cometeer.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/cometeer-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint: https://shopify.com/authentication/74101293355/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- metadata: https://cometeer.com/.well-known/oauth-authorization-server
  name: CometeerOAuthAuthorizationServer
  note: Byte-identical to the OIDC discovery document; the same Shopify Customer Account authorization server is advertised under both metadata standards.
  sources:
  - well-known/cometeer-oauth-authorization-server.json
  standard: RFC 8414
  type: oauth2
- name: UCPAgentProfile
  note: Not an OAuth/apiKey scheme. The UCP protocol requires the calling agent to publish a resolvable agent profile URI which the merchant fetches during JSON-RPC discovery. Observed failure mode recorded in mcp/cometeer-mcp.yml.
  scheme: ucp-agent-profile
  type: other
slug: cometeer-authentication
source_filename: cometeer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://cometeer.com/.well-known/openid-configuration\ndocs: https://cometeer.com/llms.txt\nsummary:\n  types: [none, openIdConnect, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken, jwt-bearer]\n  note: >-\n    Cometeer exposes three distinct surfaces with three distinct auth postures:\n    an anonymous read-only storefront, an OpenID Connect customer identity\n    provider (Shopify Customer Accounts), and a UCP/MCP commerce endpoint gated\n    on an agent profile rather than a bearer token.\nsurfaces:\n- id: storefront-read\n  name: Read-only storefront JSON\n  spec: openapi/cometeer-storefront-openapi.yml\n  auth: none\n  description: >-\n    Product, collection, search and sitemap endpoints are public and require no\n    credential. Cometeer documents them for agents under \"Read-Only Browsing\n    (No Authentication Required)\" in /llms.txt.\n- id: customer-account\n  name: Customer Account identity\
  \ (OpenID Connect)\n  auth: openIdConnect\n  description: >-\n    Shopify Customer Accounts, provisioned for Cometeer shop 74101293355 and\n    discoverable from Cometeer's own apex host. Intended for the shopper's own\n    account/subscription portal at https://account.cometeer.com/account, not for\n    third-party server-to-server integration.\n- id: ucp-mcp\n  name: UCP shopping MCP endpoint\n  auth: ucp-agent-profile\n  description: >-\n    https://cometeer.com/api/ucp/mcp rejects anonymous JSON-RPC calls with HTTP\n    422 / code -32001 `invalid_profile_url` until the calling agent presents a\n    resolvable UCP agent profile URI. Payment completion additionally requires\n    contemporaneous human buyer approval.\nschemes:\n- name: CometeerCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://cometeer.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/74101293355\n  authorization_endpoint: https://shopify.com/authentication/74101293355/oauth/authorize\n\
  \  token_endpoint: https://shopify.com/authentication/74101293355/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/74101293355/logout\n  jwks_uri: https://shopify.com/authentication/74101293355/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  code_challenge_methods_supported: [S256]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  scopes_supported: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  sources: [well-known/cometeer-openid-configuration.json]\n- name: CometeerOAuthAuthorizationServer\n  type: oauth2\n  metadata: https://cometeer.com/.well-known/oauth-authorization-server\n  standard: RFC 8414\n  note: >-\n    Byte-identical\
  \ to the OIDC discovery document; the same Shopify Customer\n    Account authorization server is advertised under both metadata standards.\n  sources: [well-known/cometeer-oauth-authorization-server.json]\n- name: UCPAgentProfile\n  type: other\n  scheme: ucp-agent-profile\n  note: >-\n    Not an OAuth/apiKey scheme. The UCP protocol requires the calling agent to\n    publish a resolvable agent profile URI which the merchant fetches during\n    JSON-RPC discovery. Observed failure mode recorded in mcp/cometeer-mcp.yml.\nrelated:\n  scopes: scopes/cometeer-scopes.yml\n  conventions: conventions/cometeer-conventions.yml\n  mcp: mcp/cometeer-mcp.yml\nx-evidence:\n- fetched: '2026-08-01'\n  url: https://cometeer.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n- fetched: '2026-08-01'\n  url: https://cometeer.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cometeer/refs/heads/main/authentication/cometeer-authentication.yml
summary_line: none/openIdConnect/oauth2 · 3 schemes
tags:
- Company
- Coffee
- Food and Beverage
- E-Commerce
- Direct to Consumer
- Retail
- Subscription
- Agentic Commerce
- Shopify
- MCP
---
