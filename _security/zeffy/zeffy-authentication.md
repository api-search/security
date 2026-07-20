---
api_key_in: []
api_specs:
- filename: zeffy-openapi.yml
  format: yaml
  label: Zeffy Payments API
  slug: zeffy-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeffy/refs/heads/main/openapi/zeffy-openapi.yml
- filename: zeffy-openapi.yml
  format: yaml
  label: Zeffy Contacts API
  slug: zeffy-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeffy/refs/heads/main/openapi/zeffy-openapi.yml
- filename: zeffy-openapi.yml
  format: yaml
  label: Zeffy Campaigns API
  slug: zeffy-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeffy/refs/heads/main/openapi/zeffy-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zeffy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zeffy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zeffy
provider_slug: zeffy
scheme_count: 1
schemes:
- description: 'Per-organization API key generated under Settings then Integrations, sent as "Authorization: Bearer [example key]".'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zeffy-openapi.yml
  type: http
slug: zeffy-authentication
source_filename: zeffy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zeffy-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Per-organization API key generated under Settings then Integrations, sent as\n    \"Authorization: Bearer [example key]\".'\n  sources:\n  - openapi/zeffy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeffy/refs/heads/main/authentication/zeffy-authentication.yml
summary_line: http · 1 scheme
tags:
- Fundraising
- Nonprofit
- Donations
- Payments
- Donor Management
- Free
- Webhooks
---
