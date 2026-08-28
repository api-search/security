---
api_key_in: []
api_specs:
- filename: sana-labs-assignments-api-openapi.yml
  format: yaml
  label: Sana Assignments API
  slug: sana-labs-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-assignments-api-openapi.yml
- filename: sana-labs-authentication-api-openapi.yml
  format: yaml
  label: Sana Authentication API
  slug: sana-labs-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-authentication-api-openapi.yml
- filename: sana-labs-courses-api-openapi.yml
  format: yaml
  label: Sana Courses API
  slug: sana-labs-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-courses-api-openapi.yml
- filename: sana-labs-groups-api-openapi.yml
  format: yaml
  label: Sana Groups API
  slug: sana-labs-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-groups-api-openapi.yml
- filename: sana-labs-insights-api-openapi.yml
  format: yaml
  label: Sana Insights API
  slug: sana-labs-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-insights-api-openapi.yml
- filename: sana-labs-paths-api-openapi.yml
  format: yaml
  label: Sana Paths API
  slug: sana-labs-paths-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-paths-api-openapi.yml
- filename: sana-labs-programs-api-openapi.yml
  format: yaml
  label: Sana Programs API
  slug: sana-labs-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-programs-api-openapi.yml
- filename: sana-labs-reporting-api-openapi.yml
  format: yaml
  label: Sana Reporting API
  slug: sana-labs-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-reporting-api-openapi.yml
- filename: sana-labs-teamspaces-api-openapi.yml
  format: yaml
  label: Sana Teamspaces API
  slug: sana-labs-teamspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-teamspaces-api-openapi.yml
- filename: sana-labs-users-api-openapi.yml
  format: yaml
  label: Sana Users API
  slug: sana-labs-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-users-api-openapi.yml
- filename: sana-labs-xapi-api-openapi.yml
  format: yaml
  label: Sana xAPI API
  slug: sana-labs-xapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-xapi-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sana Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sana secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sana
provider_slug: sana-labs
scheme_count: 1
schemes:
- description: 'Bearer access token obtained from POST /api/token via the OAuth 2.0 client credentials flow. Sent as: Authorization: Bearer <accessToken>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sana-labs-openapi.yml
  type: http
slug: sana-labs-authentication
source_filename: sana-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sana-labs-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer access token obtained from POST /api/token via the OAuth 2.0 client credentials\n    flow. Sent as: Authorization: Bearer <accessToken>.'\n  sources:\n  - openapi/sana-labs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/authentication/sana-labs-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Knowledge
- Learning
- LMS
- Agents
- Sweden
---
