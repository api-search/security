---
api_key_in:
- header
api_specs:
- filename: danske-bank-uk-opendata-openapi.json
  format: json
  label: Danske Bank (UK) Open Data API
  slug: danske-bank-uk-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-opendata-openapi.json
- filename: danske-bank-uk-account-transaction-openapi.json
  format: json
  label: Danske Bank (UK) Account and Transaction API
  slug: danske-bank-uk-account-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-account-transaction-openapi.json
- filename: danske-bank-uk-payment-initiation-openapi.json
  format: json
  label: Danske Bank (UK) Payment Initiation API
  slug: danske-bank-uk-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-payment-initiation-openapi.json
- filename: danske-bank-uk-confirmation-of-funds-openapi.json
  format: json
  label: Danske Bank (UK) Confirmation of Funds API
  slug: danske-bank-uk-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-confirmation-of-funds-openapi.json
- filename: danske-bank-uk-variable-recurring-payments-openapi.json
  format: json
  label: Danske Bank (UK) Variable Recurring Payments API
  slug: danske-bank-uk-variable-recurring-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-variable-recurring-payments-openapi.json
- filename: danske-bank-uk-events-openapi.json
  format: json
  label: Danske Bank (UK) Events API
  slug: danske-bank-uk-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-events-openapi.json
- filename: danske-bank-uk-account-transaction-balance-premium-openapi.json
  format: json
  label: Danske Bank (UK) Account Transaction & Balance API
  slug: danske-bank-uk-account-transaction-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-account-transaction-balance-premium-openapi.json
- filename: danske-bank-uk-payment-collection-premium-openapi.json
  format: json
  label: Danske Bank (UK) Payment Collection API
  slug: danske-bank-uk-payment-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-payment-collection-premium-openapi.json
- filename: danske-bank-uk-premium-payment-initiation-openapi.json
  format: json
  label: Danske Bank (UK) Premium Payment Initiation API
  slug: danske-bank-uk-premium-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-premium-payment-initiation-openapi.json
- filename: danske-bank-uk-fx-trade-report-openapi.json
  format: json
  label: Danske Bank (UK) FX Trade Report API
  slug: danske-bank-uk-fx-trade-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-fx-trade-report-openapi.json
- filename: danske-bank-uk-fx-trade-execution-openapi.json
  format: json
  label: Danske Bank (UK) FX Trade Execution API
  slug: danske-bank-uk-fx-trade-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/openapi/danske-bank-uk-fx-trade-execution-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Danske Bank Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Danske Bank (UK) secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Danske Bank (UK)
provider_slug: danske-bank-uk
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: 'JWT Authorization header using the Bearer scheme. Example: "Authorization: Bearer {token}"'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/danske-bank-uk-account-transaction-balance-premium-openapi.json
  - openapi/danske-bank-uk-account-transaction-openapi.json
  - openapi/danske-bank-uk-confirmation-of-funds-openapi.json
  - openapi/danske-bank-uk-events-openapi.json
  - openapi/danske-bank-uk-fx-trade-execution-openapi.json
  - openapi/danske-bank-uk-fx-trade-report-openapi.json
  - openapi/danske-bank-uk-payment-collection-premium-openapi.json
  - openapi/danske-bank-uk-payment-initiation-openapi.json
  - openapi/danske-bank-uk-premium-payment-initiation-openapi.json
  - openapi/danske-bank-uk-variable-recurring-payments-openapi.json
  type: http
- in: header
  name: clientIdHeader
  parameter: X-IBM-Client-Id
  sources:
  - openapi/danske-bank-uk-opendata-openapi.json
  type: apiKey
- description: BC2702Z
  in: header
  name: clientSecretHeader
  parameter: X-IBM-Client-Secret
  sources:
  - openapi/danske-bank-uk-opendata-openapi.json
  type: apiKey
slug: danske-bank-uk-authentication
source_filename: danske-bank-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: derived\nsource: openapi/danske-bank-uk-account-transaction-balance-premium-openapi.json, openapi/danske-bank-uk-account-transaction-openapi.json,\n  openapi/danske-bank-uk-confirmation-of-funds-openapi.json, openapi/danske-bank-uk-events-openapi.json,\n  openapi/danske-bank-uk-fx-trade-execution-openapi.json, openapi/danske-bank-uk-fx-trade-report-openapi.json,\n  openapi/danske-bank-uk-opendata-openapi.json, openapi/danske-bank-uk-payment-collection-premium-openapi.json,\n  openapi/danske-bank-uk-payment-initiation-openapi.json, openapi/danske-bank-uk-premium-payment-initiation-openapi.json,\n  openapi/danske-bank-uk-variable-recurring-payments-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'JWT Authorization header using the Bearer scheme. Example: \"Authorization: Bearer\n    {token}\"'\n  sources:\n  - openapi/danske-bank-uk-account-transaction-balance-premium-openapi.json\n\
  \  - openapi/danske-bank-uk-account-transaction-openapi.json\n  - openapi/danske-bank-uk-confirmation-of-funds-openapi.json\n  - openapi/danske-bank-uk-events-openapi.json\n  - openapi/danske-bank-uk-fx-trade-execution-openapi.json\n  - openapi/danske-bank-uk-fx-trade-report-openapi.json\n  - openapi/danske-bank-uk-payment-collection-premium-openapi.json\n  - openapi/danske-bank-uk-payment-initiation-openapi.json\n  - openapi/danske-bank-uk-premium-payment-initiation-openapi.json\n  - openapi/danske-bank-uk-variable-recurring-payments-openapi.json\n- name: clientIdHeader\n  type: apiKey\n  in: header\n  parameter: X-IBM-Client-Id\n  sources:\n  - openapi/danske-bank-uk-opendata-openapi.json\n- name: clientSecretHeader\n  type: apiKey\n  in: header\n  parameter: X-IBM-Client-Secret\n  description: BC2702Z\n  sources:\n  - openapi/danske-bank-uk-opendata-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/danske-bank-uk/refs/heads/main/authentication/danske-bank-uk-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- CMA9
- United Kingdom
- Northern Ireland
- Payments
- Account Information
- FAPI
- Fintech
---
