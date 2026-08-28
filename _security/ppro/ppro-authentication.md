---
api_key_in: []
api_specs:
- filename: ppro-payment-charges-openapi.yml
  format: yaml
  label: PPRO Global API
  slug: ppro-global-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-payment-charges-openapi.yml
- filename: ppro-onboarding-openapi.yml
  format: yaml
  label: PPRO Onboarding API
  slug: ppro-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-onboarding-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ppro Authentication
name_suffix: Authentication
oauth_flows: []
overview: PPRO secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PPRO
provider_slug: ppro
scheme_count: 1
schemes:
- name: bearer_token
  scheme: bearer
  sources:
  - openapi/ppro-payment-agreements-openapi.yml
  - openapi/ppro-payment-charges-openapi.yml
  - openapi/ppro-payment-instruments-openapi.yml
  - openapi/ppro-payment-sessions-openapi.yml
  type: http
slug: ppro-authentication
source_filename: ppro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/ppro-payment-agreements-openapi.yml, openapi/ppro-payment-charges-openapi.yml,\n  openapi/ppro-payment-instruments-openapi.yml, openapi/ppro-payment-sessions-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer_token\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/ppro-payment-agreements-openapi.yml\n  - openapi/ppro-payment-charges-openapi.yml\n  - openapi/ppro-payment-instruments-openapi.yml\n  - openapi/ppro-payment-sessions-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/authentication/ppro-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Local Payment Methods
- Financial Services
- Fintech
- Acquiring
- Checkout
- E-commerce
- Digital Wallets
- Recurring Payments
- Disputes
- Chargebacks
- Company
---
