---
api_key_in: []
api_specs:
- filename: zepto-payments-zepto.yml
  format: yaml
  label: Zepto API
  slug: zepto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/openapi/zepto-payments-zepto.yml
- filename: zepto-payments-pay-to.yml
  format: yaml
  label: Zepto PayTo API
  slug: payto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/openapi/zepto-payments-pay-to.yml
- filename: zepto-payments-validate-cop.yml
  format: yaml
  label: Zepto Validate API (Confirmation of Payee)
  slug: validate-cop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/openapi/zepto-payments-validate-cop.yml
- filename: zepto-payments-investigations.yml
  format: yaml
  label: Zepto Investigations API
  slug: investigations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/openapi/zepto-payments-investigations.yml
- filename: zepto-payments-clients.yml
  format: yaml
  label: Zepto Clients API
  slug: clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/openapi/zepto-payments-clients.yml
- filename: zepto-payments-merchant-reports.yml
  format: yaml
  label: Zepto Merchant Reports API
  slug: merchant-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/openapi/zepto-payments-merchant-reports.yml
- filename: zepto-payments-notifications.yml
  format: yaml
  label: Zepto Notifications API (Webhooks)
  slug: notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/openapi/zepto-payments-notifications.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Zepto Payments Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Zepto secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Zepto
provider_slug: zepto-payments
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zepto-payments-clients.yml
  - openapi/zepto-payments-investigations.yml
  - openapi/zepto-payments-merchant-reports.yml
  - openapi/zepto-payments-notifications.yml
  - openapi/zepto-payments-pay-to.yml
  - openapi/zepto-payments-validate-cop.yml
  type: http
- flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    scopes: 9
    tokenUrl: /oauth/token
  name: bearerAuth
  sources:
  - openapi/zepto-payments-zepto.yml
  type: oauth2
slug: zepto-payments-authentication
source_filename: zepto-payments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\ndocs: https://docs.zeptopayments.com/docs/oauth-grant-flow\nsource: openapi/zepto-payments-clients.yml, openapi/zepto-payments-investigations.yml, openapi/zepto-payments-merchant-reports.yml,\n  openapi/zepto-payments-notifications.yml, openapi/zepto-payments-pay-to.yml, openapi/zepto-payments-validate-cop.yml,\n  openapi/zepto-payments-zepto.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/zepto-payments-clients.yml\n  - openapi/zepto-payments-investigations.yml\n  - openapi/zepto-payments-merchant-reports.yml\n  - openapi/zepto-payments-notifications.yml\n  - openapi/zepto-payments-pay-to.yml\n  - openapi/zepto-payments-validate-cop.yml\n- name: bearerAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\n    scopes: 9\n  sources:\n  -\
  \ openapi/zepto-payments-zepto.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/authentication/zepto-payments-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Payments
- Australia
- Real-Time Payments
- Account-to-Account
- New Payments Platform
- PayTo
- PayID
- Direct Entry
- Open Banking
- Money Movement
---
