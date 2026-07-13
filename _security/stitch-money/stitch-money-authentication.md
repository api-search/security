---
api_key_in: []
api_specs:
- filename: stitch-money-openapi.yml
  format: yaml
  label: Stitch Payments (Pay By Bank)
  slug: payments-pay-by-bank
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stitch-money/refs/heads/main/openapi/stitch-money-openapi.yml
- filename: stitch-money-openapi.yml
  format: yaml
  label: Stitch Account Verification API
  slug: account-verification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stitch-money/refs/heads/main/openapi/stitch-money-openapi.yml
- filename: stitch-money-openapi.yml
  format: yaml
  label: Stitch Financial Data API
  slug: financial-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stitch-money/refs/heads/main/openapi/stitch-money-openapi.yml
- filename: stitch-money-openapi.yml
  format: yaml
  label: Stitch Payouts and Disbursements API
  slug: payouts-disbursements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stitch-money/refs/heads/main/openapi/stitch-money-openapi.yml
- filename: stitch-money-openapi.yml
  format: yaml
  label: Stitch Refunds API
  slug: refunds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stitch-money/refs/heads/main/openapi/stitch-money-openapi.yml
- filename: stitch-money-openapi.yml
  format: yaml
  label: Stitch Webhooks and Subscriptions API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stitch-money/refs/heads/main/openapi/stitch-money-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Stitch Money Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stitch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stitch
provider_slug: stitch-money
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth2 access token. Client tokens are obtained via the client_credentials grant (scoped, e.g. client_paymentrequest); user access tokens via the authorization-code grant with PKCE.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/stitch-money-openapi.yml
  type: http
slug: stitch-money-authentication
source_filename: stitch-money-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stitch-money-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth2 access token. Client tokens are obtained via the client_credentials grant\n    (scoped, e.g. client_paymentrequest); user access tokens via the authorization-code grant\n    with PKCE.\n  sources:\n  - openapi/stitch-money-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stitch-money/refs/heads/main/authentication/stitch-money-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Open Banking
- Pay By Bank
- GraphQL
- Africa
- South Africa
- Fintech
---
