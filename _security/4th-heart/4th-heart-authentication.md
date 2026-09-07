---
anonymous_access: true
api_key_in: []
auth_types:
- none
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: 4Th Heart Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwtBearer
overview: 4th & Heart secures its APIs with none, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwtBearer flow(s).
provider_name: 4th & Heart
provider_slug: 4th-heart
scheme_count: 4
schemes:
- applies_to: https://fourthandheart.com/api/ucp/mcp
  description: The UCP MCP endpoint accepts JSON-RPC tools/list and initialize with no credential of any kind. Verified anonymously, HTTP 200.
  name: mcp-anonymous
  sources:
  - https://fourthandheart.com/api/ucp/mcp
  type: none
- applies_to: tools/call
  description: Every tools/call carries a meta object with a ucp-agent.profile URI identifying the calling agent. It is an identity assertion the server dereferences, not a secret. Omitting it returns JSON-RPC error -32001 with data.code invalid_profile_url.
  in: body
  name: ucp-agent-profile
  parameter_name: meta.ucp-agent.profile
  required: true
  sources:
  - mcp/4th-heart-mcp-tools.json
  type: agent-identity
- applies_to: customer accounts and the customer-account MCP API
  description: Shopify Customer Accounts, published on the merchant's own domain and scoped to shop id 6414473.
  issuer: https://shopify.com/authentication/6414473
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://fourthandheart.com/.well-known/openid-configuration
  sources:
  - well-known/4th-heart-openid-configuration.json
  type: openIdConnect
- authorizationUrl: https://shopify.com/authentication/6414473/oauth/authorize
  bearer_methods_supported:
  - header
  end_session_endpoint: https://shopify.com/authentication/6414473/logout
  flows:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  jwks_uri: https://shopify.com/authentication/6414473/.well-known/jwks.json
  name: shopify-customer-account-oauth2
  pkce:
  - S256
  sources:
  - well-known/4th-heart-oauth-authorization-server.json
  - well-known/4th-heart-oauth-protected-resource.json
  tokenUrl: https://shopify.com/authentication/6414473/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: 4th-heart-authentication
source_filename: 4th-heart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://fourthandheart.com/.well-known/openid-configuration\ndocs: https://fourthandheart.com/agents.md\nnote: >-\n  Derived from probed discovery documents rather than an OpenAPI, because 4th & Heart publishes no\n  OpenAPI. Two distinct auth surfaces exist and they are not the same thing: the agent-commerce MCP\n  server is anonymous, while the customer account surface is OAuth 2.0 / OpenID Connect operated by\n  Shopify on the merchant's behalf.\nsummary:\n  types: [none, oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken, jwtBearer]\nschemes:\n- name: mcp-anonymous\n  type: none\n  applies_to: https://fourthandheart.com/api/ucp/mcp\n  description: >-\n    The UCP MCP endpoint accepts JSON-RPC tools/list and initialize with no credential of any kind.\n    Verified anonymously, HTTP 200.\n  sources: [https://fourthandheart.com/api/ucp/mcp]\n- name: ucp-agent-profile\n  type: agent-identity\n\
  \  in: body\n  parameter_name: meta.ucp-agent.profile\n  required: true\n  applies_to: tools/call\n  description: >-\n    Every tools/call carries a meta object with a ucp-agent.profile URI identifying the calling\n    agent. It is an identity assertion the server dereferences, not a secret. Omitting it returns\n    JSON-RPC error -32001 with data.code invalid_profile_url.\n  sources: [mcp/4th-heart-mcp-tools.json]\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://fourthandheart.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/6414473\n  applies_to: customer accounts and the customer-account MCP API\n  description: >-\n    Shopify Customer Accounts, published on the merchant's own domain and scoped to shop id 6414473.\n  sources: [well-known/4th-heart-openid-configuration.json]\n- name: shopify-customer-account-oauth2\n  type: oauth2\n  authorizationUrl: https://shopify.com/authentication/6414473/oauth/authorize\n\
  \  tokenUrl: https://shopify.com/authentication/6414473/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/6414473/logout\n  jwks_uri: https://shopify.com/authentication/6414473/.well-known/jwks.json\n  flows: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  pkce: [S256]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  id_token_signing_alg: [RS256]\n  bearer_methods_supported: [header]\n  sources:\n  - well-known/4th-heart-oauth-authorization-server.json\n  - well-known/4th-heart-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4th-heart/refs/heads/main/authentication/4th-heart-authentication.yml
summary_line: none/oauth2/openIdConnect · 4 schemes
tags:
- Company
- Food and Beverage
- Consumer Packaged Goods
- Retail
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
- Direct to Consumer
---
