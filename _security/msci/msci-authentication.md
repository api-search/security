---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Msci Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
- clientInitiatedBackchannelAuthentication
overview: MSCI secures its APIs with oauth2 and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, deviceCode, and clientInitiatedBackchannelAuthentication flow(s).
provider_name: MSCI
provider_slug: msci
scheme_count: 3
schemes:
- authorization_endpoint: https://accounts.msci.com/authorize
  backchannel_authentication_endpoint: https://accounts.msci.com/bc-authorize
  code_challenge_methods_supported:
  - S256
  - plain
  device_authorization_endpoint: https://accounts.msci.com/oauth/device/code
  issuer: https://accounts.msci.com/
  jwks_uri: https://accounts.msci.com/.well-known/jwks.json
  name: MSCI Accounts OIDC
  openIdConnectUrl: https://accounts.msci.com/.well-known/openid-configuration
  registration_endpoint: https://accounts.msci.com/oidc/register
  revocation_endpoint: https://accounts.msci.com/oauth/revoke
  sources:
  - well-known/msci-accounts-openid-configuration.json
  token_endpoint: https://accounts.msci.com/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
  userinfo_endpoint: https://accounts.msci.com/userinfo
- authorization_endpoint: https://mcp.msci.com/oauth/authorize
  metadata: https://api2.msci.com/.well-known/oauth-authorization-server
  name: MSCI API gateway OAuth (api2.msci.com)
  note: RFC 8414 authorization-server metadata published on the production API gateway; API calls are bearer-token authenticated and return 401 "Authorization Header Missing" anonymously (verified against https://api2.msci.com/esg/data/v3.0/issuers).
  sources:
  - well-known/msci-api2-oauth-authorization-server.json
  token_endpoint: https://accounts.msci.com/oauth/token
  type: oauth2
- authorization_endpoint: https://mcp.msci.com/oauth/authorize
  metadata: https://mcp.msci.com/.well-known/oauth-authorization-server
  name: MSCI Connector MCP OAuth (mcp.msci.com)
  note: MSCI Connector (MCP) sign-in uses MSCI ONE / Private i credentials with app consent on first use.
  registration_endpoint: https://mcp.msci.com/iams/v1.0/apps/spa
  sources:
  - well-known/msci-mcp-oauth-authorization-server.json
  type: oauth2
slug: msci-authentication
source_filename: msci-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://accounts.msci.com/.well-known/openid-configuration\ndocs: https://developer.msci.com\nsummary:\n  types:\n    - oauth2\n    - openIdConnect\n  oauth2_flows:\n    - authorizationCode\n    - deviceCode\n    - clientInitiatedBackchannelAuthentication\n  issuer: https://accounts.msci.com/\nschemes:\n  - name: MSCI Accounts OIDC\n    type: openIdConnect\n    openIdConnectUrl: https://accounts.msci.com/.well-known/openid-configuration\n    issuer: https://accounts.msci.com/\n    authorization_endpoint: https://accounts.msci.com/authorize\n    token_endpoint: https://accounts.msci.com/oauth/token\n    device_authorization_endpoint: https://accounts.msci.com/oauth/device/code\n    userinfo_endpoint: https://accounts.msci.com/userinfo\n    jwks_uri: https://accounts.msci.com/.well-known/jwks.json\n    revocation_endpoint: https://accounts.msci.com/oauth/revoke\n    registration_endpoint: https://accounts.msci.com/oidc/register\n\
  \    code_challenge_methods_supported: [S256, plain]\n    token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, private_key_jwt, none]\n    backchannel_authentication_endpoint: https://accounts.msci.com/bc-authorize\n    sources:\n      - well-known/msci-accounts-openid-configuration.json\n  - name: MSCI API gateway OAuth (api2.msci.com)\n    type: oauth2\n    metadata: https://api2.msci.com/.well-known/oauth-authorization-server\n    authorization_endpoint: https://mcp.msci.com/oauth/authorize\n    token_endpoint: https://accounts.msci.com/oauth/token\n    note: >-\n      RFC 8414 authorization-server metadata published on the production API\n      gateway; API calls are bearer-token authenticated and return 401\n      \"Authorization Header Missing\" anonymously (verified against\n      https://api2.msci.com/esg/data/v3.0/issuers).\n    sources:\n      - well-known/msci-api2-oauth-authorization-server.json\n  - name: MSCI Connector MCP OAuth (mcp.msci.com)\n\
  \    type: oauth2\n    metadata: https://mcp.msci.com/.well-known/oauth-authorization-server\n    authorization_endpoint: https://mcp.msci.com/oauth/authorize\n    registration_endpoint: https://mcp.msci.com/iams/v1.0/apps/spa\n    note: MSCI Connector (MCP) sign-in uses MSCI ONE / Private i credentials with app consent on first use.\n    sources:\n      - well-known/msci-mcp-oauth-authorization-server.json\nnotes: >-\n  MSCI publishes no public OpenAPI documents, so no securitySchemes could be\n  derived from specs; this profile is assembled from the live RFC 8414 / OIDC\n  discovery documents and the MSCI Connector user guide. Developer portal API\n  detail pages (developer.msci.com/apis/*) require an MSCI client login.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/msci/refs/heads/main/authentication/msci-authentication.yml
summary_line: oauth2/openIdConnect · 3 schemes
tags:
- Financial Data
- Indexes
- ESG
- Climate
- Risk Analytics
- Real Estate
- Private Assets
- Investing
---
