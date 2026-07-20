---
api_key_in: []
api_specs:
- filename: incognia-openapi-original.yml
  format: yaml
  label: Incognia API
  slug: incognia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incognia/refs/heads/main/openapi/incognia-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Incognia Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Incognia secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Incognia
provider_slug: incognia
scheme_count: 3
schemes:
- description: client_id and client_secret sent as HTTP Basic credentials to the token endpoint.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/incognia-openapi-original.yml
  type: http
- bearerFormat: JWT
  description: OAuth 2.0 bearer access token obtained from POST /v2/token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/incognia-openapi-original.yml
  type: http
- description: OAuth 2.0 client-credentials grant. No scopes are defined; access is scoped by the credential's tenant.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.incognia.com/api/v2/token
  name: oauth2
  sources:
  - openapi/incognia-openapi-original.yml
  type: oauth2
slug: incognia-authentication
source_filename: incognia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/incognia-openapi-original.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: client_id and client_secret sent as HTTP Basic credentials to the token endpoint.\n  sources:\n  - openapi/incognia-openapi-original.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer access token obtained from POST /v2/token.\n  sources:\n  - openapi/incognia-openapi-original.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.incognia.com/api/v2/token\n    scopes: 0\n  description: OAuth 2.0 client-credentials grant. No scopes are defined; access is scoped by\n    the credential's tenant.\n  sources:\n  - openapi/incognia-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/incognia/refs/heads/main/authentication/incognia-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Cybersecurity
- Fraud Prevention
- Device Fingerprinting
- Location Identity
- Identity Verification
- Risk Assessment
- Authentication
- Fintech
- Anti-Fraud
---
