---
api_key_in: []
api_specs:
- filename: pin-payments-openapi.yaml
  format: yaml
  label: Pin Payments API
  slug: pin-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pin-payments/refs/heads/main/openapi/pin-payments-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pin Payments Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pin Payments secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pin Payments
provider_slug: pin-payments
scheme_count: 1
schemes:
- description: HTTP Basic with the API key as the username and an empty password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/pin-payments-openapi.yaml
  type: http
slug: pin-payments-authentication
source_filename: pin-payments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pin-payments-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic with the API key as the username and an empty password.\n  sources:\n  - openapi/pin-payments-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pin-payments/refs/heads/main/authentication/pin-payments-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Cards
- Subscriptions
- Refunds
---
