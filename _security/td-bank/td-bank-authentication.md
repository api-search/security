---
api_key_in: []
api_specs:
- filename: td-bank-transactions-api-openapi.yml
  format: yaml
  label: TD Bank Transactions API
  slug: transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-transactions-api-openapi.yml
- filename: td-bank-statements-api-openapi.yml
  format: yaml
  label: TD Bank Statements API
  slug: statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-statements-api-openapi.yml
- filename: td-bank-tax-forms-api-openapi.yml
  format: yaml
  label: TD Bank Tax Forms API
  slug: tax-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-tax-forms-api-openapi.yml
- filename: td-bank-rewards-api-openapi.yml
  format: yaml
  label: TD Bank Rewards API
  slug: rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-rewards-api-openapi.yml
- filename: td-bank-notifications-api-openapi.yml
  format: yaml
  label: TD Bank Notifications API
  slug: notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-notifications-api-openapi.yml
- filename: td-bank-accounts-api-openapi.yml
  format: yaml
  label: TD Bank Accounts API
  slug: td-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-accounts-api-openapi.yml
- filename: td-bank-apps-api-openapi.yml
  format: yaml
  label: TD Bank Apps API
  slug: td-bank-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-apps-api-openapi.yml
- filename: td-bank-bill-payments-api-openapi.yml
  format: yaml
  label: TD Bank Bill Payments API
  slug: td-bank-bill-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-bill-payments-api-openapi.yml
- filename: td-bank-clusters-api-openapi.yml
  format: yaml
  label: TD Bank Clusters API
  slug: td-bank-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-clusters-api-openapi.yml
- filename: td-bank-consents-api-openapi.yml
  format: yaml
  label: TD Bank Consents API
  slug: td-bank-consents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-consents-api-openapi.yml
- filename: td-bank-customers-api-openapi.yml
  format: yaml
  label: TD Bank Customers API
  slug: td-bank-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-customers-api-openapi.yml
- filename: td-bank-payees-api-openapi.yml
  format: yaml
  label: TD Bank Payees API
  slug: td-bank-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-payees-api-openapi.yml
- filename: td-bank-service-tokens-api-openapi.yml
  format: yaml
  label: TD Bank Service Tokens API
  slug: td-bank-service-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-service-tokens-api-openapi.yml
- filename: td-bank-subscriptions-api-openapi.yml
  format: yaml
  label: TD Bank Subscriptions API
  slug: td-bank-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-subscriptions-api-openapi.yml
- filename: td-bank-tokens-api-openapi.yml
  format: yaml
  label: TD Bank Tokens API
  slug: td-bank-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-tokens-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Td Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: TD Bank secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: TD Bank
provider_slug: td-bank
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/token
  name: oauth2
  sources:
  - openapi/td-bank-account-basic-api-openapi.yml
  - openapi/td-bank-account-detailed-api-openapi.yml
  - openapi/td-bank-bill-payment-api-openapi.yml
  - openapi/td-bank-consent-api-openapi.yml
  - openapi/td-bank-customer-api-openapi.yml
  - openapi/td-bank-rewards-api-openapi.yml
  - openapi/td-bank-statements-api-openapi.yml
  - openapi/td-bank-tax-forms-api-openapi.yml
  - openapi/td-bank-transactions-api-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: serviceToken
  scheme: bearer
  sources:
  - openapi/td-bank-apps-management-api-openapi.yml
  - openapi/td-bank-notifications-api-openapi.yml
  type: http
slug: td-bank-authentication
source_filename: td-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/td-bank-account-basic-api-openapi.yml, openapi/td-bank-account-detailed-api-openapi.yml,\n  openapi/td-bank-apps-management-api-openapi.yml, openapi/td-bank-bill-payment-api-openapi.yml,\n  openapi/td-bank-consent-api-openapi.yml, openapi/td-bank-customer-api-openapi.yml, openapi/td-bank-notifications-api-openapi.yml,\n  openapi/td-bank-rewards-api-openapi.yml, openapi/td-bank-statements-api-openapi.yml, openapi/td-bank-tax-forms-api-openapi.yml,\n  openapi/td-bank-transactions-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/authorize\n    tokenUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/token\n    scopes: 1\n  sources:\n  - openapi/td-bank-account-basic-api-openapi.yml\n  - openapi/td-bank-account-detailed-api-openapi.yml\n\
  \  - openapi/td-bank-bill-payment-api-openapi.yml\n  - openapi/td-bank-consent-api-openapi.yml\n  - openapi/td-bank-customer-api-openapi.yml\n  - openapi/td-bank-rewards-api-openapi.yml\n  - openapi/td-bank-statements-api-openapi.yml\n  - openapi/td-bank-tax-forms-api-openapi.yml\n  - openapi/td-bank-transactions-api-openapi.yml\n- name: serviceToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/td-bank-apps-management-api-openapi.yml\n  - openapi/td-bank-notifications-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/authentication/td-bank-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Account Aggregation
- AML
- Akoya
- Banking
- Bank Secrecy Act
- Bill Payment
- Consent
- Consumer Banking
- FDX
- Financial Services
- Merchant Solutions
- Notifications
- Open Banking
- Payments
- Rewards
- Tax Forms
- Token Management
- Transactions
---
