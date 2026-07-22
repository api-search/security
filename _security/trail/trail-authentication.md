---
api_key_in:
- header
api_specs:
- filename: trail_task_reports_v1.yaml
  format: yaml
  label: Trail Task Reports API
  slug: trail-task-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_task_reports_v1.yaml
- filename: trail_task_instances_v1.yaml
  format: yaml
  label: Trail Task Instances API
  slug: trail-task-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_task_instances_v1.yaml
- filename: trail_task_templates_v1.yaml
  format: yaml
  label: Trail Task Templates API
  slug: trail-task-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_task_templates_v1.yaml
- filename: trail_sites_v1.yaml
  format: yaml
  label: Trail Sites API
  slug: trail-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_sites_v1.yaml
- filename: trail_areas_v1.yaml
  format: yaml
  label: Trail Areas API
  slug: trail-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_areas_v1.yaml
- filename: trail_tags_v1.yaml
  format: yaml
  label: Trail Tags API
  slug: trail-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_tags_v1.yaml
- filename: trail_scores_v1.yaml
  format: yaml
  label: Trail Scores API
  slug: trail-scores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_scores_v1.yaml
- filename: trail_evo_api_v1.yaml
  format: yaml
  label: Trail Evo API
  slug: trail-evo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/openapi/trail_evo_api_v1.yaml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Trail Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Trail secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Trail
provider_slug: trail
scheme_count: 2
schemes:
- in: header
  name: API_KEY
  parameter: API_KEY
  sources:
  - openapi/trail_areas_v1.yaml
  - openapi/trail_scores_v1.yaml
  - openapi/trail_sites_v1.yaml
  - openapi/trail_tags_v1.yaml
  - openapi/trail_task_instances_v1.yaml
  - openapi/trail_task_reports_v1.yaml
  - openapi/trail_task_templates_v1.yaml
  type: apiKey
- flows:
  - authorizationUrl: https://preprodidentity.accessacloud.com/connect/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: /api/evo_api/oauth/token
  name: oauth2
  sources:
  - openapi/trail_evo_api_v1.yaml
  type: oauth2
slug: trail-authentication
source_filename: trail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/trail_areas_v1.yaml, openapi/trail_evo_api_v1.yaml, openapi/trail_scores_v1.yaml,\n  openapi/trail_sites_v1.yaml, openapi/trail_tags_v1.yaml, openapi/trail_task_instances_v1.yaml,\n  openapi/trail_task_reports_v1.yaml, openapi/trail_task_templates_v1.yaml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: API_KEY\n  type: apiKey\n  in: header\n  parameter: API_KEY\n  sources:\n  - openapi/trail_areas_v1.yaml\n  - openapi/trail_scores_v1.yaml\n  - openapi/trail_sites_v1.yaml\n  - openapi/trail_tags_v1.yaml\n  - openapi/trail_task_instances_v1.yaml\n  - openapi/trail_task_reports_v1.yaml\n  - openapi/trail_task_templates_v1.yaml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://preprodidentity.accessacloud.com/connect/authorize\n    tokenUrl: /api/evo_api/oauth/token\n    scopes: 4\n  sources:\n\
  \  - openapi/trail_evo_api_v1.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trail/refs/heads/main/authentication/trail-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Hospitality
- Checklists
- Task Management
- Compliance
- Food Safety
- Operations
---
