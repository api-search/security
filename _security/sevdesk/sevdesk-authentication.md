---
api_key_in: []
api_specs:
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Contacts API
  slug: sevdesk-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Invoices API
  slug: sevdesk-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Orders API
  slug: sevdesk-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Credit Notes API
  slug: sevdesk-credit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Vouchers API
  slug: sevdesk-vouchers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Bank and Transactions API
  slug: sevdesk-bank-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Parts API
  slug: sevdesk-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Tags API
  slug: sevdesk-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Export and Reports API
  slug: sevdesk-export-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sevdesk Authentication
name_suffix: Authentication
oauth_flows: []
overview: sevdesk secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: sevdesk
provider_slug: sevdesk
scheme_count: 1
schemes:
- description: 'Per-administrator sevdesk API token - a 32-character hexadecimal string found in the sevdesk web application under the user''s settings. Passed as the raw value of the `Authorization` header (no `Bearer` prefix), for example `Authorization: b7794de0085f5cd00560f160f290af38`. Tokens have an infinite lifetime and can be regenerated (confirmed with the account password) to revoke a previous token. Self-serve: any paying account administrator can obtain a token with no separate application or approval.'
  headerName: Authorization
  in: header
  name: api_key
  sources:
  - openapi/sevdesk-openapi.yml
  - https://api.sevdesk.de/
  type: apiKey
slug: sevdesk-authentication
source_filename: sevdesk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/sevdesk-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  headerName: Authorization\n  description: >-\n    Per-administrator sevdesk API token - a 32-character hexadecimal string\n    found in the sevdesk web application under the user's settings. Passed as\n    the raw value of the `Authorization` header (no `Bearer` prefix), for\n    example `Authorization: b7794de0085f5cd00560f160f290af38`. Tokens have an\n    infinite lifetime and can be regenerated (confirmed with the account\n    password) to revoke a previous token. Self-serve: any paying account\n    administrator can obtain a token with no separate application or approval.\n  sources:\n  - openapi/sevdesk-openapi.yml\n  - https://api.sevdesk.de/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/authentication/sevdesk-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Accounting
- Invoicing
- Bookkeeping
- Finance
- Germany
- Vouchers
- Contacts
- SaaS
- ERP
- Financial Software
---
