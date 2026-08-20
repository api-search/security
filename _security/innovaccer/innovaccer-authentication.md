---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Innovaccer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Innovaccer declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Innovaccer
provider_slug: innovaccer
scheme_count: 5
schemes:
- description: User-mediated flow. The client calls /authorize with response_type=code, client_id, redirect_uri, scope, state and audience/aud set to the HMCP server URI, then exchanges the code at /token for a bearer access token.
  flow: authorizationCode
  id: oauth2-authorization-code
  parameters:
  - response_type
  - client_id
  - redirect_uri
  - scope
  - state
  - audience
  - aud
  pkce: true
  pkce_note: PKCE is named in the HMCP repository description as part of the OAuth 2.0 posture.
  token_response_fields:
  - access_token
  - token_type
  - expires_in
  - scope
  - id_token
  - patient
  type: oauth2
- description: Service-to-service flow with no user involvement. POST /token with grant_type=client_credentials, client_id, client_secret and scope. The specification recommends pairing it with mTLS.
  flow: clientCredentials
  id: oauth2-client-credentials
  type: oauth2
- description: OIDC on top of the authorization-code flow — request the `openid` scope to receive an ID token; a UserInfo endpoint supplies additional user attributes. Standard claims include SMART on FHIR and healthcare-specific claims.
  id: openid-connect
  type: openIdConnect
- description: Mutual TLS is named in the HMCP specification index as one of the two primary authentication mechanisms, for secure service-to-service communication.
  id: mutual-tls
  type: mutualTLS
- bearer_format: JWT
  description: 'Every HMCP API request carries `Authorization: Bearer ACCESS_TOKEN`. Access tokens are JWTs.'
  id: bearer-token
  scheme: bearer
  type: http
slug: innovaccer-authentication
source_filename: innovaccer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nsource: https://github.com/innovaccer/Healthcare-MCP/blob/main/docs/specification/auth.md\ndocs:\n- https://github.com/innovaccer/Healthcare-MCP/blob/main/docs/specification/auth.md\n- https://github.com/innovaccer/Healthcare-MCP/blob/main/docs/specification/index.md\n- https://github.com/innovaccer/Healthcare-MCP/blob/main/docs/specification/hmcp_auth_vs_mcp_auth.md\n- https://github.com/innovaccer/Healthcare-MCP/blob/main/docs/specification/context.md\nsummary: >-\n  Innovaccer publishes no OpenAPI and no anonymous auth reference for the Nucleus /\n  Datashop developer platform — that portal's API catalog sits behind a session\n  login. The auth profile recorded here is the one Innovaccer DOES publish openly:\n  the Healthcare Model Context Protocol (HMCP), its first-party open-source\n  extension of MCP, whose specification documents the OAuth 2.0 / OpenID Connect /\n  SMART on FHIR authorization model that healthcare agents use\
  \ to reach an HMCP\n  server. Derived from the published specification text, not from a machine-readable\n  contract.\napplies_to:\n  api: Healthcare Model Context Protocol (HMCP)\n  repository: https://github.com/innovaccer/Healthcare-MCP\n  note: >-\n    HMCP is a protocol specification plus a Python reference implementation. There is\n    no Innovaccer-hosted public HMCP endpoint to probe; a customer or partner runs an\n    HMCP server (or connects to the Innovaccer HMCP Cloud Gateway under contract).\nframework: SMART on FHIR (OAuth 2.0 + OpenID Connect)\nschemes:\n- id: oauth2-authorization-code\n  type: oauth2\n  flow: authorizationCode\n  description: >-\n    User-mediated flow. The client calls /authorize with response_type=code,\n    client_id, redirect_uri, scope, state and audience/aud set to the HMCP server\n    URI, then exchanges the code at /token for a bearer access token.\n  parameters:\n  - response_type\n  - client_id\n  - redirect_uri\n  - scope\n  - state\n  - audience\n\
  \  - aud\n  token_response_fields:\n  - access_token\n  - token_type\n  - expires_in\n  - scope\n  - id_token\n  - patient\n  pkce: true\n  pkce_note: PKCE is named in the HMCP repository description as part of the OAuth 2.0 posture.\n- id: oauth2-client-credentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    Service-to-service flow with no user involvement. POST /token with\n    grant_type=client_credentials, client_id, client_secret and scope. The\n    specification recommends pairing it with mTLS.\n- id: openid-connect\n  type: openIdConnect\n  description: >-\n    OIDC on top of the authorization-code flow — request the `openid` scope to\n    receive an ID token; a UserInfo endpoint supplies additional user attributes.\n    Standard claims include SMART on FHIR and healthcare-specific claims.\n- id: mutual-tls\n  type: mutualTLS\n  description: >-\n    Mutual TLS is named in the HMCP specification index as one of the two primary\n    authentication mechanisms,\
  \ for secure service-to-service communication.\n- id: bearer-token\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    Every HMCP API request carries `Authorization: Bearer ACCESS_TOKEN`. Access\n    tokens are JWTs.\ntoken_claims:\n  format: JWT\n  standard:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - scope\n  healthcare:\n  - patient\n  - encounter\n  - tenant\n  - acr\n  - fhirUser\n  validation_guidance: >-\n    The specification instructs clients and servers to verify all claims including\n    audience (aud) and issuer (iss).\npatient_context:\n  mechanisms:\n  - {kind: oauth-scope, detail: \"patient/ scope prefix plus launch/patient; token response carries a `patient` (and optionally `encounter`) parameter\"}\n  - {kind: jwt-claim, detail: \"patient/encounter embedded as JWT claims; server enforces context without per-call parameters\"}\n  - {kind: http-header, detail: \"HTTP headers supported for backwards compatibility with systems that do not fully\
  \ implement SMART on FHIR\"}\ntoken_storage_guidance:\n- Store access tokens in memory where possible, not in localStorage or cookies\n- Use secure OS credential storage in native apps\n- Prefer refresh tokens over long-lived access tokens\n- Validate tokens on both client and server\ngaps:\n- >-\n  No anonymous /.well-known/openid-configuration or /.well-known/oauth-authorization-server\n  is served: nucleus.innovaccer.com 302s those paths to /login (see well-known/innovaccer-well-known.yml).\n- >-\n  The specification uses placeholder issuer/audience hosts\n  (authorization-server.example.com, hmcp-server.example.com); no Innovaccer-operated\n  authorization server host is published.\n- No auth reference is published for the Nucleus / Datashop platform API itself.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/innovaccer/refs/heads/main/authentication/innovaccer-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Healthcare
- Health Data
- FHIR
- Interoperability
- Population Health
- Artificial Intelligence
- Data Platform
- Design System
- MCP
---
