---
api_key_in: []
api_specs:
- filename: fieldguide-openapi-original.json
  format: json
  label: Fieldguide API
  slug: fieldguide-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Fieldguide Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fieldguide secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fieldguide
provider_slug: fieldguide
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/fieldguide-openapi-original.json
  type: http
slug: fieldguide-authentication
source_filename: fieldguide-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/fieldguide-openapi-original.json\ndocs: https://api.fieldguide.io/api\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  token_formats:\n  - jwt\n  - api-token\n  scoped: true\n  scopes_ref: scopes/fieldguide-scopes.yml\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/fieldguide-openapi-original.json\ntokens:\n- type: jwt\n  read_schema: JwtTokenRead\n  note: Short-lived JWT bearer token (user_uuid, created_at, expires_at).\n- type: api\n  read_schema: ApiTokenRead\n  note: >-\n    Named API token (uuid, name, scopes[], expires_at) granted a set of resource\n    scopes. Introspect the current token via GET /v1/token\n    (get_current_token_v1); list available scopes via GET /v1/scopes\n    (list_scopes_v1).\nauthorization:\n  model: resource-scopes\n  scopes_ref: scopes/fieldguide-scopes.yml\n  enforcement: >-\n    Operations return 403 naming the missing\
  \ scope, e.g. \"Forbidden (requires\n    scopes `engagements:write`)\".\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/authentication/fieldguide-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Audit
- Advisory
- Accounting
- Compliance
- Risk
- Engagement Management
- Artificial Intelligence
- Agents
- Webhooks
---
