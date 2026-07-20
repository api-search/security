---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Cuvva Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Cuvva secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Cuvva
provider_slug: cuvva
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://api.prod.cuv-prod.app/1/service-auth/2 (send_authorization_code method)
    flow: authorizationCode
    notes: Authorization code delivered by email; not spec-compliant at the authorize endpoint.
    tokenUrl: https://api.prod.cuv-prod.app/1/service-auth/2 (authenticate method)
  - flow: refreshToken
    notes: Refresh tokens are single-use and rotate; the returned refresh_token must be used going forward.
    tokenUrl: https://api.prod.cuv-prod.app/1/service-auth/2 (authenticate method)
  name: OAuth2
  sources:
  - https://github.com/cuvva/docs/blob/master/apis/auth.md
  type: oauth2
- bearerFormat: JWT
  name: BearerAccessToken
  notes: Downstream services authorize requests with the JWT access_token as a bearer token; the JWT subject must match the user_id for non-internal requests.
  scheme: bearer
  sources:
  - https://github.com/cuvva/docs/blob/master/apis/auth.md
  type: http
slug: cuvva-authentication
source_filename: cuvva-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://github.com/cuvva/docs/blob/master/apis/auth.md\ndocs: https://github.com/cuvva/docs/blob/master/apis/auth.md\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode, refreshToken]\n  token_type: bearer\n  notes: >-\n    Cuvva runs its own OAuth 2.0 implementation via the service-auth API. Clients\n    obtain a short-lived JWT access_token (token_type: bearer) plus a rotating\n    refresh_token. The authorization step is delivered by email (authorization\n    codes sent to an identifier), which the docs explicitly note is NOT\n    OAuth-spec-compliant for the authorization endpoint, though the token endpoint\n    follows RFC 6749 section 3.2. Refresh tokens are single-use and rotate on every\n    use; reuse revokes the whole chain.\nschemes:\n  - name: OAuth2\n    type: oauth2\n    sources: [https://github.com/cuvva/docs/blob/master/apis/auth.md]\n    flows:\n      - flow: authorizationCode\n        authorizationUrl:\
  \ https://api.prod.cuv-prod.app/1/service-auth/2 (send_authorization_code method)\n        tokenUrl: https://api.prod.cuv-prod.app/1/service-auth/2 (authenticate method)\n        notes: Authorization code delivered by email; not spec-compliant at the authorize endpoint.\n      - flow: refreshToken\n        tokenUrl: https://api.prod.cuv-prod.app/1/service-auth/2 (authenticate method)\n        notes: Refresh tokens are single-use and rotate; the returned refresh_token must be used going forward.\n  - name: BearerAccessToken\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    sources: [https://github.com/cuvva/docs/blob/master/apis/auth.md]\n    notes: Downstream services authorize requests with the JWT access_token as a bearer token; the JWT subject must match the user_id for non-internal requests.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cuvva/refs/heads/main/authentication/cuvva-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Insurance
- Insurtech
- Car Insurance
- Financial Services
- Mobile
- OAuth
- United Kingdom
---
