---
api_key_in: []
api_specs:
- filename: chargedesk-rest-api-openapi.yml
  format: yaml
  label: ChargeDesk REST API
  slug: chargedesk-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargedesk/refs/heads/main/openapi/chargedesk-rest-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Chargedesk Authentication
name_suffix: Authentication
oauth_flows: []
overview: ChargeDesk secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ChargeDesk
provider_slug: chargedesk
scheme_count: 1
schemes:
- description: 'Use your ChargeDesk secret key as the username with an empty password. Format: Authorization: YOUR_SECRET_KEY:'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/chargedesk-rest-api-openapi.yml
  type: http
slug: chargedesk-authentication
source_filename: chargedesk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chargedesk-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'Use your ChargeDesk secret key as the username with an empty password. Format:\n    Authorization: YOUR_SECRET_KEY:'\n  sources:\n  - openapi/chargedesk-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chargedesk/refs/heads/main/authentication/chargedesk-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Billing
- Subscriptions
- Charges
- Refunds
- Customer Management
- Payment Gateway
- Helpdesk Integration
- REST API
---
