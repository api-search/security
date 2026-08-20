---
api_key_in: []
auth_types:
- none
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Bespoken Spirits Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- urn:ietf:params:oauth:grant-type:jwt-bearer
overview: Bespoken Spirits secures its APIs with none, openIdConnect, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and urn:ietf:params:oauth:grant-type:jwt-bearer flow(s).
provider_name: Bespoken Spirits
provider_slug: bespoken-spirits
scheme_count: 4
schemes:
- description: Storefront catalog JSON (/products.json, /products/{handle}.json, /collections/{handle}/products.json) and MCP initialize + tools/list on both endpoints require no credential of any kind.
  name: anonymous
  sources:
  - https://bespokenspirits.com/llms.txt
  - https://bespokenspirits.com/api/ucp/mcp
  type: none
- description: JSON-RPC params.meta.ucp-agent.profile — a URI pointing at the calling agent's own UCP profile. Required on every tools/call; absent it the server returns JSON-RPC -32001 with data.code invalid_profile_url. Not a bearer token and not issued by Bespoken Spirits.
  in: json-rpc params
  name: ucp-agent-profile
  parameter: meta.ucp-agent.profile
  required: true
  sources:
  - mcp/bespoken-spirits-ucp-mcp-tools.json
  type: agent-identity
- authorizationUrl: https://shopify.com/authentication/75681399024/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/75681399024/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/75681399024
  jwks_uri: https://shopify.com/authentication/75681399024/.well-known/jwks.json
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://bespokenspirits.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes: scopes/bespoken-spirits-scopes.yml
  sources:
  - well-known/bespoken-spirits-openid-configuration.json
  tokenUrl: https://shopify.com/authentication/75681399024/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- authorization_servers:
  - https://shopify.com/authentication/75681399024
  bearer_methods_supported:
  - header
  description: RFC 9728 protected-resource metadata declaring bespokenspirits.com as the resource, the Shopify authentication host as its authorization server, and header-borne bearer tokens as the only supported presentation method.
  name: shopify-oauth-protected-resource
  resource: https://bespokenspirits.com
  sources:
  - well-known/bespoken-spirits-oauth-protected-resource.json
  type: oauth2
slug: bespoken-spirits-authentication
source_filename: bespoken-spirits-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: searched\nsource: https://bespokenspirits.com/.well-known/openid-configuration\ndocs: https://bespokenspirits.com/agents.md\nnotes: >-\n  Bespoken Spirits publishes no API keys and no developer program. Its machine surface\n  splits into three auth postures: (1) fully anonymous read — the storefront product\n  JSON endpoints and MCP initialize/tools/list; (2) agent-profile-bound — every\n  tools/call on the UCP MCP endpoint requires a caller-hosted UCP agent profile URI in\n  meta.ucp-agent.profile, which is a discovery identity rather than a bearer credential;\n  (3) OIDC/OAuth 2.0 — the Shopify Customer Account authorization server, used for\n  buyer accounts and for the customer-account MCP API. Payment on complete_checkout\n  additionally requires contemporaneous human buyer approval, which is an authorization\n  gate the protocol enforces rather than a credential.\nsummary:\n  types:\n  - none\n  - openIdConnect\n  - oauth2\n  api_key_in:\
  \ []\n  oauth2_flows:\n  - authorizationCode\n  - refreshToken\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\nschemes:\n- name: anonymous\n  type: none\n  description: Storefront catalog JSON (/products.json, /products/{handle}.json,\n    /collections/{handle}/products.json) and MCP initialize + tools/list on both\n    endpoints require no credential of any kind.\n  sources:\n  - https://bespokenspirits.com/llms.txt\n  - https://bespokenspirits.com/api/ucp/mcp\n- name: ucp-agent-profile\n  type: agent-identity\n  description: JSON-RPC params.meta.ucp-agent.profile — a URI pointing at the calling\n    agent's own UCP profile. Required on every tools/call; absent it the server returns\n    JSON-RPC -32001 with data.code invalid_profile_url. Not a bearer token and not\n    issued by Bespoken Spirits.\n  in: json-rpc params\n  parameter: meta.ucp-agent.profile\n  required: true\n  sources:\n  - mcp/bespoken-spirits-ucp-mcp-tools.json\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n\
  \  openIdConnectUrl: https://bespokenspirits.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/75681399024\n  authorizationUrl: https://shopify.com/authentication/75681399024/oauth/authorize\n  tokenUrl: https://shopify.com/authentication/75681399024/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/75681399024/logout\n  jwks_uri: https://shopify.com/authentication/75681399024/.well-known/jwks.json\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  code_challenge_methods_supported:\n  - S256\n  id_token_signing_alg_values_supported:\n  - RS256\n  scopes: scopes/bespoken-spirits-scopes.yml\n  sources:\n  - well-known/bespoken-spirits-openid-configuration.json\n- name: shopify-oauth-protected-resource\n  type: oauth2\n  description: RFC 9728 protected-resource\
  \ metadata declaring bespokenspirits.com as\n    the resource, the Shopify authentication host as its authorization server, and\n    header-borne bearer tokens as the only supported presentation method.\n  resource: https://bespokenspirits.com\n  authorization_servers:\n  - https://shopify.com/authentication/75681399024\n  bearer_methods_supported:\n  - header\n  sources:\n  - well-known/bespoken-spirits-oauth-protected-resource.json\nx-evidence:\n  fetched: '2026-08-07'\n  probes:\n  - url: https://bespokenspirits.com/.well-known/openid-configuration\n    http_status: 200\n  - url: https://bespokenspirits.com/.well-known/oauth-protected-resource\n    http_status: 200\n  - url: https://bespokenspirits.com/api/ucp/mcp\n    http_status: 200\n    note: tools/call without meta.ucp-agent.profile returns -32001 invalid_profile_url\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bespoken-spirits/refs/heads/main/authentication/bespoken-spirits-authentication.yml
summary_line: none/openIdConnect/oauth2 · 4 schemes
tags:
- Company
- Spirits
- Beverage Alcohol
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- Retail
- Manufacturing
---
