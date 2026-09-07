---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Latchkey Jobs API
  slug: latchkey-jobs-api
  spec_type: OpenAPI
  url: https://latchkey.dev/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Latchkey Authentication
name_suffix: Authentication
oauth_flows: []
overview: Latchkey Jobs API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Latchkey Jobs API
provider_slug: latchkey
scheme_count: 1
schemes:
- description: 'A Latchkey API key, sent as `Authorization: Bearer lk_live_...`. Create one in the Latchkey dashboard. Scopes: `jobs:read` for getJob, getJobLogs and listJobs; `jobs:run` for createJob, submitJob and cancelJob.'
  name: latchkeyApiKey
  scheme: bearer
  sources:
  - openapi/latchkey-jobs-api-openapi.json
  type: http
slug: latchkey-authentication
source_filename: latchkey-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: derived\nsource: openapi/latchkey-jobs-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: latchkeyApiKey\n  type: http\n  scheme: bearer\n  description: 'A Latchkey API key, sent as `Authorization: Bearer lk_live_...`. Create one\n    in the Latchkey dashboard. Scopes: `jobs:read` for getJob, getJobLogs and listJobs; `jobs:run`\n    for createJob, submitJob and cancelJob.'\n  sources:\n  - openapi/latchkey-jobs-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/latchkey/refs/heads/main/authentication/latchkey-authentication.yml
summary_line: http · 1 scheme
tags:
- CI/CD
- DevOps
- GitHub Actions
- Ephemeral Compute
- Build & Test Infrastructure
- Agent-Native
- AI Coding Agents
---
