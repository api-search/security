---
api_key_in: []
api_specs:
- filename: wells-fargo-gateway-api-openapi.yml
  format: yaml
  label: Wells Fargo Gateway API
  slug: gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wells-fargo/refs/heads/main/openapi/wells-fargo-gateway-api-openapi.yml
- filename: wells-fargo-account-transactions-api-openapi.yml
  format: yaml
  label: Wells Fargo Account Transactions API
  slug: account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wells-fargo/refs/heads/main/openapi/wells-fargo-account-transactions-api-openapi.yml
- filename: wells-fargo-ach-payments-api-openapi.yml
  format: yaml
  label: Wells Fargo ACH Payments API
  slug: ach-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wells-fargo/refs/heads/main/openapi/wells-fargo-ach-payments-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Wells Fargo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: wells-fargo secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: wells-fargo
provider_slug: wells-fargo
scheme_count: 3
schemes:
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://api.wellsfargo.com/oauth2/token
  name: oauth2
  sources:
  - openapi/wells-fargo-account-transactions-api-openapi.yml
  - openapi/wells-fargo-ach-payments-api-openapi.yml
  type: oauth2
- flows:
  - authorizationUrl: https://api.wellsfargo.com/oauth2/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://api.wellsfargo.com/oauth2/token
  name: oauth2
  sources:
  - openapi/wells-fargo-gateway-api-openapi.yml
  type: oauth2
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/wells-fargo-gateway-api-openapi.yml
  type: http
slug: wells-fargo-authentication
source_filename: wells-fargo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wells-fargo-account-transactions-api-openapi.yml, openapi/wells-fargo-ach-payments-api-openapi.yml,\n  openapi/wells-fargo-gateway-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.wellsfargo.com/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/wells-fargo-account-transactions-api-openapi.yml\n  - openapi/wells-fargo-ach-payments-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.wellsfargo.com/oauth2/authorize\n    tokenUrl: https://api.wellsfargo.com/oauth2/token\n    scopes: 3\n  sources:\n  - openapi/wells-fargo-gateway-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/wells-fargo-gateway-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wells-fargo/refs/heads/main/authentication/wells-fargo-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Fortune 100
---
