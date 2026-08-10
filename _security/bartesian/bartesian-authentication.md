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
name: Bartesian Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: Bartesian secures its APIs with oauth2, openIdConnect, and custom-header across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: Bartesian
provider_slug: bartesian
scheme_count: 3
schemes:
- applies_to: tool execution (tools/call), resources/list
  description: 'URL to the calling platform''s UCP profile document. Required on every UCP Shopping Service tool invocation - `meta.ucp-agent` is in the required list of all 13 published tool schemas. An anonymous tools/call returns HTTP 422 with JSON-RPC error -32001 "UCP discovery failed" and data.code invalid_profile_url. It is NOT required to read the contract: tools/list returns all 13 tools and their full inputSchemas without it.'
  does_not_apply_to:
  - initialize
  - tools/list
  format: uri
  in: header
  json_rpc_param: meta.ucp-agent.profile
  name: ucp-agent
  parameter_name: UCP-Agent
  required: true
  sources:
  - mcp/bartesian-ucp-shopping-tools.json
  type: custom-header
- authorizationUrl: https://shopify.com/authentication/3860496433/oauth/authorize
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
  end_session_endpoint: https://shopify.com/authentication/3860496433/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/3860496433
  jwks_uri: https://shopify.com/authentication/3860496433/.well-known/jwks.json
  name: shopify-customer-account-oidc
  op_policy_uri: https://www.shopify.com/legal/privacy
  op_tos_uri: https://www.shopify.com/legal/terms
  openIdConnectUrl: https://bartesian.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/bartesian-openid-configuration.json
  subject_types_supported:
  - public
  tokenUrl: https://shopify.com/authentication/3860496433/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- identical_to: shopify-customer-account-oidc
  metadata_url: https://bartesian.com/.well-known/oauth-authorization-server
  name: shopify-oauth-authorization-server
  note: byte-identical document to the OIDC discovery response
  rfc: RFC 8414
  sources:
  - well-known/bartesian-oauth-authorization-server.json
  type: oauth2
slug: bartesian-authentication
source_filename: bartesian-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://bartesian.com/.well-known/openid-configuration\ndocs: https://bartesian.com/agents.md\nsummary:\n  types: [oauth2, openIdConnect, custom-header]\n  oauth2_flows: [authorizationCode, refreshToken, jwt-bearer]\n  pkce: [S256]\n  api_key_in: []\n  note: >-\n    Bartesian publishes no first-party developer API and issues no API keys. Two\n    distinct auth models were observed on the storefront host. (1) The UCP / MCP\n    commerce endpoint leaves DISCOVERY entirely open - anonymous initialize and\n    tools/list both return 200 - and gates only EXECUTION, requiring a UCP-Agent\n    identity header carrying the calling platform's own UCP profile URI, with\n    payment authorization deferred to the buyer. (2) Shopify customer accounts on\n    the same host publish full OAuth 2.0 / OpenID Connect discovery.\nschemes:\n- name: ucp-agent\n  type: custom-header\n  in: header\n  parameter_name: UCP-Agent\n  json_rpc_param: meta.ucp-agent.profile\n\
  \  required: true\n  format: uri\n  applies_to: tool execution (tools/call), resources/list\n  does_not_apply_to: [initialize, tools/list]\n  description: >-\n    URL to the calling platform's UCP profile document. Required on every UCP\n    Shopping Service tool invocation - `meta.ucp-agent` is in the required list\n    of all 13 published tool schemas. An anonymous tools/call returns HTTP 422\n    with JSON-RPC error -32001 \"UCP discovery failed\" and data.code\n    invalid_profile_url. It is NOT required to read the contract: tools/list\n    returns all 13 tools and their full inputSchemas without it.\n  sources: [mcp/bartesian-ucp-shopping-tools.json]\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://bartesian.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/3860496433\n  authorizationUrl: https://shopify.com/authentication/3860496433/oauth/authorize\n  tokenUrl: https://shopify.com/authentication/3860496433/oauth/token\n\
  \  end_session_endpoint: https://shopify.com/authentication/3860496433/logout\n  jwks_uri: https://shopify.com/authentication/3860496433/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  code_challenge_methods_supported: [S256]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  op_policy_uri: https://www.shopify.com/legal/privacy\n  op_tos_uri: https://www.shopify.com/legal/terms\n  sources: [well-known/bartesian-openid-configuration.json]\n- name: shopify-oauth-authorization-server\n  type: oauth2\n  rfc: RFC 8414\n  metadata_url: https://bartesian.com/.well-known/oauth-authorization-server\n  identical_to:\
  \ shopify-customer-account-oidc\n  note: byte-identical document to the OIDC discovery response\n  sources: [well-known/bartesian-oauth-authorization-server.json]\nprotected_resource:\n  rfc: RFC 9728\n  metadata_url: https://bartesian.com/.well-known/oauth-protected-resource\n  resource: https://bartesian.com\n  authorization_servers: [https://shopify.com/authentication/3860496433]\n  bearer_methods_supported: [header]\n  sources: [well-known/bartesian-oauth-protected-resource.json]\npayment_authorization:\n  model: buyer-approved\n  rule: >-\n    complete_checkout must not be called without contemporaneous buyer approval\n    of the payment. Bartesian states this as a hard rule in its own agents.md.\n  handlers: [shop_pay, shopify.card, gpay]\n  agent_never_handles_card: true\nnot_found:\n- {path: /.well-known/security.txt, host: bartesian.com, status: 404}\n- {path: /.well-known/api-catalog, host: bartesian.com, status: 404}\n- {note: 'no api.bartesian.com, developer.bartesian.com or\
  \ docs.bartesian.com host\n    resolves'}\nx-evidence:\n  fetched: '2026-08-06'\n  urls:\n  - {url: 'https://bartesian.com/.well-known/openid-configuration', http_status: 200}\n  - {url: 'https://bartesian.com/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://bartesian.com/.well-known/oauth-protected-resource', http_status: 200}\n  - {url: 'https://bartesian.com/api/ucp/mcp', http_status: 200, note: 'anonymous tools/list\n      ACCEPTED - 13 tools returned'}\n  - {url: 'https://bartesian.com/api/ucp/mcp', http_status: 422, note: 'anonymous tools/call\n      rejected - UCP-Agent profile required'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bartesian/refs/heads/main/authentication/bartesian-authentication.yml
summary_line: oauth2/openIdConnect/custom-header · 3 schemes
tags:
- Company
- Retail
- Ecommerce
- Consumer Products
- Appliances
- Beverages
- Direct to Consumer
- Commerce
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
---
