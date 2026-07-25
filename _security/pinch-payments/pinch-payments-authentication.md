---
api_key_in: []
api_specs:
- filename: pinch-payments-core.yml
  format: yaml
  label: Pinch Core API
  slug: pinch-payments-core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-core.yml
- filename: pinch-payments-payments.yml
  format: yaml
  label: Pinch Payments API
  slug: pinch-payments-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-payments.yml
- filename: pinch-payments-payers.yml
  format: yaml
  label: Pinch Payers API
  slug: pinch-payments-payers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-payers.yml
- filename: pinch-payments-payment-links.yml
  format: yaml
  label: Pinch Payment Links API
  slug: pinch-payments-payment-links
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-payment-links.yml
- filename: pinch-payments-merchants.yml
  format: yaml
  label: Pinch Merchants API
  slug: pinch-payments-merchants
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-merchants.yml
- filename: pinch-payments-webhooks.yml
  format: yaml
  label: Pinch Webhooks API
  slug: pinch-payments-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-webhooks.yml
- filename: pinch-payments-contacts.yml
  format: yaml
  label: Pinch Contacts API
  slug: pinch-payments-contacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-contacts.yml
- filename: pinch-payments-transfers.yml
  format: yaml
  label: Pinch Transfers API
  slug: pinch-payments-transfers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-transfers.yml
- filename: pinch-payments-merchant-financial-data.yml
  format: yaml
  label: Pinch Merchant Financial Data API
  slug: pinch-payments-merchant-financial-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-merchant-financial-data.yml
- filename: pinch-payments-authentication.yml
  format: yaml
  label: Pinch Authentication API
  slug: pinch-payments-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-authentication.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Pinch Payments Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Pinch Payments secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Pinch Payments
provider_slug: pinch-payments
scheme_count: 2
schemes:
- flows:
    clientCredentials:
      scopes:
        api1: Full access to the Pinch REST API
      tokenUrl: https://auth.getpinch.com.au/connect/token
  name: OAuth2 client-credentials
  sources:
  - openapi/pinch-payments-contacts.yml
  - openapi/pinch-payments-core.yml
  - openapi/pinch-payments-merchant-financial-data.yml
  - openapi/pinch-payments-merchants.yml
  - openapi/pinch-payments-payers.yml
  - openapi/pinch-payments-payment-links.yml
  - openapi/pinch-payments-payments.yml
  - openapi/pinch-payments-transfers.yml
  - openapi/pinch-payments-webhooks.yml
  type: oauth2
- name: HTTP Basic (token endpoint only)
  note: Used only at the /connect/token endpoint to present the Application ID + Secret Key when exchanging for a Bearer token; not used against the resource API.
  scheme: basic
  sources:
  - openapi/pinch-payments-authentication.yml
  type: http
slug: pinch-payments-authentication
source_filename: pinch-payments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/pinch-payments-authentication.yml + https://docs.getpinch.com.au/docs/application-authentication\ndocs: https://docs.getpinch.com.au/docs/application-authentication\nsummary:\n  types:\n  - oauth2\n  - http\n  model: OAuth 2.0 client-credentials\n  detail: >-\n    Every Pinch API request requires a Bearer JWT. Obtain one by POSTing to the\n    token endpoint (auth.getpinch.com.au/connect/token) with grant_type=client_credentials\n    and scope=api1, authenticating with your Application ID + Secret Key via HTTP\n    Basic (base64(client_id:client_secret)) or as client_id/client_secret in the\n    x-www-form-urlencoded body. The response is a Bearer token that expires in 3600s;\n    cache and reuse it. Send it as `Authorization: Bearer <token>` on every request.\n    Authenticating with a Merchant ID as client_id is DEPRECATED — new integrations\n    must use an Application. Client-side card/bank tokenisation (CaptureJS)\
  \ uses a\n    separate Merchant Publishable key (pk_test_.../pk_live_...).\n  oauth2_flows: [clientCredentials]\n  token_url: https://auth.getpinch.com.au/connect/token\n  token_ttl_seconds: 3600\n  scopes: [api1]\nschemes:\n- name: OAuth2 client-credentials\n  type: oauth2\n  flows:\n    clientCredentials:\n      tokenUrl: https://auth.getpinch.com.au/connect/token\n      scopes:\n        api1: Full access to the Pinch REST API\n  sources:\n  - openapi/pinch-payments-contacts.yml\n  - openapi/pinch-payments-core.yml\n  - openapi/pinch-payments-merchant-financial-data.yml\n  - openapi/pinch-payments-merchants.yml\n  - openapi/pinch-payments-payers.yml\n  - openapi/pinch-payments-payment-links.yml\n  - openapi/pinch-payments-payments.yml\n  - openapi/pinch-payments-transfers.yml\n  - openapi/pinch-payments-webhooks.yml\n- name: HTTP Basic (token endpoint only)\n  type: http\n  scheme: basic\n  note: >-\n    Used only at the /connect/token endpoint to present the Application ID + Secret\n\
  \    Key when exchanging for a Bearer token; not used against the resource API.\n  sources:\n  - openapi/pinch-payments-authentication.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/authentication/pinch-payments-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Payments
- Australia
- Payment Gateway
- Payment Processing
- Direct Debit
- Card Payments
- Subscriptions
- Billing
- Payment Facilitator
- Account-to-Account
- New Zealand
---
