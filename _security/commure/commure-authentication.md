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
source_yaml: "generated: '2026-08-15'\nmethod: searched\nsource: openapi/commure-fhir-openapi.yml\ndocs: https://www.postman.com/commure/commure/documentation/vp76tv7/commure-fhir-api\nalso_probed:\n- https://accounts.commure.com/.well-known/openid-configuration\n- https://accounts.commure.com/.well-known/oauth-authorization-server\n- https://accounts.commure.com/oauth2/default/.well-known/openid-configuration\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: SMARTonFHIR\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-{tenant-id}.developer.commure.com/auth/authorize\n    tokenUrl: https://api-{tenant-id}.developer.commure.com/auth/token\n    scopes: 5\n  - flow: clientCredentials\n    tokenUrl: https://api-{tenant-id}.developer.commure.com/auth/token\n    scopes: 0\n  description: OpenID Connect / SMART App Launch. Supports the authorization code (with PKCE),\n    implicit,\
  \ hybrid, client credentials and refresh token grants.\n  sources:\n  - openapi/commure-fhir-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Access token issued by the Commure Authentication API, presented as a bearer\n    token (tokens are prefixed \"Sec-\").\n  sources:\n  - openapi/commure-fhir-openapi.yml\ntoken:\n  type: bearer\n  header: Authorization\n  format: 'Bearer Sec-...'\n  prefix: Sec-\ngrants:\n- authorization_code\n- client_credentials\n- refresh_token\nextras:\n  pkce: true\n  implicit_flow_supported: true\n  hybrid_flow_supported: true\n  smart_ehr_launch: true\n  smart_standalone_launch: true\n  sso: >-\n    The authorize endpoint authenticates the user via single sign-on, typically using an SSO\n    provider configured by the hospital.\nendpoints:\n  authorize: /auth/authorize\n  token: /auth/token\n  userinfo: /auth/userinfo\n  jwks: /auth/jwks\n  logout: /auth/logout\n  openid_configuration: /auth/.well-known/openid-configuration\n\
  \  smart_configuration: /api/v1/r4/.well-known/smart-configuration\ntenancy:\n  model: host-scoped\n  note: >-\n    The tenant id is part of the host (api-{tenant-id}.developer.commure.com), so a token is\n    scoped to a single tenant host. Commure's own example tenant id is 99750511.\nidentity_provider:\n  scope: >-\n    This block describes the LIVE identity surface for Commure's PRODUCTS (the accounts.commure.com\n    sign-in already linked from apis.yml). It is a separate surface from the FHIR API auth\n    described above, which lives on the retired tenant hosts. It is recorded here because it is the\n    only Commure authentication endpoint that is currently reachable and machine-readable.\n  host: accounts.commure.com\n  platform: Okta Customer Identity (Okta-hosted, on Commure's own domain)\n  method: probed\n  probed: '2026-08-15'\n  issuers:\n  - issuer: https://accounts.commure.com\n    metadata:\n    - path: /.well-known/openid-configuration\n      status: 200\n      file:\
  \ well-known/commure-accounts-openid-configuration.json\n      spec: OpenID Connect Discovery 1.0\n    - path: /.well-known/oauth-authorization-server\n      status: 200\n      file: well-known/commure-accounts-oauth-authorization-server.json\n      spec: RFC 8414 OAuth 2.0 Authorization Server Metadata\n    endpoints:\n      authorization: https://accounts.commure.com/oauth2/v1/authorize\n      token: https://accounts.commure.com/oauth2/v1/token\n      userinfo: https://accounts.commure.com/oauth2/v1/userinfo\n      jwks: https://accounts.commure.com/oauth2/v1/keys\n      introspection: https://accounts.commure.com/oauth2/v1/introspect\n      revocation: https://accounts.commure.com/oauth2/v1/revoke\n      registration: https://accounts.commure.com/oauth2/v1/clients\n      device_authorization: https://accounts.commure.com/oauth2/v1/device/authorize\n      end_session: https://accounts.commure.com/oauth2/v1/logout\n  - issuer: https://accounts.commure.com/oauth2/default\n    role: Commure's\
  \ custom authorization server - the one carrying Commure-configured scopes.\n    metadata:\n    - path: /oauth2/default/.well-known/openid-configuration\n      status: 200\n      file: well-known/commure-accounts-default-openid-configuration.json\n      spec: OpenID Connect Discovery 1.0\n    endpoints:\n      authorization: https://accounts.commure.com/oauth2/default/v1/authorize\n      token: https://accounts.commure.com/oauth2/default/v1/token\n      userinfo: https://accounts.commure.com/oauth2/default/v1/userinfo\n      jwks: https://accounts.commure.com/oauth2/default/v1/keys\n      introspection: https://accounts.commure.com/oauth2/default/v1/introspect\n      revocation: https://accounts.commure.com/oauth2/default/v1/revoke\n      end_session: https://accounts.commure.com/oauth2/default/v1/logout\n  grants:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - client_credentials\n  - 'urn:ietf:params:oauth:grant-type:device_code'\n  grants_note: >-\n    client_credentials\
  \ is advertised only by the org authorization server\n    (/.well-known/oauth-authorization-server); the custom `default` server does not list it. The\n    urn:okta:* and auth0.com MFA grant types in the raw documents are Okta platform grants and are\n    not restated here.\n  response_types: [code, token, id_token, code id_token, code token, id_token token, code id_token token]\n  pkce: true\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, client_secret_jwt, private_key_jwt, none]\n  private_key_jwt: true\n  dpop: true\n  dpop_algorithms: [RS256, RS384, RS512, ES256, ES384, ES512]\n  dynamic_client_registration: true\n  dynamic_client_registration_note: >-\n    A registration_endpoint is advertised (/oauth2/v1/clients). This is standard Okta org behaviour\n    and is almost certainly access-token protected; it was not exercised.\n  caveat: >-\n    This is a delegated identity provider. It authenticates humans into Commure's product\
  \ estate;\n    it is NOT an authorization server for a public Commure API, and no Commure API resource server\n    advertises it (/.well-known/oauth-protected-resource returns 405 here). Do not read it as a\n    developer-facing API auth surface.\nx-searched:\n  fetched: '2026-08-15'\n  previous: '2026-07-31'\n  sources:\n  - https://www.postman.com/commure/commure/documentation/vp76tv7/commure-fhir-api\n  - postman/commure-fhir-api-collection.json\n  findings:\n  - Commure publishes no standalone authentication documentation page; the auth contract above\n    is taken from the request descriptions in its public Postman collection.\n  - Access is gated by the Commure Developer User Agreement - credentials are issued under a\n    partner/approval relationship, not self-serve.\n  - Neither discovery document (/auth/.well-known/openid-configuration,\n    /api/v1/r4/.well-known/smart-configuration) is currently served by any reachable host; see\n    well-known/commure-well-known.yml.\n"
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
