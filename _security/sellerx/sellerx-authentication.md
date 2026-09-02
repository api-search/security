---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Sellerx Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: SellerX secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: SellerX
provider_slug: sellerx
scheme_count: 1
schemes:
- applies_to: https://mcp.sellerx.com/mcp
  bearer_methods_supported:
  - header
  code_challenge_methods_supported:
  - S256
  flows:
  - authorizationUrl: https://mcp.sellerx.com/authorize
    flow: authorizationCode
    refreshUrl: https://mcp.sellerx.com/token
    scopes:
      read: The only scope advertised in scopes_supported. SellerX publishes no scope reference describing what it grants.
    tokenUrl: https://mcp.sellerx.com/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://mcp.sellerx.com/
  name: OAuth2
  registration_endpoint: https://mcp.sellerx.com/register
  response_types_supported:
  - code
  sources:
  - well-known/sellerx-oauth-authorization-server.json
  - well-known/sellerx-oauth-protected-resource.json
  token_endpoint_auth_methods_supported:
  - client_secret_post
  type: oauth2
slug: sellerx-authentication
source_filename: sellerx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://mcp.sellerx.com/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  SellerX publishes no OpenAPI, so this profile is not derived from\n  securitySchemes. It is read verbatim from the RFC 8414 authorization-server\n  metadata and the RFC 9728 protected-resource metadata that the SellerX MCP\n  host serves anonymously, plus the observed 401 challenge on the MCP endpoint.\n\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  bearer_methods: [header]\n  pkce_required: true\n  dynamic_client_registration: true\n\nschemes:\n- name: OAuth2\n  type: oauth2\n  applies_to: https://mcp.sellerx.com/mcp\n  sources:\n  - well-known/sellerx-oauth-authorization-server.json\n  - well-known/sellerx-oauth-protected-resource.json\n  issuer: https://mcp.sellerx.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.sellerx.com/authorize\n    tokenUrl: https://mcp.sellerx.com/token\n\
  \    refreshUrl: https://mcp.sellerx.com/token\n    scopes:\n      read: >-\n        The only scope advertised in scopes_supported. SellerX publishes no\n        scope reference describing what it grants.\n  registration_endpoint: https://mcp.sellerx.com/register\n  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported: [code]\n  token_endpoint_auth_methods_supported: [client_secret_post]\n  code_challenge_methods_supported: [S256]\n  bearer_methods_supported: [header]\n\nobserved_challenge:\n  url: https://mcp.sellerx.com/mcp\n  http_status: 401\n  www_authenticate: >-\n    Bearer error=\"invalid_token\", error_description=\"Authentication failed. The\n    provided bearer token is invalid, expired, or no longer recognized by the\n    server. To resolve: clear authentication tokens in your MCP client and\n    reconnect. Your client should automatically re-register and obtain new\n    tokens.\",\n    resource_metadata=\"https://mcp.sellerx.com/.well-known/oauth-protected-resource/mcp\"\
  \n\ngaps:\n- >-\n  No OpenID Connect discovery: /.well-known/openid-configuration returns 404, so\n  the authorization server is OAuth 2.0/2.1 only, not OIDC.\n- >-\n  No human-readable authentication documentation is published anywhere on\n  sellerx.com; the metadata endpoints are the only public description of the\n  auth model.\n- >-\n  scopes_supported carries a single opaque `read` scope with no published\n  meaning, so a client cannot reason about least privilege before registering.\n\nx-evidence:\n  fetched: '2026-08-05'\n  probed:\n  - url: https://mcp.sellerx.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://mcp.sellerx.com/.well-known/oauth-protected-resource/mcp\n    http_status: 200\n  - url: https://mcp.sellerx.com/mcp\n    http_status: 401\n  - url: https://mcp.sellerx.com/.well-known/openid-configuration\n    http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sellerx/refs/heads/main/authentication/sellerx-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- E-Commerce
- Consumer Brands
- Retail
- Amazon Aggregator
- Marketplace-Seller
- Consumer Packaged Goods
- Germany
---
