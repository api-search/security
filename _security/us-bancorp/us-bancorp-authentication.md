---
api_key_in: []
api_specs:
- filename: us-bancorp-accounts-api-openapi.yml
  format: yaml
  label: US Bancorp Accounts API
  slug: us-bancorp-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bancorp-accounts-api-openapi.yml
- filename: us-bancorp-balances-api-openapi.yml
  format: yaml
  label: US Bancorp Balances API
  slug: us-bancorp-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bancorp-balances-api-openapi.yml
- filename: us-bancorp-credit-transfers-api-openapi.yml
  format: yaml
  label: US Bancorp Credit Transfers API
  slug: us-bancorp-credit-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bancorp-credit-transfers-api-openapi.yml
- filename: us-bancorp-exception-history-api-openapi.yml
  format: yaml
  label: US Bancorp Exception History API
  slug: us-bancorp-exception-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bancorp-exception-history-api-openapi.yml
- filename: us-bancorp-exceptions-api-openapi.yml
  format: yaml
  label: US Bancorp Exceptions API
  slug: us-bancorp-exceptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bancorp-exceptions-api-openapi.yml
- filename: us-bancorp-push-to-card-payments-api-openapi.yml
  format: yaml
  label: US Bancorp Push to Card Payments API
  slug: us-bancorp-push-to-card-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bancorp-push-to-card-payments-api-openapi.yml
- filename: us-bancorp-request-for-payment-api-openapi.yml
  format: yaml
  label: US Bancorp Request for Payment API
  slug: us-bancorp-request-for-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bancorp-request-for-payment-api-openapi.yml
- filename: us-bancorp-rtp-eligibility-api-openapi.yml
  format: yaml
  label: US Bancorp RTP Eligibility API
  slug: us-bancorp-rtp-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bancorp-rtp-eligibility-api-openapi.yml
- filename: us-bancorp-transactions-api-openapi.yml
  format: yaml
  label: US Bancorp Transactions API
  slug: us-bancorp-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bancorp-transactions-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Us Bancorp Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: US Bancorp secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: US Bancorp
provider_slug: us-bancorp
scheme_count: 1
schemes:
- description: OAuth 2.0 with MFA using SinglePoint credentials
  flows:
  - authorizationUrl: https://api.usbank.com/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.usbank.com/oauth/token
  name: OAuth2MFA
  sources:
  - openapi/us-bank-corporate-account-information-openapi.yml
  - openapi/us-bank-positive-pay-openapi.yml
  - openapi/us-bank-push-to-card-openapi.yml
  - openapi/us-bank-rtp-openapi.yml
  type: oauth2
slug: us-bancorp-authentication
source_filename: us-bancorp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/us-bank-corporate-account-information-openapi.yml, openapi/us-bank-positive-pay-openapi.yml,\n  openapi/us-bank-push-to-card-openapi.yml, openapi/us-bank-rtp-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2MFA\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.usbank.com/oauth/authorize\n    tokenUrl: https://api.usbank.com/oauth/token\n    scopes: 2\n  description: OAuth 2.0 with MFA using SinglePoint credentials\n  sources:\n  - openapi/us-bank-corporate-account-information-openapi.yml\n  - openapi/us-bank-positive-pay-openapi.yml\n  - openapi/us-bank-push-to-card-openapi.yml\n  - openapi/us-bank-rtp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/authentication/us-bancorp-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Banking
- Finance
- Fortune 500
- Corporate Banking
- Payments
- Open Banking
- Treasury Management
- Consumer Banking
---
