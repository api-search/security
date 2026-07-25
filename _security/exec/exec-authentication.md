---
api_key_in: []
api_specs:
- filename: exec-collections-api-openapi.yml
  format: yaml
  label: Exec Collections API
  slug: exec-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/openapi/exec-collections-api-openapi.yml
- filename: exec-knowledge-hub-folders-api-openapi.yml
  format: yaml
  label: Exec Knowledge Hub - Folders API
  slug: exec-knowledge-hub-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/openapi/exec-knowledge-hub-folders-api-openapi.yml
- filename: exec-knowledge-hub-pages-api-openapi.yml
  format: yaml
  label: Exec Knowledge Hub - Pages API
  slug: exec-knowledge-hub-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/openapi/exec-knowledge-hub-pages-api-openapi.yml
- filename: exec-knowledge-hub-sources-api-openapi.yml
  format: yaml
  label: Exec Knowledge Hub - Sources API
  slug: exec-knowledge-hub-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/openapi/exec-knowledge-hub-sources-api-openapi.yml
- filename: exec-scenario-studio-api-openapi.yml
  format: yaml
  label: Exec Scenario Studio API
  slug: exec-scenario-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/openapi/exec-scenario-studio-api-openapi.yml
- filename: exec-scenarios-api-openapi.yml
  format: yaml
  label: Exec Scenarios API
  slug: exec-scenarios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/openapi/exec-scenarios-api-openapi.yml
- filename: exec-sessions-api-openapi.yml
  format: yaml
  label: Exec Sessions API
  slug: exec-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/openapi/exec-sessions-api-openapi.yml
- filename: exec-skills-api-openapi.yml
  format: yaml
  label: Exec Skills API
  slug: exec-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/openapi/exec-skills-api-openapi.yml
- filename: exec-workspace-api-openapi.yml
  format: yaml
  label: Exec Workspace API
  slug: exec-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/openapi/exec-workspace-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Exec Authentication
name_suffix: Authentication
oauth_flows: []
overview: Exec secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Exec
provider_slug: exec
scheme_count: 1
schemes:
- description: 'API key created in Settings > API. Passed as `Authorization: Bearer [example key]`.


    Format: `exec_live_` followed by 40 alphanumeric characters.

    Keys grant full admin access to the workspace (no scopes/permissions).

    Keys are shown only once at creation; deactivation is reversible, deletion is permanent.'
  docs: https://docs.exec.com/api-reference/authentication
  key_prefix: exec_live_
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/exec-openapi-original.yml
  test_prefix: null
  type: http
slug: exec-authentication
source_filename: exec-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/exec-openapi-original.yml\ndocs: https://docs.exec.com/api-reference/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\n  scopes: none\n  access: full-admin\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    API key created in Settings > API. Passed as `Authorization: Bearer [example key]`.\n\n    Format: `exec_live_` followed by 40 alphanumeric characters.\n    Keys grant full admin access to the workspace (no scopes/permissions).\n    Keys are shown only once at creation; deactivation is reversible, deletion is permanent.\n  key_prefix: exec_live_\n  test_prefix: null\n  sources:\n  - openapi/exec-openapi-original.yml\n  docs: https://docs.exec.com/api-reference/authentication\nnotes: >-\n  No test/sandbox key variant is documented (only exec_live_). No OAuth or scope\n  surface, so scopes/ is intentionally omitted for\
  \ this provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/authentication/exec-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Sales Enablement
- Training
- Roleplay
- Coaching
- Learning
- Knowledge Management
- LMS
---
