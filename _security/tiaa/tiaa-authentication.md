---
api_key_in: []
api_specs:
- filename: tiaa-fdx-openapi.yml
  format: yaml
  label: TIAA Financial Data Exchange API
  slug: tiaa-fdx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiaa/refs/heads/main/openapi/tiaa-fdx-openapi.yml
- filename: tiaa-sia-openapi.yml
  format: yaml
  label: TIAA Secure Income Account API
  slug: tiaa-sia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiaa/refs/heads/main/openapi/tiaa-sia-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Tiaa Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: TIAA secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: TIAA
provider_slug: tiaa
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://auth.tiaa.org/oauth2/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://auth.tiaa.org/oauth2/token
  name: OAuth2
  sources:
  - openapi/tiaa-fdx-openapi.yml
  type: oauth2
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://auth.tiaa.org/oauth2/token
  name: ClientCredentials
  sources:
  - openapi/tiaa-sia-openapi.yml
  type: oauth2
slug: tiaa-authentication
source_filename: tiaa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tiaa-fdx-openapi.yml, openapi/tiaa-sia-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.tiaa.org/oauth2/authorize\n    tokenUrl: https://auth.tiaa.org/oauth2/token\n    scopes: 6\n  sources:\n  - openapi/tiaa-fdx-openapi.yml\n- name: ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.tiaa.org/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/tiaa-sia-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiaa/refs/heads/main/authentication/tiaa-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Finance
- Financial Data
- Fintech
- Insurance
- Investment Management
- Retirement
- Wealth Management
- Fortune 100
---
