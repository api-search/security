---
api_key_in:
- header
api_specs:
- filename: open-loyalty-openapi.yml
  format: yaml
  label: Open Loyalty Customer API
  slug: open-loyalty-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-openapi.yml
- filename: open-loyalty-openapi.yml
  format: yaml
  label: Open Loyalty Transactions API
  slug: open-loyalty-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-openapi.yml
- filename: open-loyalty-openapi.yml
  format: yaml
  label: Open Loyalty Points Transfers API
  slug: open-loyalty-points-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-openapi.yml
- filename: open-loyalty-openapi.yml
  format: yaml
  label: Open Loyalty Reward Campaigns API
  slug: open-loyalty-reward-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-openapi.yml
- filename: open-loyalty-openapi.yml
  format: yaml
  label: Open Loyalty Levels API
  slug: open-loyalty-levels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-openapi.yml
- filename: open-loyalty-openapi.yml
  format: yaml
  label: Open Loyalty Earning Rules API
  slug: open-loyalty-earning-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Open Loyalty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Open Loyalty secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Open Loyalty
provider_slug: open-loyalty
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'JWT obtained from POST /admin/login_check (admin) or POST /{storeCode}/customer/login_check (member), sent as Authorization: Bearer <token>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/open-loyalty-openapi.yml
  type: http
- description: Permanent API token issued to an admin account.
  in: header
  name: permanentToken
  parameter: X-AUTH-TOKEN
  sources:
  - openapi/open-loyalty-openapi.yml
  type: apiKey
slug: open-loyalty-authentication
source_filename: open-loyalty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/open-loyalty-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'JWT obtained from POST /admin/login_check (admin) or POST /{storeCode}/customer/login_check\n    (member), sent as Authorization: Bearer <token>.'\n  sources:\n  - openapi/open-loyalty-openapi.yml\n- name: permanentToken\n  type: apiKey\n  in: header\n  parameter: X-AUTH-TOKEN\n  description: Permanent API token issued to an admin account.\n  sources:\n  - openapi/open-loyalty-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/authentication/open-loyalty-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Loyalty
- Gamification
- Rewards
- Points
- Loyalty Program
- Customer Engagement
- Headless
- API First
---
