---
api_key_in: []
api_specs:
- filename: chargedesk-charges-api-openapi.yml
  format: yaml
  label: ChargeDesk Charges API
  slug: chargedesk-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargedesk/refs/heads/main/openapi/chargedesk-charges-api-openapi.yml
- filename: chargedesk-customers-api-openapi.yml
  format: yaml
  label: ChargeDesk Customers API
  slug: chargedesk-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargedesk/refs/heads/main/openapi/chargedesk-customers-api-openapi.yml
- filename: chargedesk-gateway-api-openapi.yml
  format: yaml
  label: ChargeDesk Gateway API
  slug: chargedesk-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargedesk/refs/heads/main/openapi/chargedesk-gateway-api-openapi.yml
- filename: chargedesk-products-api-openapi.yml
  format: yaml
  label: ChargeDesk Products API
  slug: chargedesk-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargedesk/refs/heads/main/openapi/chargedesk-products-api-openapi.yml
- filename: chargedesk-subscriptions-api-openapi.yml
  format: yaml
  label: ChargeDesk Subscriptions API
  slug: chargedesk-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargedesk/refs/heads/main/openapi/chargedesk-subscriptions-api-openapi.yml
- filename: chargedesk-webhooks-api-openapi.yml
  format: yaml
  label: ChargeDesk Webhooks API
  slug: chargedesk-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargedesk/refs/heads/main/openapi/chargedesk-webhooks-api-openapi.yml
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
- Subscription
- Charges
- Refunds
- Customer Management
- Payment Gateway
- Helpdesk Integration
- REST API
---
