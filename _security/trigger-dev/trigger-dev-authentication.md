---
api_key_in: []
api_specs:
- filename: trigger-dev-management-openapi.yml
  format: yaml
  label: Trigger.dev Management API
  slug: trigger-dev-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trigger-dev/refs/heads/main/openapi/trigger-dev-management-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Trigger Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trigger.dev secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Trigger.dev
provider_slug: trigger-dev
scheme_count: 1
schemes:
- description: Secret API key (starts with tr_dev_, tr_prod_, or tr_stg_). Set TRIGGER_SECRET_KEY environment variable or pass in Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/trigger-dev-management-openapi.yml
  type: http
slug: trigger-dev-authentication
source_filename: trigger-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trigger-dev-management-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Secret API key (starts with tr_dev_, tr_prod_, or tr_stg_). Set TRIGGER_SECRET_KEY\n    environment variable or pass in Authorization header.\n  sources:\n  - openapi/trigger-dev-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trigger-dev/refs/heads/main/authentication/trigger-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Developer-First
- Workflow Automation
- Background Jobs
- Durable Execution
- TypeScript
- AI Agents
- Realtime
- Open Source
---
