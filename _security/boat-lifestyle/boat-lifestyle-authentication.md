---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Boat Lifestyle Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Boat Lifestyle secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Boat Lifestyle
provider_slug: boat-lifestyle
scheme_count: 2
schemes:
- authorization_endpoint: https://shopify.com/authentication/5789384802/oauth/authorize
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
  end_session_endpoint: https://shopify.com/authentication/5789384802/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/5789384802
  jwks_uri: https://shopify.com/authentication/5789384802/.well-known/jwks.json
  name: ShopifyCustomerAccountsOIDC
  openIdConnectUrl: https://www.boat-lifestyle.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/boat-lifestyle-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint: https://shopify.com/authentication/5789384802/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- field: meta.ucp-agent.profile
  format: uri
  in: request body
  name: UCPAgentProfile
  note: Not an authentication scheme in the OAuth sense — a mandatory agent-profile URI every MCP tool call must carry, used for agent attestation and policy.
  required: true
  sources:
  - mcp/boat-lifestyle-tools-list.json
  type: agentIdentity
slug: boat-lifestyle-authentication
source_filename: boat-lifestyle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: searched\nsource:\n- https://www.boat-lifestyle.com/.well-known/openid-configuration\n- https://www.boat-lifestyle.com/.well-known/oauth-authorization-server\n- https://www.boat-lifestyle.com/.well-known/oauth-protected-resource\n- https://www.boat-lifestyle.com/agents.md\nnote: >-\n  Derived from live discovery documents rather than an OpenAPI — boAt Lifestyle\n  publishes no OpenAPI. The identity layer is Shopify Customer Accounts; the\n  storefront host publishes the discovery documents but the issuer is Shopify.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  anonymous_surface: >-\n    The UCP MCP tools/list, catalog and cart tools answer without credentials.\n    Buyer-scoped operations (order retrieval, saved customer data) require an\n    access token from the Shopify authorization server.\nschemes:\n- name: ShopifyCustomerAccountsOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://www.boat-lifestyle.com/.well-known/openid-configuration\n\
  \  issuer: https://shopify.com/authentication/5789384802\n  authorization_endpoint: https://shopify.com/authentication/5789384802/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/5789384802/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/5789384802/logout\n  jwks_uri: https://shopify.com/authentication/5789384802/.well-known/jwks.json\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  code_challenge_methods_supported:\n  - S256\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  claims_supported:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - nonce\n  - sid\n  - email\n  - email_verified\n  sources:\n  - well-known/boat-lifestyle-openid-configuration.json\n- name: UCPAgentProfile\n  type: agentIdentity\n  in: request body\n\
  \  field: meta.ucp-agent.profile\n  format: uri\n  required: true\n  note: >-\n    Not an authentication scheme in the OAuth sense — a mandatory agent-profile URI\n    every MCP tool call must carry, used for agent attestation and policy.\n  sources:\n  - mcp/boat-lifestyle-tools-list.json\nprotected_resource:\n  resource: https://www.boat-lifestyle.com\n  authorization_servers:\n  - https://shopify.com/authentication/5789384802\n  bearer_methods_supported:\n  - header\n  spec: RFC 9728 OAuth 2.0 Protected Resource Metadata\n  sources:\n  - well-known/boat-lifestyle-oauth-protected-resource.json\npkce:\n  required: true\n  methods:\n  - S256\ndocs: https://www.boat-lifestyle.com/agents.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boat-lifestyle/refs/heads/main/authentication/boat-lifestyle-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Consumer Electronics
- E-Commerce
- Retail
- Audio
- Wearables
- Agent Commerce
- MCP
- Shopify
- India
---
