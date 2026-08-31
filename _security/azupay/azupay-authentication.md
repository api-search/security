---
api_key_in:
- header
api_specs:
- filename: azupay-api-keys-api-openapi.yml
  format: yaml
  label: Azupay API Keys API
  slug: azupay-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-api-keys-api-openapi.yml
- filename: azupay-billing-and-transaction-reports-api-openapi.yml
  format: yaml
  label: Azupay Billing and Transaction Reports API
  slug: azupay-billing-and-transaction-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-billing-and-transaction-reports-api-openapi.yml
- filename: azupay-check-accounts-api-openapi.yml
  format: yaml
  label: Azupay Check Accounts API
  slug: azupay-check-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-check-accounts-api-openapi.yml
- filename: azupay-clients-api-openapi.yml
  format: yaml
  label: Azupay Clients API
  slug: azupay-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-clients-api-openapi.yml
- filename: azupay-current-balances-api-openapi.yml
  format: yaml
  label: Azupay Current Balances API
  slug: azupay-current-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-current-balances-api-openapi.yml
- filename: azupay-payment-agreement-api-openapi.yml
  format: yaml
  label: Azupay Payment Agreement API
  slug: azupay-payment-agreement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-payment-agreement-api-openapi.yml
- filename: azupay-payment-agreement-request-api-openapi.yml
  format: yaml
  label: Azupay Payment Agreement Request API
  slug: azupay-payment-agreement-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-payment-agreement-request-api-openapi.yml
- filename: azupay-payment-api-openapi.yml
  format: yaml
  label: Azupay Payment API
  slug: azupay-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-payment-api-openapi.yml
- filename: azupay-payment-initiation-api-openapi.yml
  format: yaml
  label: Azupay Payment Initiation API
  slug: azupay-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-payment-initiation-api-openapi.yml
- filename: azupay-payment-request-api-openapi.yml
  format: yaml
  label: Azupay Payment Request API
  slug: azupay-payment-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-payment-request-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Azupay Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Azupay secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Azupay
provider_slug: azupay
scheme_count: 3
schemes:
- description: Secret (SECR) key for restricted/charging operations (including outbound payments); store encrypted, restrict to authorised systems.
  in: header
  name: SecretKey
  parameter: Authorization
  sources: &id001
  - openapi/azupay-check-accounts.yml
  - openapi/azupay-configuration.yml
  - openapi/azupay-payment-agreement.yml
  - openapi/azupay-payment-request.yml
  - openapi/azupay-payment.yml
  - openapi/azupay-reports.yml
  type: apiKey
- description: Distributable (DIST) key with limited access; may be exposed publicly to payers.
  in: header
  name: DistributableKey
  parameter: Authorization
  sources: *id001
  type: apiKey
- description: 'Additional server-to-server option (enabled per client). Short-lived JWT bearer token; oauth2TokenUrl and allowed scopes are returned by enableClientOAuth2/getClientOAuth2. Send as Authorization: Bearer <token>.'
  flow: clientCredentials
  name: OAuth2ClientCredentials
  sources:
  - 'docs: https://developer.azupay.com.au/docs/oauth-20-api'
  tokenUrl: dynamic (oauth2TokenUrl)
  type: oauth2
slug: azupay-authentication
source_filename: azupay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/azupay-check-accounts.yml, openapi/azupay-configuration.yml, openapi/azupay-payment-agreement.yml,\n  openapi/azupay-payment-request.yml, openapi/azupay-payment.yml, openapi/azupay-reports.yml\ndocs: https://developer.azupay.com.au/docs/getting-started-1, https://developer.azupay.com.au/docs/oauth-20-api\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: SecretKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Secret (SECR) key for restricted/charging operations (including outbound payments); store\n    encrypted, restrict to authorised systems.\n  sources: &id001\n  - openapi/azupay-check-accounts.yml\n  - openapi/azupay-configuration.yml\n  - openapi/azupay-payment-agreement.yml\n  - openapi/azupay-payment-request.yml\n  - openapi/azupay-payment.yml\n  - openapi/azupay-reports.yml\n- name: DistributableKey\n \
  \ type: apiKey\n  in: header\n  parameter: Authorization\n  description: Distributable (DIST) key with limited access; may be exposed publicly to payers.\n  sources: *id001\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  description: 'Additional server-to-server option (enabled per client). Short-lived JWT bearer token;\n    oauth2TokenUrl and allowed scopes are returned by enableClientOAuth2/getClientOAuth2. Send as Authorization:\n    Bearer <token>.'\n  tokenUrl: dynamic (oauth2TokenUrl)\n  sources:\n  - 'docs: https://developer.azupay.com.au/docs/oauth-20-api'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/authentication/azupay-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Payments
- Australia
- Real-Time Payments
- Account-to-Account
- New Payments Platform
- PayID
- PayTo
- Money Transfer
- Confirmation of Payee
- Open Banking
---
