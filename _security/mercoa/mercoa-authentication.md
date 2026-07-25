---
api_key_in: []
api_specs:
- filename: mercoa-entities-api-openapi.yml
  format: yaml
  label: Mercoa Entities API
  slug: mercoa-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/openapi/mercoa-entities-api-openapi.yml
- filename: mercoa-entity-groups-api-openapi.yml
  format: yaml
  label: Mercoa Entity Groups API
  slug: mercoa-entity-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/openapi/mercoa-entity-groups-api-openapi.yml
- filename: mercoa-invoice-templates-api-openapi.yml
  format: yaml
  label: Mercoa Invoice Templates API
  slug: mercoa-invoice-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/openapi/mercoa-invoice-templates-api-openapi.yml
- filename: mercoa-invoices-api-openapi.yml
  format: yaml
  label: Mercoa Invoices API
  slug: mercoa-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/openapi/mercoa-invoices-api-openapi.yml
- filename: mercoa-ocr-api-openapi.yml
  format: yaml
  label: Mercoa OCR API
  slug: mercoa-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/openapi/mercoa-ocr-api-openapi.yml
- filename: mercoa-organization-api-openapi.yml
  format: yaml
  label: Mercoa Organization API
  slug: mercoa-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/openapi/mercoa-organization-api-openapi.yml
- filename: mercoa-payment-gateway-api-openapi.yml
  format: yaml
  label: Mercoa Payment Gateway API
  slug: mercoa-payment-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/openapi/mercoa-payment-gateway-api-openapi.yml
- filename: mercoa-payment-methods-api-openapi.yml
  format: yaml
  label: Mercoa Payment Methods API
  slug: mercoa-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/openapi/mercoa-payment-methods-api-openapi.yml
- filename: mercoa-transactions-api-openapi.yml
  format: yaml
  label: Mercoa Transactions API
  slug: mercoa-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/openapi/mercoa-transactions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mercoa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mercoa secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mercoa
provider_slug: mercoa
scheme_count: 1
schemes:
- bearerFormat: token
  description: 'Mercoa API key or JWT. Send as "Authorization: Bearer {token}". API keys

    are issued from the Mercoa Dashboard and are backend-only. JWTs scope

    access to an entity or entity group.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mercoa-openapi.yml
  type: http
slug: mercoa-authentication
source_filename: mercoa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mercoa-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  description: |-\n    Mercoa API key or JWT. Send as \"Authorization: Bearer {token}\". API keys\n    are issued from the Mercoa Dashboard and are backend-only. JWTs scope\n    access to an entity or entity group.\n  sources:\n  - openapi/mercoa-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/authentication/mercoa-authentication.yml
summary_line: http · 1 scheme
tags:
- Mercoa
- Embedded Finance
- Accounts Payable
- Accounts Receivable
- BillPay
- Invoicing
- Payments
- Vertical SaaS
- Vendors
- Approvals
- Disbursements
- Virtual Cards
---
