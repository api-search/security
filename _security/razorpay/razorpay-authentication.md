---
api_key_in: []
api_specs:
- filename: overview
  format: yaml
  label: Razorpay Core REST API
  slug: core-api
  spec_type: Postman
  url: https://www.postman.com/razorpaydev/razorpay-public-workspace/overview
- filename: razorpay-webhooks-asyncapi.yml
  format: yaml
  label: Razorpay Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/razorpay/refs/heads/main/asyncapi/razorpay-webhooks-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Razorpay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Razorpay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Razorpay
provider_slug: razorpay
scheme_count: 1
schemes:
- description: HTTP Basic auth — username is Razorpay key_id, password is key_secret.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/razorpay-openapi.yml
  type: http
slug: razorpay-authentication
source_filename: razorpay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/razorpay-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth — username is Razorpay key_id, password is key_secret.\n  sources:\n  - openapi/razorpay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/razorpay/refs/heads/main/authentication/razorpay-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Payment Gateway
- Fintech
- India
- UPI
- Subscriptions
- Payouts
- Checkout
---
