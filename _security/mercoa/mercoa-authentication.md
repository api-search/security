---
api_key_in: []
api_specs:
- filename: mercoa-openapi.yml
  format: yaml
  label: Mercoa API
  slug: mercoa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercoa/refs/heads/main/openapi/mercoa-openapi.yml
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
