---
api_key_in: []
api_specs:
- filename: notch-financial-bank-accounts-api-openapi.yml
  format: yaml
  label: Notch Bank Accounts API
  slug: notch-financial-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notch-financial/refs/heads/main/openapi/notch-financial-bank-accounts-api-openapi.yml
- filename: notch-financial-customers-api-openapi.yml
  format: yaml
  label: Notch Customers API
  slug: notch-financial-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notch-financial/refs/heads/main/openapi/notch-financial-customers-api-openapi.yml
- filename: notch-financial-invoices-api-openapi.yml
  format: yaml
  label: Notch Invoices API
  slug: notch-financial-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notch-financial/refs/heads/main/openapi/notch-financial-invoices-api-openapi.yml
- filename: notch-financial-payment-methods-api-openapi.yml
  format: yaml
  label: Notch Payment Methods API
  slug: notch-financial-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notch-financial/refs/heads/main/openapi/notch-financial-payment-methods-api-openapi.yml
- filename: notch-financial-payments-api-openapi.yml
  format: yaml
  label: Notch Payments API
  slug: notch-financial-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notch-financial/refs/heads/main/openapi/notch-financial-payments-api-openapi.yml
- filename: notch-financial-webhooks-api-openapi.yml
  format: yaml
  label: Notch Webhooks API
  slug: notch-financial-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notch-financial/refs/heads/main/openapi/notch-financial-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Notch Financial Authentication
name_suffix: Authentication
oauth_flows: []
overview: Notch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Notch
provider_slug: notch-financial
scheme_count: 1
schemes:
- description: Illustrative Bearer API key scheme. Notch's actual authentication mechanism is not publicly documented and is unverified.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/notch-financial-openapi.yml
  type: http
slug: notch-financial-authentication
source_filename: notch-financial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/notch-financial-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Illustrative Bearer API key scheme. Notch's actual authentication mechanism is\n    not publicly documented and is unverified.\n  sources:\n  - openapi/notch-financial-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notch-financial/refs/heads/main/authentication/notch-financial-authentication.yml
summary_line: http · 1 scheme
tags:
- Accounts Receivable
- Accounts Payable
- B2B Payments
- Invoicing
- FinTech
---
