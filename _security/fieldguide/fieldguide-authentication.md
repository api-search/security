---
api_key_in: []
api_specs:
- filename: fieldguide-api-api-openapi.yml
  format: yaml
  label: Fieldguide api API
  slug: fieldguide-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-api-api-openapi.yml
- filename: fieldguide-comments-api-openapi.yml
  format: yaml
  label: Fieldguide comments API
  slug: fieldguide-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-comments-api-openapi.yml
- filename: fieldguide-companies-api-openapi.yml
  format: yaml
  label: Fieldguide companies API
  slug: fieldguide-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-companies-api-openapi.yml
- filename: fieldguide-controls-api-openapi.yml
  format: yaml
  label: Fieldguide controls API
  slug: fieldguide-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-controls-api-openapi.yml
- filename: fieldguide-engagements-api-openapi.yml
  format: yaml
  label: Fieldguide engagements API
  slug: fieldguide-engagements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-engagements-api-openapi.yml
- filename: fieldguide-files-api-openapi.yml
  format: yaml
  label: Fieldguide files API
  slug: fieldguide-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-files-api-openapi.yml
- filename: fieldguide-insights-api-openapi.yml
  format: yaml
  label: Fieldguide insights API
  slug: fieldguide-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-insights-api-openapi.yml
- filename: fieldguide-jobs-api-openapi.yml
  format: yaml
  label: Fieldguide jobs API
  slug: fieldguide-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-jobs-api-openapi.yml
- filename: fieldguide-milestones-api-openapi.yml
  format: yaml
  label: Fieldguide milestones API
  slug: fieldguide-milestones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-milestones-api-openapi.yml
- filename: fieldguide-requests-api-openapi.yml
  format: yaml
  label: Fieldguide requests API
  slug: fieldguide-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-requests-api-openapi.yml
- filename: fieldguide-sheet-columns-api-openapi.yml
  format: yaml
  label: Fieldguide sheet-columns API
  slug: fieldguide-sheet-columns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-sheet-columns-api-openapi.yml
- filename: fieldguide-sheet-rows-api-openapi.yml
  format: yaml
  label: Fieldguide sheet-rows API
  slug: fieldguide-sheet-rows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-sheet-rows-api-openapi.yml
- filename: fieldguide-sheets-api-openapi.yml
  format: yaml
  label: Fieldguide sheets API
  slug: fieldguide-sheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-sheets-api-openapi.yml
- filename: fieldguide-users-api-openapi.yml
  format: yaml
  label: Fieldguide users API
  slug: fieldguide-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-users-api-openapi.yml
- filename: fieldguide-webhooks-api-openapi.yml
  format: yaml
  label: Fieldguide webhooks API
  slug: fieldguide-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-webhooks-api-openapi.yml
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
- Webhook
---
