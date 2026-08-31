---
api_key_in: []
api_specs:
- filename: pinch-payments-connect-api-openapi.yml
  format: yaml
  label: Pinch Payments Connect API
  slug: pinch-payments-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-connect-api-openapi.yml
- filename: pinch-payments-contacts-api-openapi.yml
  format: yaml
  label: Pinch Payments Contacts API
  slug: pinch-payments-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-contacts-api-openapi.yml
- filename: pinch-payments-events-api-openapi.yml
  format: yaml
  label: Pinch Payments Events API
  slug: pinch-payments-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-events-api-openapi.yml
- filename: pinch-payments-fees-api-openapi.yml
  format: yaml
  label: Pinch Payments Fees API
  slug: pinch-payments-fees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-fees-api-openapi.yml
- filename: pinch-payments-health-api-openapi.yml
  format: yaml
  label: Pinch Payments Health API
  slug: pinch-payments-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-health-api-openapi.yml
- filename: pinch-payments-merchant-financial-data-api-openapi.yml
  format: yaml
  label: Pinch Payments Merchant Financial Data API
  slug: pinch-payments-merchant-financial-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-merchant-financial-data-api-openapi.yml
- filename: pinch-payments-merchants-api-openapi.yml
  format: yaml
  label: Pinch Payments Merchants API
  slug: pinch-payments-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-merchants-api-openapi.yml
- filename: pinch-payments-payers-api-openapi.yml
  format: yaml
  label: Pinch Payments Payers API
  slug: pinch-payments-payers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-payers-api-openapi.yml
- filename: pinch-payments-payment-links-api-openapi.yml
  format: yaml
  label: Pinch Payments Payment Links API
  slug: pinch-payments-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-payment-links-api-openapi.yml
- filename: pinch-payments-payments-api-openapi.yml
  format: yaml
  label: Pinch Payments Payments API
  slug: pinch-payments-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-payments-api-openapi.yml
- filename: pinch-payments-plans-api-openapi.yml
  format: yaml
  label: Pinch Payments Plans API
  slug: pinch-payments-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-plans-api-openapi.yml
- filename: pinch-payments-refund-api-openapi.yml
  format: yaml
  label: Pinch Payments Refund API
  slug: pinch-payments-refund-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-refund-api-openapi.yml
- filename: pinch-payments-refunds-api-openapi.yml
  format: yaml
  label: Pinch Payments Refunds API
  slug: pinch-payments-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-refunds-api-openapi.yml
- filename: pinch-payments-subscriptions-api-openapi.yml
  format: yaml
  label: Pinch Payments Subscriptions API
  slug: pinch-payments-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-subscriptions-api-openapi.yml
- filename: pinch-payments-tokens-api-openapi.yml
  format: yaml
  label: Pinch Payments Tokens API
  slug: pinch-payments-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-tokens-api-openapi.yml
- filename: pinch-payments-transfers-api-openapi.yml
  format: yaml
  label: Pinch Payments Transfers API
  slug: pinch-payments-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-transfers-api-openapi.yml
- filename: pinch-payments-webhooks-api-openapi.yml
  format: yaml
  label: Pinch Payments Webhooks API
  slug: pinch-payments-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-webhooks-api-openapi.yml
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
- Subscription
- Billing
- Payment Facilitator
- Account-to-Account
- New Zealand
---
