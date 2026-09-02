---
api_key_in:
- header
api_specs:
- filename: open-loyalty-authorization-api-openapi.yml
  format: yaml
  label: Open Loyalty Authorization API
  slug: open-loyalty-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-authorization-api-openapi.yml
- filename: open-loyalty-earning-rules-api-openapi.yml
  format: yaml
  label: Open Loyalty Earning Rules API
  slug: open-loyalty-earning-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-earning-rules-api-openapi.yml
- filename: open-loyalty-members-api-openapi.yml
  format: yaml
  label: Open Loyalty Members API
  slug: open-loyalty-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-members-api-openapi.yml
- filename: open-loyalty-points-api-openapi.yml
  format: yaml
  label: Open Loyalty Points API
  slug: open-loyalty-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-points-api-openapi.yml
- filename: open-loyalty-rewards-api-openapi.yml
  format: yaml
  label: Open Loyalty Rewards API
  slug: open-loyalty-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-rewards-api-openapi.yml
- filename: open-loyalty-tiers-api-openapi.yml
  format: yaml
  label: Open Loyalty Tiers API
  slug: open-loyalty-tiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-tiers-api-openapi.yml
- filename: open-loyalty-transactions-api-openapi.yml
  format: yaml
  label: Open Loyalty Transactions API
  slug: open-loyalty-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-transactions-api-openapi.yml
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
- API-First
---
