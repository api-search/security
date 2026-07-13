---
api_key_in: []
api_specs:
- filename: payu-europe-rest-api.yaml
  format: yaml
  label: PayU Europe REST API
  slug: payu-europe-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-europe-rest-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Payu Authentication
name_suffix: Authentication
oauth_flows: []
overview: PayU secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PayU
provider_slug: payu
scheme_count: 2
schemes:
- name: Bearer
  scheme: bearer
  sources:
  - openapi/payu-europe-rest-api.yaml
  type: http
- name: Basic
  scheme: basic
  sources:
  - openapi/payu-europe-rest-api.yaml
  type: http
slug: payu-authentication
source_filename: payu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/payu-europe-rest-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/payu-europe-rest-api.yaml\n- name: Basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/payu-europe-rest-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/authentication/payu-authentication.yml
summary_line: http · 2 schemes
tags:
- Payments
- Payment Processing
- Fintech
- Financial Services
- Subscriptions
- Fraud Detection
- Checkout
- Marketplace
- Tokenization
- Emerging Markets
---
