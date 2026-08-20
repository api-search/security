---
api_key_in:
- header
api_specs:
- filename: toloka-assignments-api-openapi.yml
  format: yaml
  label: Toloka Assignments API
  slug: toloka-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-assignments-api-openapi.yml
- filename: toloka-attachments-api-openapi.yml
  format: yaml
  label: Toloka Attachments API
  slug: toloka-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-attachments-api-openapi.yml
- filename: toloka-operations-api-openapi.yml
  format: yaml
  label: Toloka Operations API
  slug: toloka-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-operations-api-openapi.yml
- filename: toloka-pools-api-openapi.yml
  format: yaml
  label: Toloka Pools API
  slug: toloka-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-pools-api-openapi.yml
- filename: toloka-projects-api-openapi.yml
  format: yaml
  label: Toloka Projects API
  slug: toloka-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-projects-api-openapi.yml
- filename: toloka-skills-api-openapi.yml
  format: yaml
  label: Toloka Skills API
  slug: toloka-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-skills-api-openapi.yml
- filename: toloka-task-suites-api-openapi.yml
  format: yaml
  label: Toloka Task Suites API
  slug: toloka-task-suites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-task-suites-api-openapi.yml
- filename: toloka-tasks-api-openapi.yml
  format: yaml
  label: Toloka Tasks API
  slug: toloka-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-tasks-api-openapi.yml
- filename: toloka-training-api-openapi.yml
  format: yaml
  label: Toloka Training API
  slug: toloka-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-training-api-openapi.yml
- filename: toloka-user-bonuses-api-openapi.yml
  format: yaml
  label: Toloka User Bonuses API
  slug: toloka-user-bonuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-user-bonuses-api-openapi.yml
- filename: toloka-user-restrictions-api-openapi.yml
  format: yaml
  label: Toloka User Restrictions API
  slug: toloka-user-restrictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-user-restrictions-api-openapi.yml
- filename: toloka-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: Toloka Webhook Subscriptions API
  slug: toloka-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-webhook-subscriptions-api-openapi.yml
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
- Artificial Intelligence
---
