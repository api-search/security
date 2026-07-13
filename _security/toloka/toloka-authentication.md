---
api_key_in:
- header
api_specs:
- filename: toloka-openapi.yml
  format: yaml
  label: Toloka Projects API
  slug: projects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-openapi.yml
- filename: toloka-openapi.yml
  format: yaml
  label: Toloka Pools API
  slug: pools
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-openapi.yml
- filename: toloka-openapi.yml
  format: yaml
  label: Toloka Tasks & Task Suites API
  slug: tasks-task-suites
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-openapi.yml
- filename: toloka-openapi.yml
  format: yaml
  label: Toloka Assignments API
  slug: assignments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-openapi.yml
- filename: toloka-openapi.yml
  format: yaml
  label: Toloka Operations & Webhooks API
  slug: operations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Toloka Authentication
name_suffix: Authentication
oauth_flows: []
overview: Toloka secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Toloka
provider_slug: toloka
scheme_count: 1
schemes:
- description: 'Pass your Toloka OAuth token (or API key) in the Authorization header as `Authorization: OAuth <token>` (legacy) or `Authorization: ApiKey <key>`.'
  in: header
  name: OAuthToken
  parameter: Authorization
  sources:
  - openapi/toloka-openapi.yml
  type: apiKey
slug: toloka-authentication
source_filename: toloka-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/toloka-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: OAuthToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Pass your Toloka OAuth token (or API key) in the Authorization header as `Authorization:\n    OAuth <token>` (legacy) or `Authorization: ApiKey <key>`.'\n  sources:\n  - openapi/toloka-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/authentication/toloka-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Labeling
- Crowdsourcing
- Human-in-the-Loop
- Training Data
- AI
---
