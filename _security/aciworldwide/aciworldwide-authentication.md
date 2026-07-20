---
api_key_in:
- header
- body
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Aciworldwide Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aciworldwide secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Aciworldwide
provider_slug: aciworldwide
scheme_count: 2
schemes:
- description: 'Access token sent as "Authorization: Bearer {token}" on every request. Issued per channel; separate tokens for the test (eu-test.oppwa.com) and live (eu-prod.oppwa.com) environments.'
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - docs
  type: http
- description: Channel entity identifier that scopes the request to a specific merchant channel/currency configuration. Sent as the "entityId" form parameter (or query string). Distinct test and live entityId values.
  in: body
  name: entityId
  parameter: entityId
  sources:
  - docs
  type: apiKey
slug: aciworldwide-authentication
source_filename: aciworldwide-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.aciworldwide.com/tutorials/integration-guide/authentication\ndocs: https://docs.aciworldwide.com\nsummary:\n  types: [http]\n  api_key_in: [header, body]\n  oauth2_flows: []\n  notes: >-\n    Access is authorized by a bearer access token plus a channel entity\n    identifier (entityId). There is no OAuth2 authorization/token flow — the\n    bearer token is a long-lived credential issued per channel from the merchant\n    portal. entityId is submitted as a request parameter (form body or query),\n    the access token as an HTTP Authorization: Bearer header.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  description: >-\n    Access token sent as \"Authorization: Bearer {token}\" on every request.\n    Issued per channel; separate tokens for the test (eu-test.oppwa.com) and\n    live (eu-prod.oppwa.com) environments.\n  sources: [docs]\n- name: entityId\n\
  \  type: apiKey\n  in: body\n  parameter: entityId\n  description: >-\n    Channel entity identifier that scopes the request to a specific merchant\n    channel/currency configuration. Sent as the \"entityId\" form parameter (or\n    query string). Distinct test and live entityId values.\n  sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aciworldwide/refs/heads/main/authentication/aciworldwide-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Payments
- Payment Gateway
- Real-Time Payments
- eCommerce
- Fraud Management
- Tokenization
- Financial Services
---
