---
api_key_in:
- header
api_specs:
- filename: rtr-inbound-participant-payment-api-openapi.yml
  format: yaml
  label: RTR Sandbox - Inbound Participant Payment API
  slug: rtr-inbound-participant-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/rtr-inbound-participant-payment-api-openapi.yml
- filename: rtr-inbound-csp-heartbeat-api-openapi.yml
  format: yaml
  label: RTR Sandbox - Inbound Exchange Heartbeat API
  slug: rtr-inbound-heartbeat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/rtr-inbound-csp-heartbeat-api-openapi.yml
- filename: rtr-interest-report-api-openapi.yml
  format: yaml
  label: RTR Sandbox - Interest Report API
  slug: rtr-interest-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/rtr-interest-report-api-openapi.yml
- filename: rtr-balance-report-api-openapi.yml
  format: yaml
  label: RTR Sandbox - Payment Capacity Balance Report API
  slug: rtr-balance-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/rtr-balance-report-api-openapi.yml
- filename: fif-extracts-api-openapi.yml
  format: yaml
  label: FIF Extracts API
  slug: fif-extracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/fif-extracts-api-openapi.yml
- filename: fif-branch-api-openapi.yml
  format: yaml
  label: FIF Branch API
  slug: fif-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/fif-branch-api-openapi.yml
- filename: ccin-extracts-api-openapi.yml
  format: yaml
  label: CCIN Extracts API
  slug: ccin-extracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/ccin-extracts-api-openapi.yml
- filename: ccin-lookup-api-openapi.yml
  format: yaml
  label: CCIN Lookup API
  slug: ccin-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/openapi/ccin-lookup-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Payments Canada Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Payments Canada secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Payments Canada
provider_slug: payments-canada
scheme_count: 2
schemes:
- in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/fif-branch-api-openapi.yml
  - openapi/fif-extracts-api-openapi.yml
  type: apiKey
- description: This API uses OAuth 2 with the implicit grant flow. (The access token expires in 5 minutes)
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.payments.ca/accesstoken
  name: oAuth
  sources:
  - openapi/rtr-balance-report-api-openapi.yml
  - openapi/rtr-inbound-csp-heartbeat-api-openapi.yml
  - openapi/rtr-inbound-participant-payment-api-openapi.yml
  - openapi/rtr-interest-report-api-openapi.yml
  type: oauth2
slug: payments-canada-authentication
source_filename: payments-canada-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: derived\nsource: openapi/fif-branch-api-openapi.yml, openapi/fif-extracts-api-openapi.yml, openapi/rtr-balance-report-api-openapi.yml,\n  openapi/rtr-inbound-csp-heartbeat-api-openapi.yml, openapi/rtr-inbound-participant-payment-api-openapi.yml,\n  openapi/rtr-interest-report-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/fif-branch-api-openapi.yml\n  - openapi/fif-extracts-api-openapi.yml\n- name: oAuth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.payments.ca/accesstoken\n    scopes: 1\n  description: This API uses OAuth 2 with the implicit grant flow. (The access token expires\n    in 5 minutes)\n  sources:\n  - openapi/rtr-balance-report-api-openapi.yml\n  - openapi/rtr-inbound-csp-heartbeat-api-openapi.yml\n  - openapi/rtr-inbound-participant-payment-api-openapi.yml\n\
  \  - openapi/rtr-interest-report-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payments-canada/refs/heads/main/authentication/payments-canada-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Financial Services
- Payments
- Canada
- Payment Infrastructure
- Clearing and Settlement
- Real-Time Rail
- ISO 20022
- Lynx
- Crown Corporation
- Faster Payments
---
