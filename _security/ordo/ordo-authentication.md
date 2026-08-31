---
api_key_in:
- header
- query
api_specs:
- filename: ordo-account-data-client-hosted-api-openapi.yml
  format: yaml
  label: Ordo Account Data - Client Hosted API
  slug: ordo-account-data-client-hosted-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-account-data-client-hosted-api-openapi.yml
- filename: ordo-account-data-ordo-hosted-api-openapi.yml
  format: yaml
  label: Ordo Account Data - Ordo Hosted API
  slug: ordo-account-data-ordo-hosted-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-account-data-ordo-hosted-api-openapi.yml
- filename: ordo-account-verification-client-hosted-api-openapi.yml
  format: yaml
  label: Ordo Account Verification - Client Hosted API
  slug: ordo-account-verification-client-hosted-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-account-verification-client-hosted-api-openapi.yml
- filename: ordo-account-verification-ordo-hosted-api-openapi.yml
  format: yaml
  label: Ordo Account Verification - Ordo Hosted API
  slug: ordo-account-verification-ordo-hosted-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-account-verification-ordo-hosted-api-openapi.yml
- filename: ordo-bank-accounts-api-openapi.yml
  format: yaml
  label: Ordo Bank accounts API
  slug: ordo-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-bank-accounts-api-openapi.yml
- filename: ordo-client-hosted-api-openapi.yml
  format: yaml
  label: Ordo Client hosted API
  slug: ordo-client-hosted-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-client-hosted-api-openapi.yml
- filename: ordo-create-a-mandate-api-openapi.yml
  format: yaml
  label: Ordo Create a mandate API
  slug: ordo-create-a-mandate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-create-a-mandate-api-openapi.yml
- filename: ordo-ordo-hosted-api-openapi.yml
  format: yaml
  label: Ordo Ordo hosted API
  slug: ordo-ordo-hosted-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-ordo-hosted-api-openapi.yml
- filename: ordo-retrieve-mandate-details-api-openapi.yml
  format: yaml
  label: Ordo Retrieve mandate details API
  slug: ordo-retrieve-mandate-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-retrieve-mandate-details-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ordo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ordo secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ordo
provider_slug: ordo
scheme_count: 2
schemes:
- in: header
  name: apiKeyHeader
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/ordo-account-data-client-hosted.yml
  - openapi/ordo-account-data-ordo-hosted.yml
  - openapi/ordo-recurring-payment-mandates.yml
  - openapi/ordo-registry-manager.yml
  - openapi/ordo-single-payments.yml
  - openapi/ordo-smart-request-manager.yml
  type: apiKey
- in: query
  name: apiKeyQuery
  parameter: subscription-key
  sources:
  - openapi/ordo-account-data-client-hosted.yml
  - openapi/ordo-account-data-ordo-hosted.yml
  - openapi/ordo-recurring-payment-mandates.yml
  - openapi/ordo-registry-manager.yml
  - openapi/ordo-single-payments.yml
  - openapi/ordo-smart-request-manager.yml
  type: apiKey
slug: ordo-authentication
source_filename: ordo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: derived\nsource: openapi/ordo-account-data-client-hosted.yml, openapi/ordo-account-data-ordo-hosted.yml,\n  openapi/ordo-recurring-payment-mandates.yml, openapi/ordo-registry-manager.yml, openapi/ordo-single-payments.yml,\n  openapi/ordo-smart-request-manager.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  sources:\n  - openapi/ordo-account-data-client-hosted.yml\n  - openapi/ordo-account-data-ordo-hosted.yml\n  - openapi/ordo-recurring-payment-mandates.yml\n  - openapi/ordo-registry-manager.yml\n  - openapi/ordo-single-payments.yml\n  - openapi/ordo-smart-request-manager.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  sources:\n  - openapi/ordo-account-data-client-hosted.yml\n  - openapi/ordo-account-data-ordo-hosted.yml\n  - openapi/ordo-recurring-payment-mandates.yml\n \
  \ - openapi/ordo-registry-manager.yml\n  - openapi/ordo-single-payments.yml\n  - openapi/ordo-smart-request-manager.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/authentication/ordo-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Payments
- United Kingdom
- Open Banking
- Account-to-Account
- Payment Initiation
- Variable Recurring Payments
- Request to Pay
- Real-Time Payments
- Faster Payments
- PSD2
- Account Information
---
