---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Healthex Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: HealthEx secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: HealthEx
provider_slug: healthex
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'Organization API access. Admins mint an apiKey / apiSecret pair in the HealthEx web-app Admin panel, then exchange them at the token endpoint for a JWT that is sent as `Authorization: Bearer <JWT>`. Tokens are valid for 24 hours. HealthEx notes that none of the currently supported organization APIs require additional permissions/scopes.'
  name: organizationBearerJWT
  scheme: bearer
  sources:
  - docs.healthex.io/authentication
  token_endpoint: https://api.healthex.io/v1/auth/token
  token_lifetime_hours: 24
  token_request:
    body: '{"apiKey": "...", "apiSecret": "..."}'
    content_type: application/json
    method: POST
  type: http
- description: Patient-mediated OAuth 2.0 (SMART-on-FHIR style) for accessing an individual patient's consented FHIR records and the MCP server. PKCE (S256) required; public (none) and client_secret_post client auth supported.
  flows:
  - authorizationUrl: https://api.healthex.io/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://api.healthex.io/oauth/register
    revocationUrl: https://api.healthex.io/oauth/revoke
    scopes:
      email: Email claim
      offline_access: Issue a refresh token for long-lived access
      openid: OpenID Connect authentication
      patient/*.read: Read access to the patient's consented FHIR records
      profile: Basic profile claims
    tokenUrl: https://api.healthex.io/oauth/token
  name: patientOAuth2
  sources:
  - api.healthex.io/.well-known/oauth-authorization-server
  - api.healthex.io/.well-known/oauth-protected-resource
  type: oauth2
slug: healthex-authentication
source_filename: healthex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.healthex.io/authentication\ndocs: https://docs.healthex.io/authentication\nsummary:\n  types: [http, oauth2]\n  http_scheme: bearer\n  bearer_format: JWT\n  oauth2_flows: [authorizationCode]\n  models:\n    - organization-api-token\n    - patient-oauth2\nschemes:\n  - name: organizationBearerJWT\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Organization API access. Admins mint an apiKey / apiSecret pair in the\n      HealthEx web-app Admin panel, then exchange them at the token endpoint for\n      a JWT that is sent as `Authorization: Bearer <JWT>`. Tokens are valid for\n      24 hours. HealthEx notes that none of the currently supported organization\n      APIs require additional permissions/scopes.\n    token_endpoint: https://api.healthex.io/v1/auth/token\n    token_request:\n      method: POST\n      content_type: application/json\n      body: '{\"apiKey\": \"...\",\
  \ \"apiSecret\": \"...\"}'\n    token_lifetime_hours: 24\n    sources: [docs.healthex.io/authentication]\n  - name: patientOAuth2\n    type: oauth2\n    description: >-\n      Patient-mediated OAuth 2.0 (SMART-on-FHIR style) for accessing an\n      individual patient's consented FHIR records and the MCP server. PKCE\n      (S256) required; public (none) and client_secret_post client auth\n      supported.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.healthex.io/oauth/authorize\n        tokenUrl: https://api.healthex.io/oauth/token\n        registrationUrl: https://api.healthex.io/oauth/register\n        revocationUrl: https://api.healthex.io/oauth/revoke\n        pkce: S256\n        scopes:\n          patient/*.read: Read access to the patient's consented FHIR records\n          offline_access: Issue a refresh token for long-lived access\n          openid: OpenID Connect authentication\n          profile: Basic profile claims\n          email: Email\
  \ claim\n    sources:\n      - api.healthex.io/.well-known/oauth-authorization-server\n      - api.healthex.io/.well-known/oauth-protected-resource\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/healthex/refs/heads/main/authentication/healthex-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Healthcare
- Health Records
- FHIR
- Patient Consent
- Data Sharing
- Interoperability
- TEFCA
- MCP
- Agents
---
