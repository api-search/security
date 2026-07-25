---
api_key_in: []
api_specs:
- filename: przelewy24-additional-api-functionality-api-openapi.yml
  format: yaml
  label: Przelewy24 Additional API functionality API
  slug: przelewy24-additional-api-functionality-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-additional-api-functionality-api-openapi.yml
- filename: przelewy24-additional-services-mass-payments-transactions-api-openapi.yml
  format: yaml
  label: Przelewy24 Additional services Mass Payments Transactions API
  slug: przelewy24-additional-services-mass-payments-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-additional-services-mass-payments-transactions-api-openapi.yml
- filename: przelewy24-apay-api-api-openapi.yml
  format: yaml
  label: Przelewy24 APay API API
  slug: przelewy24-apay-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-apay-api-api-openapi.yml
- filename: przelewy24-blik-api-api-openapi.yml
  format: yaml
  label: Przelewy24 BLIK API API
  slug: przelewy24-blik-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-blik-api-api-openapi.yml
- filename: przelewy24-card-api-api-openapi.yml
  format: yaml
  label: Przelewy24 Card API API
  slug: przelewy24-card-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-card-api-api-openapi.yml
- filename: przelewy24-ekspres-p24-api-api-openapi.yml
  format: yaml
  label: Przelewy24 Ekspres P24 API API
  slug: przelewy24-ekspres-p24-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-ekspres-p24-api-api-openapi.yml
- filename: przelewy24-gpay-api-api-openapi.yml
  format: yaml
  label: Przelewy24 GPay API API
  slug: przelewy24-gpay-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-gpay-api-api-openapi.yml
- filename: przelewy24-marketplace-management-api-api-openapi.yml
  format: yaml
  label: Przelewy24 Marketplace Management API API
  slug: przelewy24-marketplace-management-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-marketplace-management-api-api-openapi.yml
- filename: przelewy24-marketplace-merchant-api-api-openapi.yml
  format: yaml
  label: Przelewy24 Marketplace Merchant API API
  slug: przelewy24-marketplace-merchant-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-marketplace-merchant-api-api-openapi.yml
- filename: przelewy24-marketplace-partner-api-api-openapi.yml
  format: yaml
  label: Przelewy24 Marketplace Partner API API
  slug: przelewy24-marketplace-partner-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-marketplace-partner-api-api-openapi.yml
- filename: przelewy24-recursion-dopayment-api-openapi.yml
  format: yaml
  label: Przelewy24 Recursion (doPayment) API
  slug: przelewy24-recursion-dopayment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-recursion-dopayment-api-openapi.yml
- filename: przelewy24-report-api-api-openapi.yml
  format: yaml
  label: Przelewy24 Report API API
  slug: przelewy24-report-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-report-api-api-openapi.yml
- filename: przelewy24-transaction-service-api-api-openapi.yml
  format: yaml
  label: Przelewy24 Transaction service API API
  slug: przelewy24-transaction-service-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/przelewy24-transaction-service-api-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Przelewy24 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Przelewy24 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Przelewy24
provider_slug: przelewy24
scheme_count: 1
schemes:
- description: This is the default authentication method. User login is API REST key the password assigned to it.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/openapi-ekspres.yml
  - openapi/openapi-extended.yml
  - openapi/openapi-marketplace.yml
  - openapi/openapi.yml
  type: http
slug: przelewy24-authentication
source_filename: przelewy24-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi-ekspres.yml, openapi/openapi-extended.yml, openapi/openapi-marketplace.yml,\n  openapi/openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: This is the default authentication method. User login is API REST key the password\n    assigned to it.\n  sources:\n  - openapi/openapi-ekspres.yml\n  - openapi/openapi-extended.yml\n  - openapi/openapi-marketplace.yml\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/authentication/przelewy24-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Payment Gateway
- Bank Transfer
- BLIK
- Card Payments
- E-Commerce
- Poland
- Polish
- Multi-Currency
- Fintech
---
