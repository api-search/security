---
api_key_in: []
api_specs:
- filename: harbor-challenges-api-openapi.yml
  format: yaml
  label: Harbor Challenges API
  slug: harbor-challenges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbor/refs/heads/main/openapi/harbor-challenges-api-openapi.yml
- filename: harbor-communities-api-openapi.yml
  format: yaml
  label: Harbor Communities API
  slug: harbor-communities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbor/refs/heads/main/openapi/harbor-communities-api-openapi.yml
- filename: harbor-leaderboards-api-openapi.yml
  format: yaml
  label: Harbor Leaderboards API
  slug: harbor-leaderboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbor/refs/heads/main/openapi/harbor-leaderboards-api-openapi.yml
- filename: harbor-members-api-openapi.yml
  format: yaml
  label: Harbor Members API
  slug: harbor-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbor/refs/heads/main/openapi/harbor-members-api-openapi.yml
- filename: harbor-redemptions-api-openapi.yml
  format: yaml
  label: Harbor Redemptions API
  slug: harbor-redemptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbor/refs/heads/main/openapi/harbor-redemptions-api-openapi.yml
- filename: harbor-rewards-api-openapi.yml
  format: yaml
  label: Harbor Rewards API
  slug: harbor-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbor/refs/heads/main/openapi/harbor-rewards-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Harbor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Harbor secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Harbor
provider_slug: harbor
scheme_count: 1
schemes:
- description: Bearer token obtained via OAuth 2.0 client credentials flow. Contact Harbor to obtain API credentials.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/harbor-openapi.yml
  type: http
slug: harbor-authentication
source_filename: harbor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/harbor-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained via OAuth 2.0 client credentials flow. Contact Harbor to\n    obtain API credentials.\n  sources:\n  - openapi/harbor-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harbor/refs/heads/main/authentication/harbor-authentication.yml
summary_line: http · 1 scheme
tags:
- Community
- Engagement
- Loyalty
- Superfans
---
