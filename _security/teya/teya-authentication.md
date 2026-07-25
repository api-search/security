---
api_key_in: []
api_specs:
- filename: teya-captures-api-openapi.yml
  format: yaml
  label: Teya Captures API
  slug: teya-captures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-captures-api-openapi.yml
- filename: teya-dcc-api-openapi.yml
  format: yaml
  label: Teya DCC API
  slug: teya-dcc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-dcc-api-openapi.yml
- filename: teya-epos-registration-api-openapi.yml
  format: yaml
  label: Teya ePOS Registration API
  slug: teya-epos-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-epos-registration-api-openapi.yml
- filename: teya-hosted-checkout-api-openapi.yml
  format: yaml
  label: Teya Hosted Checkout API
  slug: teya-hosted-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-hosted-checkout-api-openapi.yml
- filename: teya-internal-api-openapi.yml
  format: yaml
  label: Teya '@internal' API
  slug: teya-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-internal-api-openapi.yml
- filename: teya-pay-at-table-api-openapi.yml
  format: yaml
  label: Teya Pay at Table API
  slug: teya-pay-at-table-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-pay-at-table-api-openapi.yml
- filename: teya-paybylink-api-openapi.yml
  format: yaml
  label: Teya PayByLink API
  slug: teya-paybylink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-paybylink-api-openapi.yml
- filename: teya-payment-requests-api-openapi.yml
  format: yaml
  label: Teya Payment Requests API
  slug: teya-payment-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-payment-requests-api-openapi.yml
- filename: teya-print-receipts-epos-api-openapi.yml
  format: yaml
  label: Teya Print Receipts (ePOS) API
  slug: teya-print-receipts-epos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-print-receipts-epos-api-openapi.yml
- filename: teya-public-api-openapi.yml
  format: yaml
  label: Teya '@public' API
  slug: teya-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-public-api-openapi.yml
- filename: teya-refunds-api-openapi.yml
  format: yaml
  label: Teya Refunds API
  slug: teya-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-refunds-api-openapi.yml
- filename: teya-reversals-api-openapi.yml
  format: yaml
  label: Teya Reversals API
  slug: teya-reversals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-reversals-api-openapi.yml
- filename: teya-stores-api-openapi.yml
  format: yaml
  label: Teya Stores API
  slug: teya-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-stores-api-openapi.yml
- filename: teya-terminals-api-openapi.yml
  format: yaml
  label: Teya Terminals API
  slug: teya-terminals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-terminals-api-openapi.yml
- filename: teya-tokens-api-openapi.yml
  format: yaml
  label: Teya Tokens API
  slug: teya-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-tokens-api-openapi.yml
- filename: teya-transactions-api-openapi.yml
  format: yaml
  label: Teya Transactions API
  slug: teya-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-transactions-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Teya Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Teya secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Teya
provider_slug: teya
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://id.teya.xyz/oauth/v2/oauth-authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://id.teya.xyz/oauth/v2/oauth-token
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://id.teya.xyz/oauth/v2/oauth-token
  name: checkout_oauth_dev
  sources:
  - openapi/teya-online-payments-openapi.yaml
  - openapi/teya-payments-openapi.yaml
  type: oauth2
- flows:
  - authorizationUrl: https://id.teya.com/oauth/v2/oauth-authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://id.teya.com/oauth/v2/oauth-token
  name: Teya_Digital_Receipts_Service_oauth_prd
  sources:
  - openapi/teya-online-payments-openapi.yaml
  - openapi/teya-poslink-openapi.json
  type: oauth2
slug: teya-authentication
source_filename: teya-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/teya-online-payments-openapi.yaml, openapi/teya-payments-openapi.yaml, openapi/teya-poslink-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: checkout_oauth_dev\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.teya.xyz/oauth/v2/oauth-authorize\n    tokenUrl: https://id.teya.xyz/oauth/v2/oauth-token\n    scopes: 0\n  - flow: clientCredentials\n    tokenUrl: https://id.teya.xyz/oauth/v2/oauth-token\n    scopes: 0\n  sources:\n  - openapi/teya-online-payments-openapi.yaml\n  - openapi/teya-payments-openapi.yaml\n- name: Teya_Digital_Receipts_Service_oauth_prd\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.teya.com/oauth/v2/oauth-authorize\n    tokenUrl: https://id.teya.com/oauth/v2/oauth-token\n    scopes: 0\n  sources:\n  - openapi/teya-online-payments-openapi.yaml\n\
  \  - openapi/teya-poslink-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/authentication/teya-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Payments
- Payment Processing
- Card Acquiring
- Online Payments
- Point of Sale
- E-commerce
- Fintech
- Merchant Services
- Europe
---
