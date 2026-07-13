---
api_key_in: []
api_specs:
- filename: bonusly-openapi.yml
  format: yaml
  label: Bonusly Bonuses API
  slug: bonusly-bonuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonusly/refs/heads/main/openapi/bonusly-openapi.yml
- filename: bonusly-openapi.yml
  format: yaml
  label: Bonusly Users API
  slug: bonusly-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonusly/refs/heads/main/openapi/bonusly-openapi.yml
- filename: bonusly-openapi.yml
  format: yaml
  label: Bonusly Rewards API
  slug: bonusly-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonusly/refs/heads/main/openapi/bonusly-openapi.yml
- filename: bonusly-openapi.yml
  format: yaml
  label: Bonusly Redemptions API
  slug: bonusly-redemptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonusly/refs/heads/main/openapi/bonusly-openapi.yml
- filename: bonusly-openapi.yml
  format: yaml
  label: Bonusly Analytics API
  slug: bonusly-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonusly/refs/heads/main/openapi/bonusly-openapi.yml
- filename: bonusly-openapi.yml
  format: yaml
  label: Bonusly Company API
  slug: bonusly-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonusly/refs/heads/main/openapi/bonusly-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bonusly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bonusly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bonusly
provider_slug: bonusly
scheme_count: 1
schemes:
- description: A Bonusly personal access token (PAT) passed as a Bearer token in the Authorization header. Tokens carry read / write / administer scopes per resource and are minted by a Global or Tech admin. A token that lacks the required scope returns 403 Forbidden.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bonusly-openapi.yml
  type: http
slug: bonusly-authentication
source_filename: bonusly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bonusly-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: A Bonusly personal access token (PAT) passed as a Bearer token in the Authorization\n    header. Tokens carry read / write / administer scopes per resource and are minted by a Global\n    or Tech admin. A token that lacks the required scope returns 403 Forbidden.\n  sources:\n  - openapi/bonusly-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bonusly/refs/heads/main/authentication/bonusly-authentication.yml
summary_line: http · 1 scheme
tags:
- Employee Recognition
- Rewards
- Employee Engagement
- HR
- Company Culture
- Bonuses
---
