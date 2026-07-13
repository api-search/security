---
api_key_in: []
api_specs:
- filename: runloop-openapi.yml
  format: yaml
  label: Runloop Devboxes API
  slug: runloop-devboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop/refs/heads/main/openapi/runloop-openapi.yml
- filename: runloop-openapi.yml
  format: yaml
  label: Runloop Blueprints API
  slug: runloop-blueprints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop/refs/heads/main/openapi/runloop-openapi.yml
- filename: runloop-openapi.yml
  format: yaml
  label: Runloop Snapshots API
  slug: runloop-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop/refs/heads/main/openapi/runloop-openapi.yml
- filename: runloop-openapi.yml
  format: yaml
  label: Runloop Code Mounts API
  slug: runloop-code-mounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop/refs/heads/main/openapi/runloop-openapi.yml
- filename: runloop-openapi.yml
  format: yaml
  label: Runloop Repositories API
  slug: runloop-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop/refs/heads/main/openapi/runloop-openapi.yml
- filename: runloop-openapi.yml
  format: yaml
  label: Runloop Scenarios API
  slug: runloop-scenarios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop/refs/heads/main/openapi/runloop-openapi.yml
- filename: runloop-openapi.yml
  format: yaml
  label: Runloop Benchmarks API
  slug: runloop-benchmarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop/refs/heads/main/openapi/runloop-openapi.yml
- filename: runloop-openapi.yml
  format: yaml
  label: Runloop Objects API
  slug: runloop-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop/refs/heads/main/openapi/runloop-openapi.yml
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
