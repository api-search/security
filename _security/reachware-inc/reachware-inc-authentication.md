---
api_key_in: []
api_specs:
- filename: reachware-inc-reachpay-openapi.yml
  format: yaml
  label: Reach Pay API
  slug: reach-pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reachware-inc/refs/heads/main/openapi/reachware-inc-reachpay-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Reachware Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reachware Inc. secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reachware Inc.
provider_slug: reachware-inc
scheme_count: 1
schemes:
- description: 'Merchant API token: Authorization: Bearer {reachToken}'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/reachware-inc-reachpay-openapi.yml
  type: http
slug: reachware-inc-authentication
source_filename: reachware-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/reachware-inc-reachpay-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Merchant API token: Authorization: Bearer {reachToken}'\n  sources:\n  - openapi/reachware-inc-reachpay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reachware-inc/refs/heads/main/authentication/reachware-inc-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Payments
- iPaaS
- Integration
- Fintech
- Payment Gateway
- Tokenization
- Saudi Arabia
---
