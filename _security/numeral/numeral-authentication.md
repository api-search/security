---
api_key_in: []
api_specs:
- filename: numeral-openapi.yml
  format: yaml
  label: Numeral Tax Calculations API
  slug: tax-calculations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numeral/refs/heads/main/openapi/numeral-openapi.yml
- filename: numeral-openapi.yml
  format: yaml
  label: Numeral Transactions API
  slug: transactions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numeral/refs/heads/main/openapi/numeral-openapi.yml
- filename: numeral-openapi.yml
  format: yaml
  label: Numeral Products & Tax Codes API
  slug: tax-codes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numeral/refs/heads/main/openapi/numeral-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Numeral Authentication
name_suffix: Authentication
oauth_flows: []
overview: Numeral secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Numeral
provider_slug: numeral
scheme_count: 1
schemes:
- description: Provide your Numeral API key as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/numeral-openapi.yml
  type: http
slug: numeral-authentication
source_filename: numeral-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/numeral-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Provide your Numeral API key as a Bearer token in the Authorization header.\n  sources:\n  - openapi/numeral-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/numeral/refs/heads/main/authentication/numeral-authentication.yml
summary_line: http · 1 scheme
tags:
- Sales Tax
- Tax Compliance
- Tax Calculation
- Ecommerce
- SaaS
---
