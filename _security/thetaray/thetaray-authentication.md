---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Thetaray Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: ThetaRay secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: ThetaRay
provider_slug: thetaray
scheme_count: 1
schemes:
- client_id_metadata_document_supported: true
  flows:
  - authorizationUrl: https://api.thetaray.com/_mcp/oauth2/auth
    flow: authorizationCode
    scopes:
    - openid
    - profile
    - email
    - offline_access
    tokenUrl: https://api.thetaray.com/_mcp/oauth2/token-portal
  - flow: clientCredentials
    tokenUrl: https://api.thetaray.com/_mcp/oauth2/token-portal
  id_token_signing_alg_values:
  - RS256
  issuer: https://auth.cloud.redocly.com
  jwks_uri: https://auth.cloud.redocly.com/.well-known/jwks.json
  name: RedoclyPortalOAuth2
  registration_endpoint: https://api.thetaray.com/_mcp/register
  sources:
  - well-known/thetaray-oauth-authorization-server.json
  subject_types:
  - public
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: thetaray-authentication
source_filename: thetaray-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: https://api.thetaray.com/.well-known/oauth-authorization-server\nraw: well-known/thetaray-oauth-authorization-server.json\nscope_note: >-\n  Derived entirely from the anonymous RFC 8414 metadata document that api.thetaray.com serves. It\n  governs access to the ThetaRay developer portal and its MCP endpoint (both Redocly Cloud). The\n  authentication model of ThetaRay's AML transaction-monitoring and screening product API is NOT\n  described here — that contract sits behind the customer SSO wall and was not retrievable. No\n  OpenAPI securitySchemes were available to derive from.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  refresh_tokens: true\n  pkce: true\n  pkce_methods:\n  - S256\n  dynamic_client_registration: true\n  api_key_in: []\nschemes:\n- name: RedoclyPortalOAuth2\n  type: oauth2\n  issuer: https://auth.cloud.redocly.com\n  jwks_uri: https://auth.cloud.redocly.com/.well-known/jwks.json\n\
  \  registration_endpoint: https://api.thetaray.com/_mcp/register\n  token_endpoint_auth_methods:\n  - none\n  id_token_signing_alg_values:\n  - RS256\n  subject_types:\n  - public\n  client_id_metadata_document_supported: true\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.thetaray.com/_mcp/oauth2/auth\n    tokenUrl: https://api.thetaray.com/_mcp/oauth2/token-portal\n    scopes:\n    - openid\n    - profile\n    - email\n    - offline_access\n  - flow: clientCredentials\n    tokenUrl: https://api.thetaray.com/_mcp/oauth2/token-portal\n  sources:\n  - well-known/thetaray-oauth-authorization-server.json\nprotected_resources:\n- resource: https://api.thetaray.com/mcp\n  bearer_methods:\n  - header\n  token_types:\n  - Bearer\n  source: well-known/thetaray-oauth-protected-resource-mcp.json\ngated_surfaces:\n- url: https://api.thetaray.com/openapi\n  status: 302\n  to: https://auth.cloud.redocly.com/oidc/oauth2/auth\n  note: developer portal / API reference requires\
  \ a ThetaRay customer account\n- url: http://docs.thetaray.com/\n  status: 302\n  to: https://login.microsoftonline.com/f176e0ee-1f77-4c82-94c8-fb98d2d81117/saml2\n  note: documentation host requires Microsoft Entra SAML sign-in\nx-evidence:\n- fetched: '2026-08-05'\n  url: https://api.thetaray.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thetaray/refs/heads/main/authentication/thetaray-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- anti-money-laundering
- financial-crime
- transaction-monitoring
- sanctions-screening
- kyc
- regtech
- risk-assessment
- artificial-intelligence
- banking
- Fintech
- Payments
- Compliance
- MCP
---
