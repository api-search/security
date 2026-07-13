---
api_key_in: []
api_specs:
- filename: visa-acceptance-payments-openapi.yml
  format: yaml
  label: Visa Acceptance Payments API
  slug: visa-acceptance-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visa-acceptance/refs/heads/main/openapi/visa-acceptance-payments-openapi.yml
- filename: visa-acceptance-payments-openapi.yml
  format: yaml
  label: Visa Acceptance Invoicing API
  slug: visa-acceptance-invoicing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visa-acceptance/refs/heads/main/openapi/visa-acceptance-payments-openapi.yml
- filename: visa-acceptance-payments-openapi.yml
  format: yaml
  label: Visa Acceptance Pay by Link API
  slug: visa-acceptance-pay-by-link
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visa-acceptance/refs/heads/main/openapi/visa-acceptance-payments-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Visa Acceptance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Visa Acceptance secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Visa Acceptance
provider_slug: visa-acceptance
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: RSA-signed JSON Web Token. Generate using your merchant ID and RSA key pair from the Visa Acceptance Business Center.
  name: JWT
  scheme: bearer
  sources:
  - openapi/visa-acceptance-payments-openapi.yml
  type: http
slug: visa-acceptance-authentication
source_filename: visa-acceptance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/visa-acceptance-payments-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: JWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: RSA-signed JSON Web Token. Generate using your merchant ID and RSA key pair from\n    the Visa Acceptance Business Center.\n  sources:\n  - openapi/visa-acceptance-payments-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/visa-acceptance/refs/heads/main/authentication/visa-acceptance-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- E-Commerce
- Fintech
- Credit Cards
- Invoicing
- Payment Links
- Digital Wallets
---
