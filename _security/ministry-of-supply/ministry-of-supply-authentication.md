---
api_key_in: []
auth_types:
- none
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Ministry Of Supply Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: Ministry of Supply secures its APIs with none, openIdConnect, and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: Ministry of Supply
provider_slug: ministry-of-supply
scheme_count: 2
schemes:
- description: Every MCP tool requires meta.ucp-agent.profile, a URI identifying the calling agent's UCP profile. This is an identity declaration, not a credential — the endpoint answers unauthenticated.
  name: ucp-agent-profile
  sources:
  - mcp/ministry-of-supply-mcp-tools-list.json
  type: none
- authorizationUrl: https://shopify.com/authentication/3092321/oauth/authorize
  bearer_methods_supported:
  - header
  end_session_endpoint: https://shopify.com/authentication/3092321/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/3092321
  jwks_uri: https://shopify.com/authentication/3092321/.well-known/jwks.json
  name: shopify-customer-accounts-oidc
  openIdConnectUrl: https://www.ministryofsupply.com/.well-known/openid-configuration
  pkce:
  - S256
  protected_resource: https://www.ministryofsupply.com
  response_types:
  - code
  sources:
  - well-known/ministry-of-supply-openid-configuration.json
  - well-known/ministry-of-supply-oauth-protected-resource.json
  tokenUrl: https://shopify.com/authentication/3092321/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
slug: ministry-of-supply-authentication
source_filename: ministry-of-supply-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: >-\n  https://www.ministryofsupply.com/.well-known/openid-configuration,\n  https://www.ministryofsupply.com/.well-known/oauth-protected-resource,\n  https://www.ministryofsupply.com/api/ucp/mcp (tools/list),\n  https://www.ministryofsupply.com/llms.txt\ndocs: https://www.ministryofsupply.com/agents.md\nsummary:\n  types: [none, openIdConnect, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken, jwt-bearer]\n  note: >-\n    Two distinct auth postures. (1) The UCP/MCP commerce endpoint accepts anonymous calls — tools/list\n    returned 200 with no credential — and identity is carried per-call as an agent profile URI in\n    meta.ucp-agent.profile rather than as a bearer token. Payment authorization is delegated to a payment\n    handler with contemporaneous human approval, so the agent never holds a card credential. (2) Customer\n    accounts use Shopify Customer Accounts OpenID Connect, with the merchant's\
  \ own issuer.\nschemes:\n- name: ucp-agent-profile\n  type: none\n  description: >-\n    Every MCP tool requires meta.ucp-agent.profile, a URI identifying the calling agent's UCP profile.\n    This is an identity declaration, not a credential — the endpoint answers unauthenticated.\n  sources: [mcp/ministry-of-supply-mcp-tools-list.json]\n- name: shopify-customer-accounts-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://www.ministryofsupply.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/3092321\n  authorizationUrl: https://shopify.com/authentication/3092321/oauth/authorize\n  tokenUrl: https://shopify.com/authentication/3092321/oauth/token\n  jwks_uri: https://shopify.com/authentication/3092321/.well-known/jwks.json\n  end_session_endpoint: https://shopify.com/authentication/3092321/logout\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  response_types: [code]\n  pkce: [S256]\n  token_endpoint_auth_methods:\
  \ [client_secret_basic, client_secret_post]\n  id_token_signing_alg: [RS256]\n  bearer_methods_supported: [header]\n  protected_resource: https://www.ministryofsupply.com\n  sources: [well-known/ministry-of-supply-openid-configuration.json, well-known/ministry-of-supply-oauth-protected-resource.json]\npayment_authorization:\n  model: buyer-approved payment handler\n  handlers:\n  - id: gpay\n    name: com.google.pay\n    merchant_name: Ministry of Supply\n    merchant_origin: www.ministryofsupply.com\n  - id: shopify.card\n    name: dev.shopify.card\n  - id: shop_pay\n    name: dev.shopify.shop_pay\n  rule: >-\n    \"Checkout requires human approval. Agents must not complete payment without explicit buyer consent.\"\n    — https://www.ministryofsupply.com/llms.txt\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ministry-of-supply/refs/heads/main/authentication/ministry-of-supply-authentication.yml
summary_line: none/openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Apparel
- Retail
- E-Commerce
- Direct to Consumer
- Agentic Commerce
- MCP
- Universal Commerce Protocol
- Shopify
- Manufacturing
---
