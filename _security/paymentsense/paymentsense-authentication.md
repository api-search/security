---
api_key_in:
- header
api_specs:
- filename: paymentsense-access-token-api-openapi.yml
  format: yaml
  label: Paymentsense Access Token API
  slug: paymentsense-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/openapi/paymentsense-access-token-api-openapi.yml
- filename: paymentsense-cross-reference-payment-api-openapi.yml
  format: yaml
  label: Paymentsense Cross Reference Payment API
  slug: paymentsense-cross-reference-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/openapi/paymentsense-cross-reference-payment-api-openapi.yml
- filename: paymentsense-hospitality-reports-api-openapi.yml
  format: yaml
  label: Paymentsense Hospitality Reports API
  slug: paymentsense-hospitality-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/openapi/paymentsense-hospitality-reports-api-openapi.yml
- filename: paymentsense-hospitality-tables-api-openapi.yml
  format: yaml
  label: Paymentsense Hospitality Tables API
  slug: paymentsense-hospitality-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/openapi/paymentsense-hospitality-tables-api-openapi.yml
- filename: paymentsense-pac-reports-api-openapi.yml
  format: yaml
  label: Paymentsense PAC Reports API
  slug: paymentsense-pac-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/openapi/paymentsense-pac-reports-api-openapi.yml
- filename: paymentsense-pac-reports-ingenico-only-api-openapi.yml
  format: yaml
  label: Paymentsense PAC Reports (Ingenico Only) API
  slug: paymentsense-pac-reports-ingenico-only-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/openapi/paymentsense-pac-reports-ingenico-only-api-openapi.yml
- filename: paymentsense-pac-terminals-api-openapi.yml
  format: yaml
  label: Paymentsense PAC Terminals API
  slug: paymentsense-pac-terminals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/openapi/paymentsense-pac-terminals-api-openapi.yml
- filename: paymentsense-pac-transactions-api-openapi.yml
  format: yaml
  label: Paymentsense PAC Transactions API
  slug: paymentsense-pac-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/openapi/paymentsense-pac-transactions-api-openapi.yml
- filename: paymentsense-pat-reports-api-openapi.yml
  format: yaml
  label: Paymentsense PAT Reports API
  slug: paymentsense-pat-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/openapi/paymentsense-pat-reports-api-openapi.yml
- filename: paymentsense-pat-tables-api-openapi.yml
  format: yaml
  label: Paymentsense PAT Tables API
  slug: paymentsense-pat-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/openapi/paymentsense-pat-tables-api-openapi.yml
- filename: paymentsense-payment-details-api-openapi.yml
  format: yaml
  label: Paymentsense Payment Details API
  slug: paymentsense-payment-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/openapi/paymentsense-payment-details-api-openapi.yml
- filename: paymentsense-payment-methods-api-openapi.yml
  format: yaml
  label: Paymentsense Payment Methods API
  slug: paymentsense-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/openapi/paymentsense-payment-methods-api-openapi.yml
- filename: paymentsense-resume-payment-api-openapi.yml
  format: yaml
  label: Paymentsense Resume Payment API
  slug: paymentsense-resume-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/openapi/paymentsense-resume-payment-api-openapi.yml
- filename: paymentsense-retail-reports-api-openapi.yml
  format: yaml
  label: Paymentsense Retail Reports API
  slug: paymentsense-retail-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/openapi/paymentsense-retail-reports-api-openapi.yml
- filename: paymentsense-retail-terminals-api-openapi.yml
  format: yaml
  label: Paymentsense Retail Terminals API
  slug: paymentsense-retail-terminals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/openapi/paymentsense-retail-terminals-api-openapi.yml
- filename: paymentsense-retail-transactions-api-openapi.yml
  format: yaml
  label: Paymentsense Retail Transactions API
  slug: paymentsense-retail-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/openapi/paymentsense-retail-transactions-api-openapi.yml
- filename: paymentsense-revoke-access-token-api-openapi.yml
  format: yaml
  label: Paymentsense Revoke Access Token API
  slug: paymentsense-revoke-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/openapi/paymentsense-revoke-access-token-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Paymentsense Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paymentsense secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Paymentsense
provider_slug: paymentsense
scheme_count: 3
schemes:
- in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/paymentsense-connect-e-v0.json
  type: apiKey
- bearerFormat: JWT
  name: jwt
  scheme: bearer
  sources:
  - openapi/paymentsense-connect-e-v0.json
  type: http
- name: connectBasicAuth
  scheme: basic
  sources:
  - openapi/paymentsense-connect-v0.json
  - openapi/paymentsense-connect-v1.json
  - openapi/paymentsense-connect-v2.json
  type: http
slug: paymentsense-authentication
source_filename: paymentsense-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: derived\nsource: openapi/paymentsense-connect-e-v0.json, openapi/paymentsense-connect-v0.json, openapi/paymentsense-connect-v1.json,\n  openapi/paymentsense-connect-v2.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/paymentsense-connect-e-v0.json\n- name: jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/paymentsense-connect-e-v0.json\n- name: connectBasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/paymentsense-connect-v0.json\n  - openapi/paymentsense-connect-v1.json\n  - openapi/paymentsense-connect-v2.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/authentication/paymentsense-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Payments
- United Kingdom
- Payment Gateway
- Payment Processing
- Card Payments
- Acquiring
- Point-of-Sale
- In-Person Payments
---
