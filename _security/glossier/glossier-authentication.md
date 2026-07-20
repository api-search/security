---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Glossier Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Glossier secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Glossier
provider_slug: glossier
scheme_count: 2
schemes:
- authorization_endpoint: https://account.glossier.com/authentication/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://account.glossier.com/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/62791647477
  jwks_uri: https://account.glossier.com/authentication/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://www.glossier.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/glossier-openid-configuration.json
  - well-known/glossier-oauth-authorization-server.json
  token_endpoint: https://account.glossier.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- description: The UCP MCP endpoint requires an agent profile URI before enumerating tools.
  name: UCPAgentProfile
  scheme: ucp-agent-profile
  sources:
  - well-known/glossier-ucp.json
  type: apiKey
slug: glossier-authentication
source_filename: glossier-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.glossier.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  pkce: S256\n  note: >-\n    Customer-facing authentication is delegated to the Shopify Customer Account\n    authorization server (issuer https://shopify.com/authentication/62791647477,\n    endpoints on account.glossier.com). The storefront's agent-commerce (UCP/MCP)\n    surface is separately gated by a UCP agent-profile identity check.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://www.glossier.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/62791647477\n  authorization_endpoint: https://account.glossier.com/authentication/oauth/authorize\n  token_endpoint: https://account.glossier.com/authentication/oauth/token\n  end_session_endpoint: https://account.glossier.com/authentication/logout\n\
  \  jwks_uri: https://account.glossier.com/authentication/.well-known/jwks.json\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  id_token_signing_alg_values_supported:\n  - RS256\n  sources:\n  - well-known/glossier-openid-configuration.json\n  - well-known/glossier-oauth-authorization-server.json\n- name: UCPAgentProfile\n  type: apiKey\n  scheme: ucp-agent-profile\n  description: The UCP MCP endpoint requires an agent profile URI before enumerating tools.\n  sources:\n  - well-known/glossier-ucp.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glossier/refs/heads/main/authentication/glossier-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Consumer
- Beauty
- Cosmetics
- Ecommerce
- Retail
- Agent Commerce
- Universal Commerce Protocol
- Shopify
- MCP
---
