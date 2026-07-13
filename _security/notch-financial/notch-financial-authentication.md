---
api_key_in: []
api_specs:
- filename: notch-financial-openapi.yml
  format: yaml
  label: Notch Invoices API
  slug: invoices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notch-financial/refs/heads/main/openapi/notch-financial-openapi.yml
- filename: notch-financial-openapi.yml
  format: yaml
  label: Notch Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notch-financial/refs/heads/main/openapi/notch-financial-openapi.yml
- filename: notch-financial-openapi.yml
  format: yaml
  label: Notch Customers API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notch-financial/refs/heads/main/openapi/notch-financial-openapi.yml
- filename: notch-financial-openapi.yml
  format: yaml
  label: Notch Payment Methods API
  slug: payment-methods
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notch-financial/refs/heads/main/openapi/notch-financial-openapi.yml
- filename: notch-financial-openapi.yml
  format: yaml
  label: Notch Bank Accounts API
  slug: bank-accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notch-financial/refs/heads/main/openapi/notch-financial-openapi.yml
- filename: notch-financial-openapi.yml
  format: yaml
  label: Notch Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notch-financial/refs/heads/main/openapi/notch-financial-openapi.yml
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
