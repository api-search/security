---
api_key_in: []
api_specs:
- filename: notion-openapi.yml
  format: yaml
  label: Notion API
  slug: notion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notion/refs/heads/main/openapi/notion-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Notion Authentication
name_suffix: Authentication
oauth_flows: []
overview: Notion secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Notion
provider_slug: notion
scheme_count: 1
schemes:
- description: Notion API uses bearer token authentication. Obtain an integration token from https://www.notion.so/my-integrations. Pass the token in the Authorization header as "Bearer {token}".
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/notion-openapi.yml
  type: http
slug: notion-authentication
source_filename: notion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/notion-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Notion API uses bearer token authentication. Obtain an integration token from\n    https://www.notion.so/my-integrations. Pass the token in the Authorization header as \"Bearer\n    {token}\".\n  sources:\n  - openapi/notion-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notion/refs/heads/main/authentication/notion-authentication.yml
summary_line: http · 1 scheme
tags:
- Collaboration
- Database
- Ideas
- Notes
- Productivity
- Projects
- T1
- Tasks
- Wiki
- Workspace
---
