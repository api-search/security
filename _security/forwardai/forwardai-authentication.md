---
anonymous_access: false
api_key_in: []
api_specs:
- filename: forwardai-account-api-openapi.yml
  format: yaml
  label: Forwardly Account API
  slug: forwardai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forwardai/openapi/forwardai-account-api-openapi.yml
- filename: forwardai-bill-api-openapi.yml
  format: yaml
  label: Forwardly Bill API
  slug: forwardai-bill-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forwardai/openapi/forwardai-bill-api-openapi.yml
- filename: forwardai-bill-payment-api-openapi.yml
  format: yaml
  label: Forwardly Bill Payment API
  slug: forwardai-bill-payment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forwardai/openapi/forwardai-bill-payment-api-openapi.yml
- filename: forwardai-business-api-openapi.yml
  format: yaml
  label: Forwardly Business API
  slug: forwardai-business-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forwardai/openapi/forwardai-business-api-openapi.yml
- filename: forwardai-credit-note-api-openapi.yml
  format: yaml
  label: Forwardly Credit Note API
  slug: forwardai-credit-note-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forwardai/openapi/forwardai-credit-note-api-openapi.yml
- filename: forwardai-customer-analysis-api-openapi.yml
  format: yaml
  label: Forwardly Customer Analysis API
  slug: forwardai-customer-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forwardai/openapi/forwardai-customer-analysis-api-openapi.yml
- filename: forwardai-customer-api-openapi.yml
  format: yaml
  label: Forwardly Customer API
  slug: forwardai-customer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forwardai/openapi/forwardai-customer-api-openapi.yml
- filename: forwardai-debit-note-api-openapi.yml
  format: yaml
  label: Forwardly Debit Note API
  slug: forwardai-debit-note-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forwardai/openapi/forwardai-debit-note-api-openapi.yml
- filename: forwardai-derived-data-api-openapi.yml
  format: yaml
  label: Forwardly Derived Data API
  slug: forwardai-derived-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forwardai/openapi/forwardai-derived-data-api-openapi.yml
- filename: forwardai-employee-api-openapi.yml
  format: yaml
  label: Forwardly Employee API
  slug: forwardai-employee-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forwardai/openapi/forwardai-employee-api-openapi.yml
- filename: forwardai-invoice-api-openapi.yml
  format: yaml
  label: Forwardly Invoice API
  slug: forwardai-invoice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forwardai/openapi/forwardai-invoice-api-openapi.yml
- filename: forwardai-invoice-payment-api-openapi.yml
  format: yaml
  label: Forwardly Invoice Payment API
  slug: forwardai-invoice-payment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forwardai/openapi/forwardai-invoice-payment-api-openapi.yml
- filename: forwardai-item-api-openapi.yml
  format: yaml
  label: Forwardly Item API
  slug: forwardai-item-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forwardai/openapi/forwardai-item-api-openapi.yml
- filename: forwardai-journal-entries-api-openapi.yml
  format: yaml
  label: Forwardly Journal Entries API
  slug: forwardai-journal-entries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forwardai/openapi/forwardai-journal-entries-api-openapi.yml
- filename: forwardai-purchase-order-api-openapi.yml
  format: yaml
  label: Forwardly Purchase Order API
  slug: forwardai-purchase-order-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forwardai/openapi/forwardai-purchase-order-api-openapi.yml
- filename: forwardai-ratios-api-openapi.yml
  format: yaml
  label: Forwardly Ratios API
  slug: forwardai-ratios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forwardai/openapi/forwardai-ratios-api-openapi.yml
- filename: forwardai-reports-api-openapi.yml
  format: yaml
  label: Forwardly Reports API
  slug: forwardai-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forwardai/openapi/forwardai-reports-api-openapi.yml
- filename: forwardai-short-term-cash-flow-api-openapi.yml
  format: yaml
  label: Forwardly Short-Term Cash Flow API
  slug: forwardai-short-term-cash-flow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forwardai/openapi/forwardai-short-term-cash-flow-api-openapi.yml
- filename: forwardai-tax-rates-api-openapi.yml
  format: yaml
  label: Forwardly Tax Rates API
  slug: forwardai-tax-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forwardai/openapi/forwardai-tax-rates-api-openapi.yml
- filename: forwardai-vendor-api-openapi.yml
  format: yaml
  label: Forwardly Vendor API
  slug: forwardai-vendor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forwardai/openapi/forwardai-vendor-api-openapi.yml
auth_types: []
description: Forwardly authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Forwardai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Forwardly declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Forwardly
provider_slug: forwardai
scheme_count: 1
schemes:
- evidence: Credentials Basic base64 Basic
  header: Authorization
  location: header
  name: basicAuth
  type: http-basic
slug: forwardai-authentication
source_filename: forwardai-authentication.yml
source_heading: Authentication Profile
source_url: https://forwardai.readme.io/reference/post_v2-business.md
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://forwardai.readme.io/reference/post_v2-business.md\nsources:\n- https://forwardai.readme.io/reference/post_v2-business.md\n- https://docs.forwardai.com/reference/post_v2-business\ndescription: Forwardly authentication\nschemes:\n- type: http-basic\n  name: basicAuth\n  evidence: Credentials Basic base64 Basic\n  location: header\n  header: Authorization\ndocs: https://forwardai.readme.io/reference/post_v2-business.md\n"
source_yaml_url: https://artifacts.apis.io/forwardai/authentication/forwardai-authentication.yml
summary_line: 1 scheme
tags:
- Accounting
- Fintech
- Business Data
- Software-as-a-Service
- Company
---
