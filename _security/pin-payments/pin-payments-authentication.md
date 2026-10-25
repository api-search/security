---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pin-payments-cards-api-openapi.yml
  format: yaml
  label: Pin Payments Cards API
  slug: pin-payments-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pin-payments/refs/heads/main/openapi/pin-payments-cards-api-openapi.yml
- filename: pin-payments-charges-api-openapi.yml
  format: yaml
  label: Pin Payments Charges API
  slug: pin-payments-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pin-payments/refs/heads/main/openapi/pin-payments-charges-api-openapi.yml
- filename: pin-payments-customers-api-openapi.yml
  format: yaml
  label: Pin Payments Customers API
  slug: pin-payments-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pin-payments/refs/heads/main/openapi/pin-payments-customers-api-openapi.yml
- filename: pin-payments-refunds-api-openapi.yml
  format: yaml
  label: Pin Payments Refunds API
  slug: pin-payments-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pin-payments/refs/heads/main/openapi/pin-payments-refunds-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Pin Payments Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pin Payments secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pin Payments
provider_slug: pin-payments
scheme_count: 1
schemes:
- description: HTTP basic access authentication, with your API key as the username and an empty string as the password.
  environments:
    live: api.pinpayments.com
    test: test-api.pinpayments.com
  failure:
    body:
      error: unauthenticated
      error_description: Not authorised. (Check API Key).
    status: 401
  key_types:
    publishable: Your publishable keys only have the ability to store payment card details (with the cards API ) and bank account details (with the bank accounts API ).
    secret: Your secret keys have the ability to use all of the API. This means they can create charges, refunds, and bank transfers.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/pin-payments-openapi.yaml
  transport: You must use HTTPS ... We recommend using TLS 1.2.
  type: http
slug: pin-payments-authentication
source_filename: pin-payments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: searched\nsource: https://pinpayments.com/developers/api-reference\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP basic access authentication, with your API key as the username and an empty string as the password.\n  sources:\n  - openapi/pin-payments-openapi.yaml\n  key_types:\n    secret: Your secret keys have the ability to use all of the API. This means they can create charges, refunds,\n      and bank transfers.\n    publishable: Your publishable keys only have the ability to store payment card details (with the cards API )\n      and bank account details (with the bank accounts API ).\n  environments:\n    live: api.pinpayments.com\n    test: test-api.pinpayments.com\n  failure:\n    status: 401\n    body:\n      error: unauthenticated\n      error_description: Not authorised. (Check API Key).\n  transport: You must use HTTPS ... We recommend using TLS 1.2.\ndocs: https://pinpayments.com/developers/api-reference\n\
  webhook_signing:\n  header: Pin-Signature\n  algorithm: HMAC-SHA256 over \"<t>.<body>\" with the endpoint signing key\n  format: t=1500452255,v1=f07f5d147c613d85b9607d1c6b8c15fc342eca4d2cfaaf546f8dded19a30c350\n  docs: https://pinpayments.com/developers/integration-guides/webhooks\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pin-payments/refs/heads/main/authentication/pin-payments-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Cards
- Subscription
- Refunds
- Payment Gateway
- Recurring Payments
- Ecommerce
- Australia
---
