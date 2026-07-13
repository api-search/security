---
api_key_in: []
api_specs:
- filename: deepnote-openapi.yml
  format: yaml
  label: Deepnote Execution API (Notebooks/Projects)
  slug: execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepnote/refs/heads/main/openapi/deepnote-openapi.yml
- filename: deepnote-openapi.yml
  format: yaml
  label: Deepnote Projects API
  slug: projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepnote/refs/heads/main/openapi/deepnote-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Deepnote Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deepnote secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Deepnote
provider_slug: deepnote
scheme_count: 1
schemes:
- description: 'Workspace API key created under Settings & members > Security > API keys, sent as Authorization: Bearer <token>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/deepnote-openapi.yml
  type: http
slug: deepnote-authentication
source_filename: deepnote-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/deepnote-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Workspace API key created under Settings & members > Security > API keys, sent\n    as Authorization: Bearer <token>.'\n  sources:\n  - openapi/deepnote-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepnote/refs/heads/main/authentication/deepnote-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Science
- Notebooks
- Analytics
- Collaboration
- Data Apps
---
