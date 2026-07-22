---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Optum Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Optum secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Optum
provider_slug: optum
scheme_count: 1
schemes:
- bearer_format: JWT
  credentials: client_id + client_secret provisioned during onboarding / sandbox access
  flows:
  - flow: clientCredentials
    token_url_production: https://apigw.optum.com/apip/auth/v2/token
    token_url_sandbox: https://sandbox-apigw.optum.com/apip/auth/v2/token
  name: OptumOAuth2
  notes: Access is controlled via OAuth2 client-credentials grant. Consumers exchange a client_id and client_secret for a short-lived (1 hour) JWT access_token, returned with token_type "bearer" and expires_in 3600, then send it as a Bearer token on subsequent requests over TLS 1.2+.
  request_header: 'Authorization: Bearer <access_token>'
  scheme: bearer
  token_lifetime_seconds: 3600
  type: oauth2
slug: optum-authentication
source_filename: optum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.optum.com/apitools/reference/security-and-authorization-v2-overview\ndocs: https://developer.optum.com/eligibilityandclaims/docs/optum-security-and-authorization\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  transport_security: TLS 1.2+\nschemes:\n- name: OptumOAuth2\n  type: oauth2\n  scheme: bearer\n  bearer_format: JWT\n  flows:\n  - flow: clientCredentials\n    token_url_production: https://apigw.optum.com/apip/auth/v2/token\n    token_url_sandbox: https://sandbox-apigw.optum.com/apip/auth/v2/token\n  token_lifetime_seconds: 3600\n  request_header: 'Authorization: Bearer <access_token>'\n  credentials: client_id + client_secret provisioned during onboarding / sandbox access\n  notes: >-\n    Access is controlled via OAuth2 client-credentials grant. Consumers exchange a\n    client_id and client_secret for a short-lived (1 hour) JWT access_token, returned\n    with token_type\
  \ \"bearer\" and expires_in 3600, then send it as a Bearer token on\n    subsequent requests over TLS 1.2+.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/authentication/optum-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Healthcare
- Health Insurance
- Claims
- Eligibility
- FHIR
- Interoperability
- Pharmacy
- EDI
- X12
- Payments
- Prior Authorization
---
