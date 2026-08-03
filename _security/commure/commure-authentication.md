---
api_key_in: []
api_specs:
- filename: commure-fhir-openapi.yml
  format: yaml
  label: Commure FHIR API
  slug: commure-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commure/refs/heads/main/openapi/commure-fhir-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Commure Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Commure secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Commure
provider_slug: commure
scheme_count: 2
schemes:
- description: OpenID Connect / SMART App Launch. Supports the authorization code (with PKCE), implicit, hybrid, client credentials and refresh token grants.
  flows:
  - authorizationUrl: https://api-{tenant-id}.developer.commure.com/auth/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://api-{tenant-id}.developer.commure.com/auth/token
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api-{tenant-id}.developer.commure.com/auth/token
  name: SMARTonFHIR
  sources:
  - openapi/commure-fhir-openapi.yml
  type: oauth2
- description: Access token issued by the Commure Authentication API, presented as a bearer token (tokens are prefixed "Sec-").
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/commure-fhir-openapi.yml
  type: http
slug: commure-authentication
source_filename: commure-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: searched\nsource: openapi/commure-fhir-openapi.yml\ndocs: https://www.postman.com/commure/commure/documentation/vp76tv7/commure-fhir-api\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: SMARTonFHIR\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-{tenant-id}.developer.commure.com/auth/authorize\n    tokenUrl: https://api-{tenant-id}.developer.commure.com/auth/token\n    scopes: 5\n  - flow: clientCredentials\n    tokenUrl: https://api-{tenant-id}.developer.commure.com/auth/token\n    scopes: 0\n  description: OpenID Connect / SMART App Launch. Supports the authorization code (with PKCE),\n    implicit, hybrid, client credentials and refresh token grants.\n  sources:\n  - openapi/commure-fhir-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Access token issued by the Commure Authentication API, presented\
  \ as a bearer\n    token (tokens are prefixed \"Sec-\").\n  sources:\n  - openapi/commure-fhir-openapi.yml\ntoken:\n  type: bearer\n  header: Authorization\n  format: 'Bearer Sec-...'\n  prefix: Sec-\ngrants:\n- authorization_code\n- client_credentials\n- refresh_token\nextras:\n  pkce: true\n  implicit_flow_supported: true\n  hybrid_flow_supported: true\n  smart_ehr_launch: true\n  smart_standalone_launch: true\n  sso: >-\n    The authorize endpoint authenticates the user via single sign-on, typically using an SSO\n    provider configured by the hospital.\nendpoints:\n  authorize: /auth/authorize\n  token: /auth/token\n  userinfo: /auth/userinfo\n  jwks: /auth/jwks\n  logout: /auth/logout\n  openid_configuration: /auth/.well-known/openid-configuration\n  smart_configuration: /api/v1/r4/.well-known/smart-configuration\ntenancy:\n  model: host-scoped\n  note: >-\n    The tenant id is part of the host (api-{tenant-id}.developer.commure.com), so a token is\n    scoped to a single tenant host.\
  \ Commure's own example tenant id is 99750511.\nx-searched:\n  fetched: '2026-07-31'\n  sources:\n  - https://www.postman.com/commure/commure/documentation/vp76tv7/commure-fhir-api\n  - postman/commure-fhir-api-collection.json\n  findings:\n  - Commure publishes no standalone authentication documentation page; the auth contract above\n    is taken from the request descriptions in its public Postman collection.\n  - Access is gated by the Commure Developer User Agreement - credentials are issued under a\n    partner/approval relationship, not self-serve.\n  - Neither discovery document (/auth/.well-known/openid-configuration,\n    /api/v1/r4/.well-known/smart-configuration) is currently served by any reachable host; see\n    well-known/commure-well-known.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commure/refs/heads/main/authentication/commure-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Healthcare
- United States
- Clinical AI
- Ambient AI
- Revenue Cycle Management
- FHIR
- SMART on FHIR
- Interoperability
- EHR
- Remote Monitoring
- Health System
- Terminology Services
---
