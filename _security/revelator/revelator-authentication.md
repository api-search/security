---
api_key_in: []
api_specs:
- filename: revelator-account-api-openapi.yml
  format: yaml
  label: Revelator Account API
  slug: revelator-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-account-api-openapi.yml
- filename: revelator-accounting-api-openapi.yml
  format: yaml
  label: Revelator Accounting API
  slug: revelator-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-accounting-api-openapi.yml
- filename: revelator-analytics-api-openapi.yml
  format: yaml
  label: Revelator Analytics API
  slug: revelator-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-analytics-api-openapi.yml
- filename: revelator-distribution-api-openapi.yml
  format: yaml
  label: Revelator Distribution API
  slug: revelator-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-distribution-api-openapi.yml
- filename: revelator-integrations-api-openapi.yml
  format: yaml
  label: Revelator Integrations API
  slug: revelator-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-integrations-api-openapi.yml
- filename: revelator-lookup-api-openapi.yml
  format: yaml
  label: Revelator Lookup API
  slug: revelator-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-lookup-api-openapi.yml
- filename: revelator-revenue-api-openapi.yml
  format: yaml
  label: Revelator Revenue API
  slug: revelator-revenue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-revenue-api-openapi.yml
- filename: revelator-royalty-tokens-api-openapi.yml
  format: yaml
  label: Revelator Royalty Tokens API
  slug: revelator-royalty-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-royalty-tokens-api-openapi.yml
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
