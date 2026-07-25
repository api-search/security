---
api_key_in: []
api_specs:
- filename: deepnote-execute-v1-api-openapi.yml
  format: yaml
  label: Deepnote Execute (v1) API
  slug: deepnote-execute-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepnote/refs/heads/main/openapi/deepnote-execute-v1-api-openapi.yml
- filename: deepnote-me-api-openapi.yml
  format: yaml
  label: Deepnote Me API
  slug: deepnote-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepnote/refs/heads/main/openapi/deepnote-me-api-openapi.yml
- filename: deepnote-notebooks-api-openapi.yml
  format: yaml
  label: Deepnote Notebooks API
  slug: deepnote-notebooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepnote/refs/heads/main/openapi/deepnote-notebooks-api-openapi.yml
- filename: deepnote-projects-api-openapi.yml
  format: yaml
  label: Deepnote Projects API
  slug: deepnote-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepnote/refs/heads/main/openapi/deepnote-projects-api-openapi.yml
- filename: deepnote-runs-api-openapi.yml
  format: yaml
  label: Deepnote Runs API
  slug: deepnote-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepnote/refs/heads/main/openapi/deepnote-runs-api-openapi.yml
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
