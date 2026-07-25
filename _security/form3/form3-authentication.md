---
api_key_in: []
api_specs:
- filename: form3-payments.yml
  format: yaml
  label: Form3 Public API
  slug: form3-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/openapi/form3-payments.yml
- filename: form3-payments.yml
  format: yaml
  label: Form3 Payments API
  slug: form3-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/openapi/form3-payments.yml
- filename: form3-payments.yml
  format: yaml
  label: Form3 Direct Debits & Mandates API
  slug: form3-direct-debits-mandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/openapi/form3-payments.yml
- filename: form3-payments.yml
  format: yaml
  label: Form3 Account Identification & Verification API
  slug: form3-account-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/openapi/form3-payments.yml
- filename: form3-payments.yml
  format: yaml
  label: Form3 Files API
  slug: form3-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/openapi/form3-payments.yml
- filename: form3-payments.yml
  format: yaml
  label: Form3 Event Notifications API
  slug: form3-event-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/openapi/form3-payments.yml
- filename: form3-payments.yml
  format: yaml
  label: Form3 Security & Access API
  slug: form3-security-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/openapi/form3-payments.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Form3 Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Form3 secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Form3
provider_slug: form3
scheme_count: 2
schemes:
- name: Basic
  scheme: basic
  sources:
  - openapi/form3-payments.yml
  type: http
- description: OAuth 2.0 with Client Credentials Grant type
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.form3.tech/v1/oauth2/token
  name: OAuth2
  sources:
  - openapi/form3-payments.yml
  type: oauth2
slug: form3-authentication
source_filename: form3-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: derived\nsource: openapi/form3-payments.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: Basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/form3-payments.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.form3.tech/v1/oauth2/token\n    scopes: 0\n  description: OAuth 2.0 with Client Credentials Grant type\n  sources:\n  - openapi/form3-payments.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/authentication/form3-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Payments
- United Kingdom
- Payment Processing
- Account-to-Account
- Real-Time Payments
- Faster Payments
- Bacs
- SEPA
- Direct Debit
- Confirmation of Payee
- Cross-Border
- Banking-as-a-Service
- Embedded Payments
---
