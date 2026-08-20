---
api_key_in:
- header
auth_types:
- apiKey
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Vendia Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Vendia secures its APIs with apiKey, http, oauth2, and openIdConnect across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Vendia
provider_slug: vendia
scheme_count: 6
schemes:
- applies_to: Vendia Share GraphQL API (per node)
  format: 'Authorization: MY_API_KEY_HERE'
  in: header
  issued_via:
  - Vendia console
  - GraphQL mutation
  - share node add-api-key
  name: NodeApiKey
  note: The API key is only viewable at the time of creation.
  parameter: Authorization
  source: https://docs.vendia.com/platform/operational/scalar-data/node-authentication/
  type: apiKey
- applies_to: Vendia Share GraphQL API, Vendia MCP Gateway
  bearerFormat: JWT
  byoidp: true
  byoidp_config:
  - jwks_url
  - issuer
  - audience
  byoidp_providers_documented:
  - Okta
  - Auth0
  - AWS Cognito
  - Azure AD
  format: 'Authorization: Bearer MY_JWT_HERE'
  name: BearerJWT
  parameter: Authorization
  scheme: bearer
  source: https://docs.vendia.com/platform/operational/scalar-data/node-authentication/
  type: http
- dynamic_client_registration: true
  flows:
  - authorizationUrl: https://auth.share.vendia.com/authorize
    flow: authorizationCode
    pkce: S256
    refreshUrl: https://auth.share.vendia.com/token
    tokenUrl: https://auth.share.vendia.com/token
  - flow: clientCredentials
    note: Used for programmatic token exchange from custom applications.
    tokenUrl: https://auth.share.vendia.com/token
  id_token_signing_alg:
  - RS256
  issuer: https://auth.share.vendia.com
  name: VendiaOAuth2
  registration_endpoint: https://auth.share.vendia.com/register
  revocation_endpoint: https://auth.share.vendia.com/revoke
  source: well-known/vendia-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
- jwks_uri: https://auth.share.vendia.com/.well-known/jwks.json
  name: VendiaOIDC
  openIdConnectUrl: https://auth.share.vendia.com/.well-known/openid-configuration
  source: well-known/vendia-openid-configuration.json
  subject_types:
  - public
  type: openIdConnect
- applies_to: Vendia MCP Gateway (Pro and Enterprise tiers)
  description: Simplified path for no-code/low-code tools (OpenAI Agent Builder, Zapier, Make, n8n) that cannot perform an OAuth flow. The gateway performs the token exchange on the caller's behalf. Vendia explicitly recommends OAuth over this method.
  in: header
  name: ServiceCredentialHeaders
  parameters:
  - X-Vendia-Client-Id
  - X-Vendia-Client-Secret
  source: https://docs.vendia.com/platform/vendia-mcp-server/authentication/
  type: apiKey
- applies_to: Vendia Share GraphQL subscriptions (WebSocket)
  formats:
  - '{"type": "connection_init", "payload": {"apiKey": "YOUR_KEY"}}'
  - '{"type": "connection_init", "payload": {"token": "YOUR_JWT"}}'
  in: message
  name: WebSocketConnectionInit
  source: https://docs.vendia.com/platform/operational/scalar-data/node-authentication/
  type: apiKey
