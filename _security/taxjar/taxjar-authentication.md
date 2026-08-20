---
api_key_in: []
api_specs:
- filename: taxjar-categories-api-openapi.yml
  format: yaml
  label: TaxJar Categories API
  slug: taxjar-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxjar/refs/heads/main/openapi/taxjar-categories-api-openapi.yml
- filename: taxjar-customers-api-openapi.yml
  format: yaml
  label: TaxJar Customers API
  slug: taxjar-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxjar/refs/heads/main/openapi/taxjar-customers-api-openapi.yml
- filename: taxjar-nexus-api-openapi.yml
  format: yaml
  label: TaxJar Nexus API
  slug: taxjar-nexus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxjar/refs/heads/main/openapi/taxjar-nexus-api-openapi.yml
- filename: taxjar-rates-api-openapi.yml
  format: yaml
  label: TaxJar Rates API
  slug: taxjar-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxjar/refs/heads/main/openapi/taxjar-rates-api-openapi.yml
- filename: taxjar-summary-rates-api-openapi.yml
  format: yaml
  label: TaxJar Summary Rates API
  slug: taxjar-summary-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxjar/refs/heads/main/openapi/taxjar-summary-rates-api-openapi.yml
- filename: taxjar-taxes-api-openapi.yml
  format: yaml
  label: TaxJar Taxes API
  slug: taxjar-taxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxjar/refs/heads/main/openapi/taxjar-taxes-api-openapi.yml
- filename: taxjar-transactions-orders-api-openapi.yml
  format: yaml
  label: TaxJar Transactions - Orders API
  slug: taxjar-transactions-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxjar/refs/heads/main/openapi/taxjar-transactions-orders-api-openapi.yml
- filename: taxjar-transactions-refunds-api-openapi.yml
  format: yaml
  label: TaxJar Transactions - Refunds API
  slug: taxjar-transactions-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxjar/refs/heads/main/openapi/taxjar-transactions-refunds-api-openapi.yml
- filename: taxjar-validations-api-openapi.yml
  format: yaml
  label: TaxJar Validations API
  slug: taxjar-validations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taxjar/refs/heads/main/openapi/taxjar-validations-api-openapi.yml
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
- Fintech
---
