---
api_key_in: []
api_specs:
- filename: get-on-board-openapi-original.yml
  format: yaml
  label: Get on Board API
  slug: get-on-board-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/get-on-board/refs/heads/main/openapi/get-on-board-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Get On Board Authentication
name_suffix: Authentication
oauth_flows: []
overview: Get On Board secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Get On Board
provider_slug: get-on-board
scheme_count: 3
schemes:
- audience: company
  bearerFormat: API key
  description: 'Company authentication for the private Companies API. Send `Authorization: Bearer <api_key>`. The key is on the company profile page under the "API access" section. Requires an active subscription plan that includes API access; endpoints return 404 if the subscription expires.'
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/get-on-board-openapi-original.yml
  type: http
- audience: professional
  bearerFormat: JWT
  description: Professional JWT token obtained/refreshed via POST /api/v0/auth_tokens. Used for professional-facing endpoints (matching jobs, webhook endpoints).
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/get-on-board-openapi-original.yml
  type: http
- audience: board
  bearerFormat: Board secret
  description: 'Board+ HMAC secret key. Send `Authorization: Bearer <board_secret_key>`. A legacy query-string form (?secret_key=...) is still accepted but discouraged because secrets leak into logs, history, and referrers.'
  name: BoardSecretKey
  scheme: bearer
  sources:
  - openapi/get-on-board-openapi-original.yml
  type: http
slug: get-on-board-authentication
source_filename: get-on-board-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/get-on-board-openapi-original.yml\ndocs: https://www.getonbrd.com/api-doc.html\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  bearer_formats:\n  - API key\n  - JWT\n  - Board secret\n  oauth2_flows: []\n  api_key_location: https://www.getonbrd.com/companies/[your-company]/api_settings\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  audience: company\n  description: >-\n    Company authentication for the private Companies API. Send\n    `Authorization: Bearer <api_key>`. The key is on the company profile page\n    under the \"API access\" section. Requires an active subscription plan that\n    includes API access; endpoints return 404 if the subscription expires.\n  sources:\n  - openapi/get-on-board-openapi-original.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  audience: professional\n  description: >-\n    Professional JWT token\
  \ obtained/refreshed via POST /api/v0/auth_tokens.\n    Used for professional-facing endpoints (matching jobs, webhook endpoints).\n  sources:\n  - openapi/get-on-board-openapi-original.yml\n- name: BoardSecretKey\n  type: http\n  scheme: bearer\n  bearerFormat: Board secret\n  audience: board\n  description: >-\n    Board+ HMAC secret key. Send `Authorization: Bearer <board_secret_key>`.\n    A legacy query-string form (?secret_key=...) is still accepted but\n    discouraged because secrets leak into logs, history, and referrers.\n  sources:\n  - openapi/get-on-board-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/get-on-board/refs/heads/main/authentication/get-on-board-authentication.yml
summary_line: http · 3 schemes
tags:
- Company
- Recruitment
- Jobs
- Hiring
- ATS
- Talent
- Developers
- Latin America
---