slug: vendia-authentication
source_filename: vendia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://docs.vendia.com/platform/operational/scalar-data/node-authentication/\ndocs:\n- https://docs.vendia.com/platform/operational/scalar-data/node-authentication/\n- https://docs.vendia.com/platform/vendia-mcp-server/authentication/\n- https://docs.vendia.com/platform/integrations/sso-authentication/\nnote: >-\n  Derived mechanically from OpenAPI securitySchemes was not possible — Vendia\n  publishes no OpenAPI. This profile is searched from the documented auth reference\n  for the GraphQL API, the MCP Gateway, and the live RFC 8414 discovery document at\n  https://auth.share.vendia.com/.well-known/oauth-authorization-server (saved\n  verbatim to well-known/vendia-oauth-authorization-server.json).\nsummary:\n  types: [apiKey, http, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  pkce: [S256]\nschemes:\n- name: NodeApiKey\n  type: apiKey\n  in: header\n\
  \  parameter: Authorization\n  format: 'Authorization: MY_API_KEY_HERE'\n  applies_to: Vendia Share GraphQL API (per node)\n  issued_via: [Vendia console, GraphQL mutation, 'share node add-api-key']\n  note: The API key is only viewable at the time of creation.\n  source: https://docs.vendia.com/platform/operational/scalar-data/node-authentication/\n- name: BearerJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  parameter: Authorization\n  format: 'Authorization: Bearer MY_JWT_HERE'\n  applies_to: Vendia Share GraphQL API, Vendia MCP Gateway\n  byoidp: true\n  byoidp_config: [jwks_url, issuer, audience]\n  byoidp_providers_documented: [Okta, Auth0, AWS Cognito, Azure AD]\n  source: https://docs.vendia.com/platform/operational/scalar-data/node-authentication/\n- name: VendiaOAuth2\n  type: oauth2\n  issuer: https://auth.share.vendia.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.share.vendia.com/authorize\n    tokenUrl: https://auth.share.vendia.com/token\n\
  \    refreshUrl: https://auth.share.vendia.com/token\n    pkce: S256\n  - flow: clientCredentials\n    tokenUrl: https://auth.share.vendia.com/token\n    note: Used for programmatic token exchange from custom applications.\n  revocation_endpoint: https://auth.share.vendia.com/revoke\n  registration_endpoint: https://auth.share.vendia.com/register\n  dynamic_client_registration: true\n  token_endpoint_auth_methods: [none, client_secret_post, client_secret_basic]\n  id_token_signing_alg: [RS256]\n  source: well-known/vendia-oauth-authorization-server.json\n- name: VendiaOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://auth.share.vendia.com/.well-known/openid-configuration\n  jwks_uri: https://auth.share.vendia.com/.well-known/jwks.json\n  subject_types: [public]\n  source: well-known/vendia-openid-configuration.json\n- name: ServiceCredentialHeaders\n  type: apiKey\n  in: header\n  parameters:\n  - X-Vendia-Client-Id\n  - X-Vendia-Client-Secret\n  applies_to: Vendia MCP Gateway (Pro\
  \ and Enterprise tiers)\n  description: >-\n    Simplified path for no-code/low-code tools (OpenAI Agent Builder, Zapier, Make,\n    n8n) that cannot perform an OAuth flow. The gateway performs the token exchange\n    on the caller's behalf. Vendia explicitly recommends OAuth over this method.\n  source: https://docs.vendia.com/platform/vendia-mcp-server/authentication/\n- name: WebSocketConnectionInit\n  type: apiKey\n  in: message\n  applies_to: Vendia Share GraphQL subscriptions (WebSocket)\n  formats:\n  - '{\"type\": \"connection_init\", \"payload\": {\"apiKey\": \"YOUR_KEY\"}}'\n  - '{\"type\": \"connection_init\", \"payload\": {\"token\": \"YOUR_JWT\"}}'\n  source: https://docs.vendia.com/platform/operational/scalar-data/node-authentication/\nsso:\n  supported: true\n  tiers: [Enterprise]\n  docs: https://docs.vendia.com/platform/integrations/sso-authentication/\nx-evidence:\n  fetched: '2026-08-05'\n  probes:\n  - url: https://auth.share.vendia.com/.well-known/openid-configuration\n\
  \    status: 200\n  - url: https://auth.share.vendia.com/.well-known/jwks.json\n    status: 200\n  - url: https://auth.share.vendia.com/token\n    status: 400\n    note: POST without a body returns a JSON error — endpoint is live\n  - url: https://docs.vendia.com/platform/operational/scalar-data/node-authentication/\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vendia/refs/heads/main/authentication/vendia-authentication.yml
summary_line: apiKey/http/oauth2/openIdConnect · 6 schemes
tags:
- Company
- MCP
- Artificial Intelligence
- Data Sharing
- Data Platform
- GraphQL
- Agents
- API Gateway
- Data Governance
---
