---
api_key_in: []
api_specs:
- filename: rybbit-openapi.yml
  format: yaml
  label: Rybbit Event Tracking API
  slug: rybbit-event-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/openapi/rybbit-openapi.yml
- filename: rybbit-openapi.yml
  format: yaml
  label: Rybbit Sites API
  slug: rybbit-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/openapi/rybbit-openapi.yml
- filename: rybbit-openapi.yml
  format: yaml
  label: Rybbit Analytics Stats API
  slug: rybbit-analytics-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/openapi/rybbit-openapi.yml
- filename: rybbit-openapi.yml
  format: yaml
  label: Rybbit Sessions & Retention API
  slug: rybbit-sessions-retention-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/openapi/rybbit-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rybbit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rybbit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rybbit
provider_slug: rybbit
scheme_count: 1
schemes:
- description: 'User-scoped API key with organization-level access. Keys begin with "rb_" and are 35 characters long. Send as `Authorization: Bearer [example key]`. A `?api_key=` query parameter is also accepted for quick testing only. API keys and rate limits apply to the Stats API on Rybbit Cloud; self-hosted instances have no rate limits.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/rybbit-openapi.yml
  type: http
slug: rybbit-authentication
source_filename: rybbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rybbit-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'User-scoped API key with organization-level access. Keys begin with \"rb_\" and\n    are 35 characters long. Send as `Authorization: Bearer [example key]`. A `?api_key=` query parameter\n    is also accepted for quick testing only. API keys and rate limits apply to the Stats API\n    on Rybbit Cloud; self-hosted instances have no rate limits.'\n  sources:\n  - openapi/rybbit-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/authentication/rybbit-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Web Analytics
- Product Analytics
- Privacy
- Open Source
- Cookieless
---
