---
api_key_in: []
api_specs:
- filename: tally-forms-api-openapi.yml
  format: yaml
  label: Tally Forms API
  slug: tally-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tally/refs/heads/main/openapi/tally-forms-api-openapi.yml
- filename: tally-organization-api-openapi.yml
  format: yaml
  label: Tally Organization API
  slug: tally-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tally/refs/heads/main/openapi/tally-organization-api-openapi.yml
- filename: tally-submissions-api-openapi.yml
  format: yaml
  label: Tally Submissions API
  slug: tally-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tally/refs/heads/main/openapi/tally-submissions-api-openapi.yml
- filename: tally-users-api-openapi.yml
  format: yaml
  label: Tally Users API
  slug: tally-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tally/refs/heads/main/openapi/tally-users-api-openapi.yml
- filename: tally-webhooks-api-openapi.yml
  format: yaml
  label: Tally Webhooks API
  slug: tally-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tally/refs/heads/main/openapi/tally-webhooks-api-openapi.yml
- filename: tally-workspaces-api-openapi.yml
  format: yaml
  label: Tally Workspaces API
  slug: tally-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tally/refs/heads/main/openapi/tally-workspaces-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tally Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tally secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tally
provider_slug: tally
scheme_count: 1
schemes:
- description: 'Tally API key created in the workspace dashboard, sent as "Authorization: Bearer <token>".'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/tally-openapi.yml
  type: http
slug: tally-authentication
source_filename: tally-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tally-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Tally API key created in the workspace dashboard, sent as \"Authorization: Bearer\n    <token>\".'\n  sources:\n  - openapi/tally-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tally/refs/heads/main/authentication/tally-authentication.yml
summary_line: http · 1 scheme
tags:
- Forms
- Surveys
- No-Code
- Free
- Notion-style
- Webhooks
- MCP
---
