---
api_key_in:
- header
api_specs:
- filename: altbank-guard-openapi.yml
  format: yaml
  label: alt.bank GUARD API
  slug: altbank-guard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altbank/refs/heads/main/openapi/altbank-guard-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Altbank Authentication
name_suffix: Authentication
oauth_flows: []
overview: alt.bank secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: alt.bank
provider_slug: altbank
scheme_count: 1
schemes:
- description: Partner authentication token — a 64-character alphanumeric string issued by alt.bank, sent on every request in the `X-Partner-Auth` header.
  in: header
  name: PartnerAuth
  parameter: X-Partner-Auth
  sources:
  - openapi/altbank-guard-openapi.yml
  type: apiKey
slug: altbank-authentication
source_filename: altbank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/altbank-guard-openapi.yml\ndocs: https://developers.altbank.ai/docs/guard-api\nnotes: >-\n  GUARD authenticates every request with a static partner API key in the\n  X-Partner-Auth header (a 64-character alphanumeric token issued by alt.bank).\n  No OAuth or OIDC surface is documented on the public developer portal.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: PartnerAuth\n  type: apiKey\n  in: header\n  parameter: X-Partner-Auth\n  description: Partner authentication token — a 64-character alphanumeric string issued by alt.bank,\n    sent on every request in the `X-Partner-Auth` header.\n  sources:\n  - openapi/altbank-guard-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altbank/refs/heads/main/authentication/altbank-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Banking
- Credit Cards
- Card Issuing
- Underwriting
- Payments
- Brazil
- KYC
---
