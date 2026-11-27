---
anonymous_access: false
api_key_in: []
api_specs:
- filename: loopgantt-com-gantt-api-openapi.yml
  format: yaml
  label: LoopGantt Gantt API
  slug: loopgantt-com-gantt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loopgantt-com/openapi/loopgantt-com-gantt-api-openapi.yml
- filename: loopgantt-com-links-api-openapi.yml
  format: yaml
  label: LoopGantt Links API
  slug: loopgantt-com-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loopgantt-com/openapi/loopgantt-com-links-api-openapi.yml
- filename: loopgantt-com-me-api-openapi.yml
  format: yaml
  label: LoopGantt Me API
  slug: loopgantt-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loopgantt-com/openapi/loopgantt-com-me-api-openapi.yml
- filename: loopgantt-com-meetings-api-openapi.yml
  format: yaml
  label: LoopGantt Meetings API
  slug: loopgantt-com-meetings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loopgantt-com/openapi/loopgantt-com-meetings-api-openapi.yml
- filename: loopgantt-com-projects-api-openapi.yml
  format: yaml
  label: LoopGantt Projects API
  slug: loopgantt-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loopgantt-com/openapi/loopgantt-com-projects-api-openapi.yml
- filename: loopgantt-com-schedule-api-openapi.yml
  format: yaml
  label: LoopGantt Schedule API
  slug: loopgantt-com-schedule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loopgantt-com/openapi/loopgantt-com-schedule-api-openapi.yml
- filename: loopgantt-com-tasks-api-openapi.yml
  format: yaml
  label: LoopGantt Tasks API
  slug: loopgantt-com-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loopgantt-com/openapi/loopgantt-com-tasks-api-openapi.yml
- filename: loopgantt-com-templates-api-openapi.yml
  format: yaml
  label: LoopGantt Templates API
  slug: loopgantt-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loopgantt-com/openapi/loopgantt-com-templates-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: LoopGantt Authentication
name_suffix: Authentication
oauth_flows: []
overview: LoopGantt secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LoopGantt
provider_slug: loopgantt-com
scheme_count: 1
schemes:
- description: 'API key from https://loopgantt.com/settings/api-keys, sent as `Authorization: Bearer sk_live_…`. Keys carry scopes (projects:read, projects:write, tasks:read, tasks:write) and are limited to 120 requests per minute per key (429 RATE_LIMITED with Retry-After).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/loopgantt-com-openapi.json
  type: http
slug: loopgantt-com-authentication
source_filename: loopgantt-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/loopgantt-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key from https://loopgantt.com/settings/api-keys, sent as `Authorization:\n    Bearer sk_live_…`. Keys carry scopes (projects:read, projects:write, tasks:read, tasks:write)\n    and are limited to 120 requests per minute per key (429 RATE_LIMITED with Retry-After).'\n  sources:\n  - openapi/loopgantt-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/loopgantt-com/authentication/loopgantt-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Project Management
- Artificial Intelligence
- Gantt Chart
- Scheduling
- Software-as-a-Service
---
