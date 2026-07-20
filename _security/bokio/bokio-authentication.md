---
api_key_in: []
api_specs:
- filename: bokio-company-api-openapi.yml
  format: yaml
  label: Bokio Company API
  slug: bokio-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-company-api-openapi.yml
- filename: bokio-general-api-openapi.yml
  format: yaml
  label: Bokio General API
  slug: bokio-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-general-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Bokio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Bokio secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Bokio
provider_slug: bokio
scheme_count: 3
schemes:
- name: tokenAuth
  scheme: bearer
  sources:
  - openapi/bokio-company-api-openapi.yml
  - openapi/bokio-general-api-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /token
  - authorizationUrl: /authorize
    flow: authorizationCode
    scopes: 24
    tokenUrl: /token
  name: access_token
  sources:
  - openapi/bokio-company-api-openapi.yml
  - openapi/bokio-general-api-openapi.yml
  type: oauth2
- name: client_auth
  scheme: basic
  sources:
  - openapi/bokio-company-api-openapi.yml
  - openapi/bokio-general-api-openapi.yml
  type: http
slug: bokio-authentication
source_filename: bokio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/bokio-company-api-openapi.yml, openapi/bokio-general-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: tokenAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n  - openapi/bokio-general-api-openapi.yml\n- name: access_token\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /token\n    scopes: 0\n  - flow: authorizationCode\n    authorizationUrl: /authorize\n    tokenUrl: /token\n    scopes: 24\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n  - openapi/bokio-general-api-openapi.yml\n- name: client_auth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n  - openapi/bokio-general-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/authentication/bokio-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Fintech
- Accounting
- Bookkeeping
- Invoicing
- Payments
- Sweden
- SMB
- OAuth
---
