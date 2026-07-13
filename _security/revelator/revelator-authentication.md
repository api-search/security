---
api_key_in: []
api_specs:
- filename: revelator-openapi.yml
  format: yaml
  label: Revelator Distribution API
  slug: revelator-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-openapi.yml
- filename: revelator-openapi.yml
  format: yaml
  label: Revelator Catalog API
  slug: revelator-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-openapi.yml
- filename: revelator-openapi.yml
  format: yaml
  label: Revelator Analytics API
  slug: revelator-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-openapi.yml
- filename: revelator-openapi.yml
  format: yaml
  label: Revelator Royalties & Accounting API
  slug: revelator-royalties-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-openapi.yml
- filename: revelator-openapi.yml
  format: yaml
  label: Revelator Payments & Wallet API
  slug: revelator-payments-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Revelator Authentication
name_suffix: Authentication
oauth_flows: []
overview: Revelator secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Revelator
provider_slug: revelator
scheme_count: 1
schemes:
- description: 'Access token obtained from POST /partner/account/login (or /account/login/as), sent as ''Authorization: Bearer <token>''. Tokens are valid for 8 hours.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/revelator-openapi.yml
  type: http
slug: revelator-authentication
source_filename: revelator-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/revelator-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Access token obtained from POST /partner/account/login (or /account/login/as),\n    sent as ''Authorization: Bearer <token>''. Tokens are valid for 8 hours.'\n  sources:\n  - openapi/revelator-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/authentication/revelator-authentication.yml
summary_line: http · 1 scheme
tags:
- Music
- Distribution
- Rights
- Royalties
- Payments
- Analytics
---
