---
api_key_in: []
auth_types:
- none
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Oishii Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- urn:ietf:params:oauth:grant-type:jwt-bearer
overview: Oishii secures its APIs with none, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and urn:ietf:params:oauth:grant-type:jwt-bearer flow(s).
provider_name: Oishii
provider_slug: oishii
scheme_count: 4
schemes:
- description: The storefront MCP server (POST https://oishii.com/api/mcp) and the storefront JSON feeds (/products.json, /collections/{handle}/products.json, /products/{handle}.json) answer without any credential. tools/list, search_catalog, get_product_details and search_shop_policies_and_faqs were all reachable anonymously.
  name: anonymous-storefront
  sources:
  - https://oishii.com/api/mcp
  - https://oishii.com/agents.md
  type: none
- description: The UCP commerce endpoint (POST https://oishii.com/api/ucp/mcp) requires the calling agent to present a profile URI (meta.ucp-agent.profile). Without it the server returns HTTP 422 with JSON-RPC error -32001 invalid_profile_url. This is an agent-identity gate, not an end-user credential.
  name: ucp-agent-profile
  sources:
  - https://oishii.com/api/ucp/mcp
  - https://oishii.com/.well-known/ucp
  type: agent-identity
- authorization_endpoint: https://shopify.com/authentication/26346881082/oauth/authorize
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
  end_session_endpoint: https://shopify.com/authentication/26346881082/logout
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/26346881082
  jwks_uri: https://shopify.com/authentication/26346881082/.well-known/jwks.json
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://oishii.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/oishii-openid-configuration.json
  - well-known/oishii-oauth-authorization-server.json
  token_endpoint: https://shopify.com/authentication/26346881082/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- authorization_servers:
  - https://shopify.com/authentication/26346881082
  bearer_methods_supported:
  - header
  description: RFC 9728 protected-resource metadata declares https://oishii.com as an OAuth-protected resource whose authorization server is the Shopify customer-account issuer, with bearer tokens carried in the Authorization header.
  name: shopify-protected-resource
  resource: https://oishii.com
  sources:
  - well-known/oishii-oauth-protected-resource.json
  type: oauth2
slug: oishii-authentication
source_filename: oishii-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://oishii.com/.well-known/openid-configuration\ndocs: https://oishii.com/agents.md\nnote: >-\n  Oishii publishes no OpenAPI, so this profile is built from the live discovery documents served on the\n  oishii.com host plus the observed behaviour of the two MCP endpoints. Identity is delegated to the\n  Shopify customer-account issuer; the anonymous storefront read surface requires no credentials at all.\nsummary:\n  types:\n  - none\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - refreshToken\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  bearer_methods:\n  - header\n  pkce: S256\nschemes:\n- name: anonymous-storefront\n  type: none\n  description: >-\n    The storefront MCP server (POST https://oishii.com/api/mcp) and the storefront JSON feeds\n    (/products.json, /collections/{handle}/products.json, /products/{handle}.json) answer without any\n    credential. tools/list, search_catalog,\
  \ get_product_details and search_shop_policies_and_faqs were all\n    reachable anonymously.\n  sources:\n  - https://oishii.com/api/mcp\n  - https://oishii.com/agents.md\n- name: ucp-agent-profile\n  type: agent-identity\n  description: >-\n    The UCP commerce endpoint (POST https://oishii.com/api/ucp/mcp) requires the calling agent to present\n    a profile URI (meta.ucp-agent.profile). Without it the server returns HTTP 422 with JSON-RPC error\n    -32001 invalid_profile_url. This is an agent-identity gate, not an end-user credential.\n  sources:\n  - https://oishii.com/api/ucp/mcp\n  - https://oishii.com/.well-known/ucp\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://oishii.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/26346881082\n  authorization_endpoint: https://shopify.com/authentication/26346881082/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/26346881082/oauth/token\n  end_session_endpoint:\
  \ https://shopify.com/authentication/26346881082/logout\n  jwks_uri: https://shopify.com/authentication/26346881082/.well-known/jwks.json\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  response_types_supported:\n  - code\n  id_token_signing_alg_values_supported:\n  - RS256\n  code_challenge_methods_supported:\n  - S256\n  claims_supported:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - nonce\n  - sid\n  - email\n  - email_verified\n  scopes:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  sources:\n  - well-known/oishii-openid-configuration.json\n  - well-known/oishii-oauth-authorization-server.json\n- name: shopify-protected-resource\n  type: oauth2\n  description: >-\n    RFC 9728 protected-resource metadata declares https://oishii.com as an OAuth-protected resource whose\n    authorization server is the Shopify customer-account issuer, with bearer tokens carried in the\n    Authorization header.\n  resource: https://oishii.com\n\
  \  authorization_servers:\n  - https://shopify.com/authentication/26346881082\n  bearer_methods_supported:\n  - header\n  sources:\n  - well-known/oishii-oauth-protected-resource.json\nx-evidence:\n  fetched: '2026-08-04'\n  probes:\n  - url: https://oishii.com/.well-known/openid-configuration\n    http_status: 200\n  - url: https://oishii.com/.well-known/oauth-protected-resource\n    http_status: 200\n  - url: https://oishii.com/api/mcp\n    http_status: 200\n  - url: https://oishii.com/api/ucp/mcp\n    http_status: 422\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oishii/refs/heads/main/authentication/oishii-authentication.yml
summary_line: none/oauth2/openIdConnect · 4 schemes
tags:
- Company
- Agriculture
- Vertical Farming
- Food and Beverage
- Consumer Products
- E-Commerce
- Retail
- Agent Commerce
- Shopify
- MCP
- Universal Commerce Protocol
---
