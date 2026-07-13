---
api_key_in: []
api_specs:
- filename: reclaim-api-0.1.yml
  format: yaml
  label: Reclaim API
  slug: reclaim-api
  spec_type: OpenAPI
  url: https://api.app.reclaim.ai/swagger/reclaim-api-0.1.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Reclaim Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reclaim.ai secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reclaim.ai
provider_slug: reclaim-ai
scheme_count: 1
schemes:
- flows: []
  name: Authorization
  sources:
  - openapi/reclaim-ai-openapi.yml
  type: oauth2
slug: reclaim-ai-authentication
source_filename: reclaim-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reclaim-ai-openapi.yml\nsummary:\n  types:\n  - oauth2\nschemes:\n- name: Authorization\n  type: oauth2\n  flows: []\n  sources:\n  - openapi/reclaim-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reclaim-ai/refs/heads/main/authentication/reclaim-ai-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- AI
- Scheduling
- Calendar
- Productivity
- Tasks
- Habits
- Time Management
- Meetings
- Focus Time
---
