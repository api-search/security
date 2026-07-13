---
api_key_in:
- header
api_specs:
- filename: tithely-openapi.yml
  format: yaml
  label: Tithe.ly Transactions API
  slug: tithely-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tithely/refs/heads/main/openapi/tithely-openapi.yml
- filename: tithely-openapi.yml
  format: yaml
  label: Tithe.ly Payments & Tokenization API
  slug: tithely-payments-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tithely/refs/heads/main/openapi/tithely-openapi.yml
- filename: tithely-openapi.yml
  format: yaml
  label: Tithe.ly Organizations API
  slug: tithely-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tithely/refs/heads/main/openapi/tithely-openapi.yml
- filename: tithely-openapi.yml
  format: yaml
  label: Tithe.ly Payment Categories (Funds) API
  slug: tithely-payment-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tithely/refs/heads/main/openapi/tithely-openapi.yml
- filename: tithely-openapi.yml
  format: yaml
  label: Tithe.ly Mail API
  slug: tithely-mail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tithely/refs/heads/main/openapi/tithely-openapi.yml
- filename: tithely-openapi.yml
  format: yaml
  label: Tithe.ly Accounts API
  slug: tithely-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tithely/refs/heads/main/openapi/tithely-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tithely Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tithe.ly secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tithe.ly
provider_slug: tithely
scheme_count: 1
schemes:
- description: 'V2 requests use the header "Authorization: {API_ID}:{API_TOKEN}", where the ID and token come from the public/private API keys issued on access approval (and via the login endpoint). V1 payment calls use the private key issued on approval.'
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/tithely-openapi.yml
  type: apiKey
slug: tithely-authentication
source_filename: tithely-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tithely-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'V2 requests use the header \"Authorization: {API_ID}:{API_TOKEN}\", where the\n    ID and token come from the public/private API keys issued on access approval (and via the\n    login endpoint). V1 payment calls use the private key issued on approval.'\n  sources:\n  - openapi/tithely-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tithely/refs/heads/main/authentication/tithely-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Church Giving
- Donations
- Fundraising
- Payments
- Nonprofit
- ChMS
- Faith
---
