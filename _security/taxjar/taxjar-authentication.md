---
api_key_in: []
api_specs:
- filename: taxjar-sales-tax-openapi.yml
  format: yaml
  label: TaxJar Sales Tax API
  slug: taxjar-sales-tax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxjar/refs/heads/main/openapi/taxjar-sales-tax-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Taxjar Authentication
name_suffix: Authentication
oauth_flows: []
overview: TaxJar secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TaxJar
provider_slug: taxjar
scheme_count: 1
schemes:
- description: 'Use your TaxJar API token. Format: "Bearer [token]" or "Token token=[token]"'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/taxjar-sales-tax-openapi.yml
  type: http
slug: taxjar-authentication
source_filename: taxjar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/taxjar-sales-tax-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Use your TaxJar API token. Format: \"Bearer [token]\" or \"Token token=[token]\"'\n  sources:\n  - openapi/taxjar-sales-tax-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taxjar/refs/heads/main/authentication/taxjar-authentication.yml
summary_line: http · 1 scheme
tags:
- Sales Tax
- Tax Compliance
- E-Commerce
- Tax Calculation
- Tax Automation
- Stripe
- FinTech
---
