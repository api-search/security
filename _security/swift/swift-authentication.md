---
anonymous_access: false
api_key_in: []
api_specs:
- filename: swift-payment-pre-validation-api-openapi.yml
  format: yaml
  label: Payment Pre-validation API
  slug: payment-pre-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-payment-pre-validation-api-openapi.yml
- filename: swift-account-numbers-api-openapi.yml
  format: yaml
  label: SWIFT Account Numbers API
  slug: swift-account-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-account-numbers-api-openapi.yml
- filename: swift-bbans-api-openapi.yml
  format: yaml
  label: SWIFT BBANs API
  slug: swift-bbans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-bbans-api-openapi.yml
- filename: swift-bics-api-openapi.yml
  format: yaml
  label: SWIFT BICs API
  slug: swift-bics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-bics-api-openapi.yml
- filename: swift-country-codes-api-openapi.yml
  format: yaml
  label: SWIFT Country Codes API
  slug: swift-country-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-country-codes-api-openapi.yml
- filename: swift-currency-codes-api-openapi.yml
  format: yaml
  label: SWIFT Currency Codes API
  slug: swift-currency-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-currency-codes-api-openapi.yml
- filename: swift-leis-api-openapi.yml
  format: yaml
  label: SWIFT LEIs API
  slug: swift-leis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-leis-api-openapi.yml
- filename: swift-national-ids-api-openapi.yml
  format: yaml
  label: SWIFT National IDs API
  slug: swift-national-ids-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-national-ids-api-openapi.yml
- filename: swift-ibans-api-openapi.yml
  format: yaml
  label: SWIFT IBANs API
  slug: swift-ibans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-ibans-api-openapi.yml
- filename: swift-account-information-api-openapi.yml
  format: yaml
  label: SWIFT Account Information API
  slug: swift-account-information-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-account-information-api-openapi.yml
- filename: swift-distributions-api-openapi.yml
  format: yaml
  label: SWIFT Distributions API
  slug: swift-distributions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-distributions-api-openapi.yml
- filename: swift-fileact-api-openapi.yml
  format: yaml
  label: SWIFT Fileact API
  slug: swift-fileact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-fileact-api-openapi.yml
- filename: swift-fin-api-openapi.yml
  format: yaml
  label: SWIFT Fin API
  slug: swift-fin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-fin-api-openapi.yml
- filename: swift-get-changed-payment-transactions-api-openapi.yml
  format: yaml
  label: SWIFT Get Changed Payment Transactions API
  slug: swift-get-changed-payment-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-get-changed-payment-transactions-api-openapi.yml
- filename: swift-get-payment-transaction-details-api-openapi.yml
  format: yaml
  label: SWIFT Get Payment Transaction Details API
  slug: swift-get-payment-transaction-details-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-get-payment-transaction-details-api-openapi.yml
- filename: swift-iban-national-ids-api-openapi.yml
  format: yaml
  label: SWIFT Iban National IDs API
  slug: swift-iban-national-ids-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-iban-national-ids-api-openapi.yml
- filename: swift-interact-api-openapi.yml
  format: yaml
  label: SWIFT Interact API
  slug: swift-interact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-interact-api-openapi.yml
- filename: swift-pmis-api-openapi.yml
  format: yaml
  label: SWIFT Pmis API
  slug: swift-pmis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-pmis-api-openapi.yml
- filename: swift-reporting-api-openapi.yml
  format: yaml
  label: SWIFT Reporting API
  slug: swift-reporting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-reporting-api-openapi.yml
- filename: swift-status-confirmations-api-openapi.yml
  format: yaml
  label: SWIFT Status Confirmations API
  slug: swift-status-confirmations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-status-confirmations-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: SWIFT Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- password
overview: SWIFT secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and password flow(s).
provider_name: SWIFT
provider_slug: swift
scheme_count: 3
schemes:
- flows:
  - flow: password
    scopes: 2
    tokenUrl: https://api.swift.com/oauth2/v1/token
  name: OAuth2
  sources:
  - openapi/swift-account-numbers-api-openapi.yml
  - openapi/swift-bbans-api-openapi.yml
  - openapi/swift-bics-api-openapi.yml
  - openapi/swift-country-codes-api-openapi.yml
  - openapi/swift-currency-codes-api-openapi.yml
  - openapi/swift-ibans-api-openapi.yml
  - openapi/swift-leis-api-openapi.yml
  - openapi/swift-national-ids-api-openapi.yml
  type: oauth2
