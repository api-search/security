---
api_key_in:
- header
api_specs:
- filename: defacto-accounting-api-openapi.yml
  format: yaml
  label: Defacto Accounting API
  slug: defacto-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/openapi/defacto-accounting-api-openapi.yml
- filename: defacto-billing-api-openapi.yml
  format: yaml
  label: Defacto Billing API
  slug: defacto-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/openapi/defacto-billing-api-openapi.yml
- filename: defacto-business-and-accounts-api-openapi.yml
  format: yaml
  label: Defacto Business and accounts API
  slug: defacto-business-and-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/openapi/defacto-business-and-accounts-api-openapi.yml
- filename: defacto-counterparty-api-openapi.yml
  format: yaml
  label: Defacto Counterparty API
  slug: defacto-counterparty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/openapi/defacto-counterparty-api-openapi.yml
- filename: defacto-credit-card-api-openapi.yml
  format: yaml
  label: Defacto Credit card API
  slug: defacto-credit-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/openapi/defacto-credit-card-api-openapi.yml
- filename: defacto-eligibility-and-credit-limit-api-openapi.yml
  format: yaml
  label: Defacto Eligibility and credit limit API
  slug: defacto-eligibility-and-credit-limit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/openapi/defacto-eligibility-and-credit-limit-api-openapi.yml
- filename: defacto-financial-product-api-openapi.yml
  format: yaml
  label: Defacto Financial product API
  slug: defacto-financial-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/openapi/defacto-financial-product-api-openapi.yml
- filename: defacto-invoice-api-openapi.yml
  format: yaml
  label: Defacto Invoice API
  slug: defacto-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/openapi/defacto-invoice-api-openapi.yml
- filename: defacto-loan-api-openapi.yml
  format: yaml
  label: Defacto Loan API
  slug: defacto-loan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/openapi/defacto-loan-api-openapi.yml
- filename: defacto-onboarding-api-openapi.yml
  format: yaml
  label: Defacto Onboarding API
  slug: defacto-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/openapi/defacto-onboarding-api-openapi.yml
- filename: defacto-payment-api-openapi.yml
  format: yaml
  label: Defacto Payment API
  slug: defacto-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/openapi/defacto-payment-api-openapi.yml
- filename: defacto-recollection-api-openapi.yml
  format: yaml
  label: Defacto Recollection API
  slug: defacto-recollection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/openapi/defacto-recollection-api-openapi.yml
- filename: defacto-repay-api-openapi.yml
  format: yaml
  label: Defacto Repay API
  slug: defacto-repay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/openapi/defacto-repay-api-openapi.yml
- filename: defacto-sharing-business-data-api-openapi.yml
  format: yaml
  label: Defacto Sharing business data API
  slug: defacto-sharing-business-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/openapi/defacto-sharing-business-data-api-openapi.yml
- filename: defacto-subscription-api-openapi.yml
  format: yaml
  label: Defacto Subscription API
  slug: defacto-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/openapi/defacto-subscription-api-openapi.yml
- filename: defacto-testing-api-openapi.yml
  format: yaml
  label: Defacto Testing API
  slug: defacto-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/openapi/defacto-testing-api-openapi.yml
- filename: defacto-translation-api-openapi.yml
  format: yaml
  label: Defacto Translation API
  slug: defacto-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/openapi/defacto-translation-api-openapi.yml
- filename: defacto-webhook-api-openapi.yml
  format: yaml
  label: Defacto Webhook API
  slug: defacto-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/openapi/defacto-webhook-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Defacto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Defacto secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Defacto
provider_slug: defacto
scheme_count: 1
schemes:
- in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/defacto-openapi-original.json
  type: apiKey
slug: defacto-authentication
source_filename: defacto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/defacto-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/defacto-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/authentication/defacto-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Embedded Finance
- Lending
- Working Capital
- Invoice Financing
- Credit
- B2B Payments
- SMB
- France
- Europe
---
