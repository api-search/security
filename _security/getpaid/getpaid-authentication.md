---
api_key_in: []
api_specs:
- filename: getpaid-openapi-original.yml
  format: yaml
  label: Getpaid API v2
  slug: getpaid-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getpaid/refs/heads/main/openapi/getpaid-openapi-original.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Getpaid Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: GetPaid secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: GetPaid
provider_slug: getpaid
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 4
    tokenUrl: https://auth.getpaid.io/oauth/token
  name: OAuth
  sources:
  - openapi/getpaid-openapi-original.yml
  type: oauth2
slug: getpaid-authentication
source_filename: getpaid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/getpaid-openapi-original.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.getpaid.io/oauth/token\n    scopes: 4\n  sources:\n  - openapi/getpaid-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getpaid/refs/heads/main/authentication/getpaid-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Payments
- Embedded Payments
- Split Settlement
- Checkout
- Marketplace
- Onboarding
- Subscriptions
- Agent Payments
- Europe
---