- bearerFormat: opaque OAuth 2.0
  description: 'The access token obtained as a result of OAuth 2.0 flows. This API supports:

    * JWT-Bearer grant type [RFC 7523](https://tools.ietf.org/html/rfc7523)


    Please visit [SWIFT OAuth Token API](https://developer.swift.com/swift-oauth-token-api) page for more information and examples on how to generate an OAuth token.


    In this declaration only the basic security element to transport the bearer token of an'
  name: oauthBearerToken
  scheme: bearer
  sources:
  - openapi/swift-cash-management-api-openapi.yml
  - openapi/swift-gpi-payment-status-cct-api-openapi.yml
  - openapi/swift-gpi-transactions-api-openapi.yml
  - openapi/swift-messaging-api-openapi.yml
  - openapi/swift-payment-pre-validation-api-openapi.yml
  - openapi/swift-swiftref-api-v4-openapi.yml
  type: http
- description: 'This API uses OAuth2 with the client credentials grant type.


    Please visit [SWIFT OAuth Token API](https://developer.swift.com/swift-oauth-token-api) for more information and examples.'
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /v1/oauth2/token
  name: oauthClientCredentials
  sources:
  - openapi/swift-payment-pre-validation-api-openapi.yml
  type: oauth2
slug: swift-authentication
source_filename: swift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/swift-account-numbers-api-openapi.yml, openapi/swift-bbans-api-openapi.yml,\n  openapi/swift-bics-api-openapi.yml, openapi/swift-cash-management-api-openapi.yml, openapi/swift-country-codes-api-openapi.yml,\n  openapi/swift-currency-codes-api-openapi.yml, openapi/swift-gpi-payment-status-cct-api-openapi.yml,\n  openapi/swift-gpi-transactions-api-openapi.yml, openapi/swift-ibans-api-openapi.yml, openapi/swift-leis-api-openapi.yml,\n  openapi/swift-messaging-api-openapi.yml, openapi/swift-national-ids-api-openapi.yml ...\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  - password\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://api.swift.com/oauth2/v1/token\n    scopes: 2\n  sources:\n  - openapi/swift-account-numbers-api-openapi.yml\n  - openapi/swift-bbans-api-openapi.yml\n  - openapi/swift-bics-api-openapi.yml\n  - openapi/swift-country-codes-api-openapi.yml\n\
  \  - openapi/swift-currency-codes-api-openapi.yml\n  - openapi/swift-ibans-api-openapi.yml\n  - openapi/swift-leis-api-openapi.yml\n  - openapi/swift-national-ids-api-openapi.yml\n- name: oauthBearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: opaque OAuth 2.0\n  description: |-\n    The access token obtained as a result of OAuth 2.0 flows. This API supports:\n    * JWT-Bearer grant type [RFC 7523](https://tools.ietf.org/html/rfc7523)\n\n    Please visit [SWIFT OAuth Token API](https://developer.swift.com/swift-oauth-token-api) page for more information and examples on how to generate an OAuth token.\n\n    In this declaration only the basic security element to transport the bearer token of an\n  sources:\n  - openapi/swift-cash-management-api-openapi.yml\n  - openapi/swift-gpi-payment-status-cct-api-openapi.yml\n  - openapi/swift-gpi-transactions-api-openapi.yml\n  - openapi/swift-messaging-api-openapi.yml\n  - openapi/swift-payment-pre-validation-api-openapi.yml\n  - openapi/swift-swiftref-api-v4-openapi.yml\n\
  - name: oauthClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth2/token\n    scopes: 0\n  description: |-\n    This API uses OAuth2 with the client credentials grant type.\n\n    Please visit [SWIFT OAuth Token API](https://developer.swift.com/swift-oauth-token-api) for more information and examples.\n  sources:\n  - openapi/swift-payment-pre-validation-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/swift/authentication/swift-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Banking
- Cross-Border Payments
- Financial Messaging
- Financial Services
- GPI
- ISO 20022
- Payments
- SWIFT
---
