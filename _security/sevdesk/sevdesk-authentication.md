---
api_key_in: []
api_specs:
- filename: sevdesk-checkaccount-api-openapi.yml
  format: yaml
  label: sevdesk CheckAccount API
  slug: sevdesk-checkaccount-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-checkaccount-api-openapi.yml
- filename: sevdesk-checkaccounttransaction-api-openapi.yml
  format: yaml
  label: sevdesk CheckAccountTransaction API
  slug: sevdesk-checkaccounttransaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-checkaccounttransaction-api-openapi.yml
- filename: sevdesk-contact-api-openapi.yml
  format: yaml
  label: sevdesk Contact API
  slug: sevdesk-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-contact-api-openapi.yml
- filename: sevdesk-creditnote-api-openapi.yml
  format: yaml
  label: sevdesk CreditNote API
  slug: sevdesk-creditnote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-creditnote-api-openapi.yml
- filename: sevdesk-invoice-api-openapi.yml
  format: yaml
  label: sevdesk Invoice API
  slug: sevdesk-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-invoice-api-openapi.yml
- filename: sevdesk-order-api-openapi.yml
  format: yaml
  label: sevdesk Order API
  slug: sevdesk-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-order-api-openapi.yml
- filename: sevdesk-part-api-openapi.yml
  format: yaml
  label: sevdesk Part API
  slug: sevdesk-part-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-part-api-openapi.yml
- filename: sevdesk-tag-api-openapi.yml
  format: yaml
  label: sevdesk Tag API
  slug: sevdesk-tag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-tag-api-openapi.yml
- filename: sevdesk-voucher-api-openapi.yml
  format: yaml
  label: sevdesk Voucher API
  slug: sevdesk-voucher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-voucher-api-openapi.yml
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
