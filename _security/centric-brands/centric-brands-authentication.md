---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Centric Brands Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwt-bearer
overview: Centric Brands secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwt-bearer flow(s).
provider_name: Centric Brands
provider_slug: centric-brands
scheme_count: 2
schemes:
- authorizationUrl: https://shopify.com/authentication/1157103680/oauth/authorize
  code_challenge_methods:
  - S256
  endSessionUrl: https://shopify.com/authentication/1157103680/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values:
  - RS256
  issuer: https://shopify.com/authentication/1157103680
  jwksUri: https://shopify.com/authentication/1157103680/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://www.hudsonjeans.com/.well-known/openid-configuration
  sources:
  - well-known/centric-brands-openid-configuration.json
  - well-known/centric-brands-oauth-authorization-server.json
  tokenUrl: https://shopify.com/authentication/1157103680/oauth/token
  type: openIdConnect
- description: The UCP MCP endpoint (/api/ucp/mcp) accepts unauthenticated JSON-RPC for catalog, cart and checkout construction. Every tool call carries a meta.ucp-agent.profile URI identifying the calling agent rather than a credential.
  name: UCPAnonymousMCP
  sources:
  - mcp/centric-brands-ucp-mcp-tools.json
  type: none
  verified: Anonymous POST tools/list returned HTTP 200 with 13 tools on 8 hosts (2026-08-13).
slug: centric-brands-authentication
source_filename: centric-brands-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://www.hudsonjeans.com/.well-known/openid-configuration,\n  https://www.hudsonjeans.com/.well-known/oauth-authorization-server,\n  https://www.hudsonjeans.com/api/ucp/mcp\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  Centric Brands publishes no corporate API and therefore no corporate auth\n  scheme. This profile describes the only authenticated surface it actually\n  operates: Shopify Customer Accounts on the owned-brand DTC storefronts,\n  read from the live OIDC and RFC 8414 discovery documents captured in\n  well-known/. Note the split posture — the UCP MCP read tools (catalog, cart,\n  checkout read) answered an anonymous JSON-RPC tools/list with HTTP 200 and no\n  credentials, while completing a payment requires contemporaneous buyer\n  approval. Values below are from www.hudsonjeans.com; the other seven brand\n  hosts return identical metadata with a per-store Shopify shop id (recorded in\n  mcp/centric-brands-mcp.yml).\n\
  summary:\n  types:\n    - openIdConnect\n    - oauth2\n  oauth2_flows:\n    - authorizationCode\n    - refreshToken\n    - jwt-bearer\n  pkce: S256\n  token_endpoint_auth:\n    - client_secret_basic\n  anonymous_read: true\n  buyer_approval_required_for_payment: true\nschemes:\n  - name: ShopifyCustomerAccountOIDC\n    type: openIdConnect\n    issuer: https://shopify.com/authentication/1157103680\n    openIdConnectUrl: https://www.hudsonjeans.com/.well-known/openid-configuration\n    authorizationUrl: https://shopify.com/authentication/1157103680/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/1157103680/oauth/token\n    endSessionUrl: https://shopify.com/authentication/1157103680/logout\n    jwksUri: https://shopify.com/authentication/1157103680/.well-known/jwks.json\n    grant_types:\n      - authorization_code\n      - refresh_token\n      - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    code_challenge_methods:\n      - S256\n    id_token_signing_alg_values:\n\
  \      - RS256\n    sources:\n      - well-known/centric-brands-openid-configuration.json\n      - well-known/centric-brands-oauth-authorization-server.json\n  - name: UCPAnonymousMCP\n    type: none\n    description: >-\n      The UCP MCP endpoint (/api/ucp/mcp) accepts unauthenticated JSON-RPC for\n      catalog, cart and checkout construction. Every tool call carries a\n      meta.ucp-agent.profile URI identifying the calling agent rather than a\n      credential.\n    verified: >-\n      Anonymous POST tools/list returned HTTP 200 with 13 tools on 8 hosts\n      (2026-08-13).\n    sources:\n      - mcp/centric-brands-ucp-mcp-tools.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centric-brands/refs/heads/main/authentication/centric-brands-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Apparel
- Accessories
- Footwear
- Beauty
- Kids
- Lifestyle
- Brand Management
- Licensing
- Entertainment Licensing
- Sports Licensing
- Fashion
- Consumer Products
- Fortune 1000
- Private Equity Owned
---
