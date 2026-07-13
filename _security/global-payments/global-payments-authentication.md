---
api_key_in: []
api_specs:
- filename: global-payments-unified-payments-api-openapi.yml
  format: yaml
  label: Global Payments Unified Payments API
  slug: payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/global-payments/refs/heads/main/openapi/global-payments-unified-payments-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Global Payments Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Global Payments secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Global Payments
provider_slug: global-payments
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 4
    tokenUrl: https://apis.globalpay.com/oauth2/token
  name: oauth2
  sources:
  - openapi/global-payments-unified-payments-api-openapi.yml
  type: oauth2
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/global-payments-unified-payments-api-openapi.yml
  type: http
slug: global-payments-authentication
source_filename: global-payments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/global-payments-unified-payments-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.globalpay.com/oauth2/token\n    scopes: 4\n  sources:\n  - openapi/global-payments-unified-payments-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/global-payments-unified-payments-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/global-payments/refs/heads/main/authentication/global-payments-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- eCommerce
- Payment Processing
- Payment Technology
- Payments
- POS
- Fortune 1000
---
