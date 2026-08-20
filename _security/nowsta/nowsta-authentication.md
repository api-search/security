---
api_key_in: []
api_specs:
- filename: nowsta-integration-openapi.yml
  format: yaml
  label: Nowsta Integration API
  slug: nowsta-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nowsta/refs/heads/main/openapi/nowsta-integration-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Nowsta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nowsta secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nowsta
provider_slug: nowsta
scheme_count: 1
schemes:
- description: 'A per-company integration token issued by Nowsta. The customer retrieves it from the Nowsta UI and enters it into the integrating platform (for example on a settings page); the platform then sends it on every request as `Authorization: Bearer <token>`.'
  format: Bearer <token>
  header: Authorization
  name: bearerAuth
  properties:
    approval_gate: Nowsta must approve a company before its token is active. Requests on behalf of an unapproved company return 403 with error code 1101.
    challenge: No WWW-Authenticate challenge is returned. A missing or invalid token yields 401 {"errors":[{"code":1000,"message":"Nil JSON web token"}]} (verified live 2026-08-01).
    expiry_documented: false
    rotation_documented: false
    scopes: none - the token is not scoped, it authorizes every operation for the company
    self_serve: false
    tenancy: One token per company. A token is bound to the single company that purchased the integration and only authorizes operations for that company; referencing another company's objects returns 403 with error code 1100.
    token_format_hint: The 401 message text is "Nil JSON web token", implying the credential is a JWT internally, but Nowsta documents it only as an opaque token and publishes no claims, issuer, audience or expiry.
    transport: HTTPS required - Nowsta warns HTTP may give unexpected results. Cross-origin browser requests are not permitted, so the credential is intended for server-to-server use only.
  scheme: bearer
  sources:
  - openapi/nowsta-integration-openapi.yml
  type: http
slug: nowsta-authentication
source_filename: nowsta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://web.archive.org/web/20240603053309/https://developer.nowsta.com/\ndocs: https://web.archive.org/web/20240603053309/https://developer.nowsta.com/\nspec_source: openapi/nowsta-integration-openapi.yml\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  oauth2_flows: []\n  api_key_in: []\n  model: static per-company bearer token, allow-listed by the provider\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  header: Authorization\n  format: 'Bearer <token>'\n  description: >-\n    A per-company integration token issued by Nowsta. The customer retrieves it from the Nowsta UI and\n    enters it into the integrating platform (for example on a settings page); the platform then sends\n    it on every request as `Authorization: Bearer <token>`.\n  sources:\n  - openapi/nowsta-integration-openapi.yml\n  properties:\n    rotation_documented: false\n    expiry_documented: false\n    scopes: none - the token\
  \ is not scoped, it authorizes every operation for the company\n    tenancy: >-\n      One token per company. A token is bound to the single company that purchased the integration and\n      only authorizes operations for that company; referencing another company's objects returns 403\n      with error code 1100.\n    self_serve: false\n    approval_gate: >-\n      Nowsta must approve a company before its token is active. Requests on behalf of an unapproved\n      company return 403 with error code 1101.\n    transport: >-\n      HTTPS required - Nowsta warns HTTP may give unexpected results. Cross-origin browser requests are\n      not permitted, so the credential is intended for server-to-server use only.\n    challenge: >-\n      No WWW-Authenticate challenge is returned. A missing or invalid token yields\n      401 {\"errors\":[{\"code\":1000,\"message\":\"Nil JSON web token\"}]} (verified live 2026-08-01).\n    token_format_hint: >-\n      The 401 message text is \"Nil JSON web token\"\
  , implying the credential is a JWT internally, but\n      Nowsta documents it only as an opaque token and publishes no claims, issuer, audience or expiry.\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_keys: false\nnotes:\n- >-\n  There is no OAuth 2.0, no OIDC discovery document and no scope surface, so no scopes/ artifact is\n  emitted for this provider - see conformance/nowsta-conformance.yml.\n- >-\n  The single unscoped, non-expiring, company-wide write token is the main authorization weakness of\n  this API: there is no way to grant an integration read-only or resource-limited access, and no\n  documented rotation or revocation procedure.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nowsta/refs/heads/main/authentication/nowsta-authentication.yml
summary_line: http · 1 scheme
tags:
- Workforce Management
- staff-scheduling
- shift-scheduling
- Time and Attendance
- Hourly Workforce
- gig-work
- event-staffing
- Hospitality
- staffing-agency
- Vendor Management
- Payroll
- Human Resources
---
