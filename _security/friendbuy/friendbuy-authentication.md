---
api_key_in: []
api_specs:
- filename: friendbuy-openapi.yml
  format: yaml
  label: Friendbuy Customers API
  slug: friendbuy-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/openapi/friendbuy-openapi.yml
- filename: friendbuy-openapi.yml
  format: yaml
  label: Friendbuy Referrals API
  slug: friendbuy-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/openapi/friendbuy-openapi.yml
- filename: friendbuy-openapi.yml
  format: yaml
  label: Friendbuy Events API
  slug: friendbuy-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/openapi/friendbuy-openapi.yml
- filename: friendbuy-openapi.yml
  format: yaml
  label: Friendbuy Analytics API
  slug: friendbuy-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/openapi/friendbuy-openapi.yml
- filename: friendbuy-openapi.yml
  format: yaml
  label: Friendbuy Rewards & Loyalty API
  slug: friendbuy-rewards-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/openapi/friendbuy-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Friendbuy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Friendbuy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Friendbuy
provider_slug: friendbuy
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Bearer JWT obtained from POST /authorization by exchanging your account key and secret. Passed as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/friendbuy-openapi.yml
  type: http
slug: friendbuy-authentication
source_filename: friendbuy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/friendbuy-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Bearer JWT obtained from POST /authorization by exchanging your account key\n    and secret. Passed as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/friendbuy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/authentication/friendbuy-authentication.yml
summary_line: http · 1 scheme
tags:
- Referral Marketing
- Loyalty
- Rewards
- Ecommerce
- Marketing
- Advocacy
---
