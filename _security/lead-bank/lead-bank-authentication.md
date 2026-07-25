---
api_key_in: []
api_specs:
- filename: lead-bank-account-number-api-openapi.yml
  format: yaml
  label: Lead Bank Account Number API
  slug: lead-bank-account-number-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-account-number-api-openapi.yml
- filename: lead-bank-ach-api-openapi.yml
  format: yaml
  label: Lead Bank ACH API
  slug: lead-bank-ach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-ach-api-openapi.yml
- filename: lead-bank-blockchain-payment-api-openapi.yml
  format: yaml
  label: Lead Bank Blockchain Payment API
  slug: lead-bank-blockchain-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-blockchain-payment-api-openapi.yml
- filename: lead-bank-compliance-api-openapi.yml
  format: yaml
  label: Lead Bank Compliance API
  slug: lead-bank-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-compliance-api-openapi.yml
- filename: lead-bank-entity-api-openapi.yml
  format: yaml
  label: Lead Bank Entity API
  slug: lead-bank-entity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-entity-api-openapi.yml
- filename: lead-bank-events-api-openapi.yml
  format: yaml
  label: Lead Bank Events API
  slug: lead-bank-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-events-api-openapi.yml
- filename: lead-bank-funding-api-openapi.yml
  format: yaml
  label: Lead Bank Funding API
  slug: lead-bank-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-funding-api-openapi.yml
- filename: lead-bank-instant-payments-api-openapi.yml
  format: yaml
  label: Lead Bank Instant Payments API
  slug: lead-bank-instant-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-instant-payments-api-openapi.yml
- filename: lead-bank-internal-transfer-api-openapi.yml
  format: yaml
  label: Lead Bank Internal Transfer API
  slug: lead-bank-internal-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-internal-transfer-api-openapi.yml
- filename: lead-bank-lending-api-openapi.yml
  format: yaml
  label: Lead Bank Lending API
  slug: lead-bank-lending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-lending-api-openapi.yml
- filename: lead-bank-lending-simulation-api-openapi.yml
  format: yaml
  label: Lead Bank Lending Simulation API
  slug: lead-bank-lending-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-lending-simulation-api-openapi.yml
- filename: lead-bank-oauth-api-openapi.yml
  format: yaml
  label: Lead Bank OAuth API
  slug: lead-bank-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-oauth-api-openapi.yml
- filename: lead-bank-originator-api-openapi.yml
  format: yaml
  label: Lead Bank Originator API
  slug: lead-bank-originator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-originator-api-openapi.yml
- filename: lead-bank-simulation-api-openapi.yml
  format: yaml
  label: Lead Bank Simulation API
  slug: lead-bank-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-simulation-api-openapi.yml
- filename: lead-bank-subledger-balances-api-openapi.yml
  format: yaml
  label: Lead Bank Subledger Balances API
  slug: lead-bank-subledger-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-subledger-balances-api-openapi.yml
- filename: lead-bank-wire-api-openapi.yml
  format: yaml
  label: Lead Bank Wire API
  slug: lead-bank-wire-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-wire-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lead Bank Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lead Bank secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lead Bank
provider_slug: lead-bank
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lead-bank-openapi.json
  type: http
slug: lead-bank-authentication
source_filename: lead-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lead-bank-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/lead-bank-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/authentication/lead-bank-authentication.yml
summary_line: http · 1 scheme
tags:
- Banking
- Sponsor Bank
- Embedded Finance
- Banking as a Service
- Payments
- Lending
- Cards
- Deposits
---
