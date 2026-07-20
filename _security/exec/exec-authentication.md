---
api_key_in: []
api_specs:
- filename: exec-openapi-original.yml
  format: yaml
  label: Exec API
  slug: exec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/openapi/exec-openapi-original.yml
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
