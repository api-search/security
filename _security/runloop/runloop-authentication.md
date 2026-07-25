---
api_key_in: []
api_specs:
- filename: runloop-account-api-openapi.yml
  format: yaml
  label: Runloop Account API
  slug: runloop-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop/refs/heads/main/openapi/runloop-account-api-openapi.yml
- filename: runloop-benchmark-api-openapi.yml
  format: yaml
  label: Runloop Benchmark API
  slug: runloop-benchmark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop/refs/heads/main/openapi/runloop-benchmark-api-openapi.yml
- filename: runloop-blueprint-api-openapi.yml
  format: yaml
  label: Runloop Blueprint API
  slug: runloop-blueprint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop/refs/heads/main/openapi/runloop-blueprint-api-openapi.yml
- filename: runloop-devbox-api-openapi.yml
  format: yaml
  label: Runloop Devbox API
  slug: runloop-devbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop/refs/heads/main/openapi/runloop-devbox-api-openapi.yml
- filename: runloop-object-api-openapi.yml
  format: yaml
  label: Runloop Object API
  slug: runloop-object-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop/refs/heads/main/openapi/runloop-object-api-openapi.yml
- filename: runloop-scenario-api-openapi.yml
  format: yaml
  label: Runloop Scenario API
  slug: runloop-scenario-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop/refs/heads/main/openapi/runloop-scenario-api-openapi.yml
- filename: runloop-snapshot-api-openapi.yml
  format: yaml
  label: Runloop Snapshot API
  slug: runloop-snapshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop/refs/heads/main/openapi/runloop-snapshot-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Runloop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Runloop secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Runloop
provider_slug: runloop
scheme_count: 1
schemes:
- description: 'Runloop API key sent as: Authorization Bearer <API_KEY>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/runloop-openapi.yml
  type: http
slug: runloop-authentication
source_filename: runloop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/runloop-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Runloop API key sent as: Authorization Bearer <API_KEY>.'\n  sources:\n  - openapi/runloop-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runloop/refs/heads/main/authentication/runloop-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Developer Environments
- Devboxes
- Coding Agents
- Benchmarking
- Cloud IDE
---
