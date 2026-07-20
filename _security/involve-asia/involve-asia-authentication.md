---
api_key_in: []
api_specs:
- filename: involve-asia-publisher-openapi.yml
  format: yaml
  label: Involve Asia Publisher API
  slug: involve-asia-publisher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/involve-asia/refs/heads/main/openapi/involve-asia-publisher-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Involve Asia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Involve Asia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Involve Asia
provider_slug: involve-asia
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/involve-asia-publisher-openapi.yml
  type: http
slug: involve-asia-authentication
source_filename: involve-asia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/involve-asia-publisher-openapi.yml\ndocs: https://api.involve.asia/docs/#auth\nsummary:\n  types:\n  - http\n  scheme: bearer\n  bearer_format: JWT\nflow:\n  type: key-secret-exchange\n  steps:\n    - POST /authenticate with form fields key + secret returns {data:{token}}.\n    - Send Authorization Bearer <token> on every other call.\n  token_ttl: 2 hours\n  caching: Cache the token ~110 minutes and refresh proactively (or on 401).\n  key_management: https://app.involve.asia/v2/publisher/api-keys\n  reauth_on_401: Re-authenticate once and retry the original request.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/involve-asia-publisher-openapi.yml\nnotes:\n  - Requests are application/x-www-form-urlencoded; use --data-urlencode so secrets with + / = are not mangled.\n  - JWT auth errors may break the standard envelope (e.g. {message,status_code} or {error}).\
  \ See errors/involve-asia-problem-types.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/involve-asia/refs/heads/main/authentication/involve-asia-authentication.yml
summary_line: http · 1 scheme
tags:
- Affiliate Marketing
- Performance Marketing
- Partnership Marketing
- Publishers
- Creators
- Conversions
- Deeplinks
- Commissions
- Ecommerce
- Southeast Asia
- Shopee
- Company
---
