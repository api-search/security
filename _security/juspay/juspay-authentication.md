---
api_key_in: []
api_specs:
- filename: juspay-openapi.yml
  format: yaml
  label: Juspay Orders API
  slug: juspay-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juspay/refs/heads/main/openapi/juspay-openapi.yml
- filename: juspay-openapi.yml
  format: yaml
  label: Juspay Transactions API
  slug: juspay-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juspay/refs/heads/main/openapi/juspay-openapi.yml
- filename: juspay-openapi.yml
  format: yaml
  label: Juspay Session API
  slug: juspay-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juspay/refs/heads/main/openapi/juspay-openapi.yml
- filename: juspay-openapi.yml
  format: yaml
  label: Juspay Refunds API
  slug: juspay-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juspay/refs/heads/main/openapi/juspay-openapi.yml
- filename: juspay-openapi.yml
  format: yaml
  label: Juspay Customers API
  slug: juspay-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juspay/refs/heads/main/openapi/juspay-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Juspay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Juspay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Juspay
provider_slug: juspay
scheme_count: 1
schemes:
- description: 'HTTP Basic authentication. The API key issued in the Juspay dashboard is the username and the password is an empty string; the `username:` pair is Base64-encoded into `Authorization: Basic <credentials>`. Requests also require an `x-merchantid` header, and Juspay recommends an `x-routing-id` header (typically the customer_id) to pin the payment session lifecycle. Client-side SDK calls instead use a short-lived (15-minute) client auth token minted by the create-order or get/create-customer endpoints.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/juspay-openapi.yml
  type: http
slug: juspay-authentication
source_filename: juspay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/juspay-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication. The API key issued in the Juspay dashboard is the\n    username and the password is an empty string; the `username:` pair is\n    Base64-encoded into `Authorization: Basic <credentials>`. Requests also\n    require an `x-merchantid` header, and Juspay recommends an `x-routing-id`\n    header (typically the customer_id) to pin the payment session lifecycle.\n    Client-side SDK calls instead use a short-lived (15-minute) client auth\n    token minted by the create-order or get/create-customer endpoints.\n  sources:\n  - openapi/juspay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/juspay/refs/heads/main/authentication/juspay-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Payment Orchestration
- Checkout
- India
- UPI
- Cards
- Payment Gateway
- Fintech
- HyperSDK
- Financial Infrastructure
---
