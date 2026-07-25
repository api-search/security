---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Zeller Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Zeller secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Zeller
provider_slug: zeller
scheme_count: 1
schemes:
- authorization_endpoint: https://developer.myzeller.com/_mcp/oauth2/auth
  description: OAuth2 / OpenID Connect protecting the Zeller developer portal (Redocly Realm "Reunite") and its hosted MCP server. Issuer auth.cloud.redocly.com; PKCE S256; dynamic client registration supported.
  flows:
  - authorizationCode
  - clientCredentials
  - refreshToken
  issuer: https://auth.cloud.redocly.com
  name: PortalOAuth2
  pkce: S256
  registration_endpoint: https://developer.myzeller.com/_mcp/register
  scopes:
  - openid
  - profile
  - email
  - offline_access
  sources:
  - well-known/zeller-oauth-authorization-server.json
  token_endpoint: https://developer.myzeller.com/_mcp/oauth2/token-portal
  type: oauth2
slug: zeller-authentication
source_filename: zeller-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://developer.myzeller.com/.well-known/oauth-authorization-server\ndocs: https://developer.myzeller.com/\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  api_key_in: []\n  gated: true\nschemes:\n- name: PortalOAuth2\n  type: oauth2\n  description: >-\n    OAuth2 / OpenID Connect protecting the Zeller developer portal (Redocly Realm\n    \"Reunite\") and its hosted MCP server. Issuer auth.cloud.redocly.com; PKCE S256;\n    dynamic client registration supported.\n  issuer: https://auth.cloud.redocly.com\n  authorization_endpoint: https://developer.myzeller.com/_mcp/oauth2/auth\n  token_endpoint: https://developer.myzeller.com/_mcp/oauth2/token-portal\n  registration_endpoint: https://developer.myzeller.com/_mcp/register\n  flows: [authorizationCode, clientCredentials, refreshToken]\n  scopes: [openid, profile, email, offline_access]\n  pkce: S256\n  sources:\
  \ [well-known/zeller-oauth-authorization-server.json]\nnotes: >-\n  Only the developer-portal / MCP OAuth surface is publicly discoverable. The\n  Zeller payments API (Terminal, Online, Tap to Pay) authenticates via credentials\n  issued after creating a free Zeller Developer account; its authentication model is\n  documented only behind that login and no anonymous OpenAPI securitySchemes are\n  published. apis.yml notes the portal historically fronted an Auth0 (OIDC) tenant;\n  the live well-known now resolves to Redocly's hosted auth.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeller/refs/heads/main/authentication/zeller-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Payments
- Australia
- Payment Gateway
- Payment Processing
- Acquiring
- Merchant Services
- Point of Sale
- In-Person Payments
- Tap to Pay
- SME
---
