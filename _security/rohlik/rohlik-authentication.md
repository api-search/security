---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Rohlik Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- tokenExchange
- refreshToken
overview: Rohlik secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, tokenExchange, and refreshToken flow(s).
provider_name: Rohlik
provider_slug: rohlik
scheme_count: 1
schemes:
- applies_to:
  - https://mcp.rohlik.cz/mcp
  authorization_endpoint: https://identity.rohlik.cz/oauth2/authorize
  code_challenge_methods_supported:
  - S256
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  issuer: https://identity.rohlik.cz
  jwks_uri: https://identity.rohlik.cz/oauth2/jwks
  name: RohlikOAuth2
  registration_endpoint: https://identity.rohlik.cz/connect/register
  response_types_supported:
  - code
  sources:
  - https://identity.rohlik.cz/.well-known/openid-configuration
  - https://mcp.rohlik.cz/.well-known/oauth-protected-resource/mcp
  token_endpoint: https://identity.rohlik.cz/oauth2/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - tls_client_auth
  - self_signed_tls_client_auth
  - none
  type: oauth2
  userinfo_endpoint: https://identity.rohlik.cz/userinfo
slug: rohlik-authentication
source_filename: rohlik-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://identity.rohlik.cz/.well-known/openid-configuration\ndocs: https://rohlik.cz/mcp-docs\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, clientCredentials, deviceCode, tokenExchange, refreshToken]\n  bearer_methods: [header]\nschemes:\n  - name: RohlikOAuth2\n    type: oauth2\n    issuer: https://identity.rohlik.cz\n    authorization_endpoint: https://identity.rohlik.cz/oauth2/authorize\n    token_endpoint: https://identity.rohlik.cz/oauth2/token\n    userinfo_endpoint: https://identity.rohlik.cz/userinfo\n    jwks_uri: https://identity.rohlik.cz/oauth2/jwks\n    registration_endpoint: https://identity.rohlik.cz/connect/register   # RFC 7591 dynamic client registration\n    grant_types_supported:\n      - authorization_code\n      - client_credentials\n      - refresh_token\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:ietf:params:oauth:grant-type:token-exchange\n \
  \   response_types_supported: [code]\n    code_challenge_methods_supported: [S256]                            # PKCE\n    token_endpoint_auth_methods_supported:\n      - client_secret_basic\n      - client_secret_post\n      - client_secret_jwt\n      - private_key_jwt\n      - tls_client_auth\n      - self_signed_tls_client_auth\n      - none\n    applies_to:\n      - https://mcp.rohlik.cz/mcp\n    sources:\n      - https://identity.rohlik.cz/.well-known/openid-configuration\n      - https://mcp.rohlik.cz/.well-known/oauth-protected-resource/mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rohlik/refs/heads/main/authentication/rohlik-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Retail
- Grocery
- E-commerce
- Delivery
- Logistics
- MCP
- OAuth
- Europe
---
