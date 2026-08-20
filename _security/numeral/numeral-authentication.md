---
api_key_in: []
api_specs:
- filename: numeral-customers-api-openapi.yml
  format: yaml
  label: Numeral Customers API
  slug: numeral-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numeral/refs/heads/main/openapi/numeral-customers-api-openapi.yml
- filename: numeral-health-api-openapi.yml
  format: yaml
  label: Numeral Health API
  slug: numeral-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numeral/refs/heads/main/openapi/numeral-health-api-openapi.yml
- filename: numeral-products-api-openapi.yml
  format: yaml
  label: Numeral Products API
  slug: numeral-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numeral/refs/heads/main/openapi/numeral-products-api-openapi.yml
- filename: numeral-refunds-api-openapi.yml
  format: yaml
  label: Numeral Refunds API
  slug: numeral-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numeral/refs/heads/main/openapi/numeral-refunds-api-openapi.yml
- filename: numeral-tax-calculations-api-openapi.yml
  format: yaml
  label: Numeral Tax Calculations API
  slug: numeral-tax-calculations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numeral/refs/heads/main/openapi/numeral-tax-calculations-api-openapi.yml
- filename: numeral-transactions-api-openapi.yml
  format: yaml
  label: Numeral Transactions API
  slug: numeral-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numeral/refs/heads/main/openapi/numeral-transactions-api-openapi.yml
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
- E-Commerce
- Software-as-a-Service
---
