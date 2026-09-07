---
anonymous_access: false
api_key_in: []
api_specs:
- filename: 701x-api-v1-openapi.json
  format: json
  label: 701x API V1
  slug: 701x-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/701x/refs/heads/main/openapi/701x-api-v1-openapi.json
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: 701X Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: 701x secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: 701x
provider_slug: 701x
scheme_count: 2
schemes:
- applied_to: '1158 of 1391 operations require [oauth2: [API701x]]; the remaining 234 declare no security requirement in the contract.'
  flows:
  - authorizationUrl: https://login.701x.com/connect/authorize
    declared_scopes:
      api1: Demo API - full access
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.701x.com/connect/token
  name: oauth2
  sources:
  - openapi/701x-api-v1-openapi.json
  type: oauth2
- name: openIdConnect
  note: Not declared in the OpenAPI, but the same issuer the oauth2 scheme points at publishes a full OIDC discovery document, so OIDC is available to clients that want id_tokens and userinfo.
  openIdConnectUrl: https://login.701x.com/.well-known/openid-configuration
  sources:
  - https://login.701x.com/.well-known/openid-configuration
  type: openIdConnect
slug: 701x-authentication
source_filename: 701x-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  https://login.701x.com/.well-known/openid-configuration (HTTP 200, fetched 2026-09-05) +\n  openapi/701x-api-v1-openapi.json\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  primary: OAuth 2.0 authorization code against the company's own IdentityServer at login.701x.com\n  api_keys: false\n  basic_auth: false\n  mtls: false\n  note: >-\n    701x publishes no authentication documentation. Everything below is read from the contract's\n    securityScheme and from the company's own OpenID Connect discovery document, both of which are\n    anonymous and public.\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.701x.com/connect/authorize\n    tokenUrl: https://login.701x.com/connect/token\n    scopes: 1\n    declared_scopes:\n      api1: Demo API - full access\n  applied_to: >-\n    1158 of 1391 operations require\
  \ [oauth2: [API701x]]; the remaining 234 declare no security\n    requirement in the contract.\n  sources:\n  - openapi/701x-api-v1-openapi.json\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://login.701x.com/.well-known/openid-configuration\n  note: >-\n    Not declared in the OpenAPI, but the same issuer the oauth2 scheme points at publishes a full\n    OIDC discovery document, so OIDC is available to clients that want id_tokens and userinfo.\n  sources:\n  - https://login.701x.com/.well-known/openid-configuration\nauthorization_server:\n  issuer: https://login.701x.com\n  discovery: https://login.701x.com/.well-known/openid-configuration\n  jwks_uri: https://login.701x.com/.well-known/openid-configuration/jwks\n  software: self-hosted (Duende/IdentityServer-shaped endpoint layout under /connect/*)\n  endpoints:\n    authorization: https://login.701x.com/connect/authorize\n    token: https://login.701x.com/connect/token\n    userinfo: https://login.701x.com/connect/userinfo\n\
  \    end_session: https://login.701x.com/connect/endsession\n    revocation: https://login.701x.com/connect/revocation\n    introspection: https://login.701x.com/connect/introspect\n    device_authorization: https://login.701x.com/connect/deviceauthorization\n    check_session_iframe: https://login.701x.com/connect/checksession\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - implicit\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  response_types_supported:\n  - code\n  - token\n  - id_token\n  - id_token token\n  - code id_token\n  - code token\n  - code id_token token\n  code_challenge_methods_supported:\n  - plain\n  - S256\n  scopes_supported:\n  - openid\n  - profile\n  - email\n  - api1\n  - offline_access\n  claims_supported_count: 18\n  logout:\n    frontchannel: true\n    backchannel: true\nfindings:\n- >-\n  The scope the API actually enforces (API701x) is NOT in the authorization server's\n  scopes_supported\
  \ list, and the scope the securityScheme documents (api1, described as\n  \"Demo API - full access\") is not the one any operation requires. A client following the\n  published contract literally would request the wrong scope.\n- >-\n  The authorization server advertises the implicit and resource-owner-password grants, both\n  discouraged by OAuth 2.0 Security Best Current Practice (RFC 9700).\n- >-\n  PKCE is supported, but \"plain\" is offered alongside S256; S256 should be preferred by clients.\n- No API-key, HTTP basic or mutual-TLS authentication path exists on this API.\ncross_links:\n  scopes: scopes/701x-scopes.yml\n  conventions: conventions/701x-conventions.yml\n  well_known: well-known/701x-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/701x/refs/heads/main/authentication/701x-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Agriculture
- AgTech
- Livestock
- Cattle Management
- Ranch Management
- Animal Health
- IoT
- GPS Tracking
- Traceability
- Beef Production
---
