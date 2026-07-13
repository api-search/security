---
api_key_in: []
api_specs:
- filename: bank-of-america-cashpro-api-openapi.yml
  format: yaml
  label: Bank of America CashPro API
  slug: cashpro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-america/refs/heads/main/openapi/bank-of-america-cashpro-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Bank Of America Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Bank of America secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Bank of America
provider_slug: bank-of-america
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bank-of-america-bofa-api-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 4
    tokenUrl: https://api.bankofamerica.com/oauth/token
  name: OAuth2
  sources:
  - openapi/bank-of-america-cashpro-api-openapi.yml
  type: oauth2
slug: bank-of-america-authentication
source_filename: bank-of-america-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bank-of-america-bofa-api-openapi.yml, openapi/bank-of-america-cashpro-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/bank-of-america-bofa-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.bankofamerica.com/oauth/token\n    scopes: 4\n  sources:\n  - openapi/bank-of-america-cashpro-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-of-america/refs/heads/main/authentication/bank-of-america-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Banking
- Corporate Banking
- Finance
- Payments
- Treasury
- CashPro
- Fortune 100
---
