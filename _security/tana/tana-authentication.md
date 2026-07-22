---
api_key_in: []
api_specs:
- filename: tana-input-api-openapi.yml
  format: yaml
  label: Tana Input API
  slug: tana-input-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tana/refs/heads/main/openapi/tana-input-api-openapi.yml
- filename: tana-docs-api-openapi.yml
  format: yaml
  label: Tana Documentation API
  slug: tana-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tana/refs/heads/main/openapi/tana-docs-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tana Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tana secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tana
provider_slug: tana
scheme_count: 1
schemes:
- description: 'Workspace-scoped API token, generated in the Tana client under API Tokens. Sent as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tana-input-api-openapi.yml
  type: http
slug: tana-authentication
source_filename: tana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/tana-input-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Workspace-scoped API token, generated in the Tana client under API Tokens. Sent\n    as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/tana-input-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tana/refs/heads/main/authentication/tana-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Note Taking
- Knowledge Management
- Productivity
- Artificial Intelligence
- Meetings
- Agents
- Collaboration
- Outliner
---
