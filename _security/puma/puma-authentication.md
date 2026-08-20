---
api_key_in:
- query
api_specs:
- filename: puma-gc-api-openapi.yml
  format: yaml
  label: Puma Gc API
  slug: puma-gc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/openapi/puma-gc-api-openapi.yml
- filename: puma-gc-stats-api-openapi.yml
  format: yaml
  label: Puma Gc Stats API
  slug: puma-gc-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/openapi/puma-gc-stats-api-openapi.yml
- filename: puma-halt-api-openapi.yml
  format: yaml
  label: Puma Halt API
  slug: puma-halt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/openapi/puma-halt-api-openapi.yml
- filename: puma-phased-restart-api-openapi.yml
  format: yaml
  label: Puma Phased Restart API
  slug: puma-phased-restart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/openapi/puma-phased-restart-api-openapi.yml
- filename: puma-refork-api-openapi.yml
  format: yaml
  label: Puma Refork API
  slug: puma-refork-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/openapi/puma-refork-api-openapi.yml
- filename: puma-reload-worker-directory-api-openapi.yml
  format: yaml
  label: Puma Reload Worker Directory API
  slug: puma-reload-worker-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/openapi/puma-reload-worker-directory-api-openapi.yml
- filename: puma-restart-api-openapi.yml
  format: yaml
  label: Puma Restart API
  slug: puma-restart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/openapi/puma-restart-api-openapi.yml
- filename: puma-stats-api-openapi.yml
  format: yaml
  label: Puma Stats API
  slug: puma-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/openapi/puma-stats-api-openapi.yml
- filename: puma-stop-api-openapi.yml
  format: yaml
  label: Puma Stop API
  slug: puma-stop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/openapi/puma-stop-api-openapi.yml
- filename: puma-thread-backtraces-api-openapi.yml
  format: yaml
  label: Puma Thread Backtraces API
  slug: puma-thread-backtraces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/openapi/puma-thread-backtraces-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Puma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Puma secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Puma
provider_slug: puma
scheme_count: 1
schemes:
- description: Shared control-app authentication token. Configured via Puma's `--control-token` option (or `auth_token` in the control app configuration). Required on every request; missing or wrong token returns 403.
  in: query
  name: controlToken
  parameter: token
  sources:
  - openapi/puma-openapi.yml
  type: apiKey
slug: puma-authentication
source_filename: puma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/puma-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: controlToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: Shared control-app authentication token. Configured via Puma's `--control-token`\n    option (or `auth_token` in the control app configuration). Required on every request; missing\n    or wrong token returns 403.\n  sources:\n  - openapi/puma-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/authentication/puma-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web Server
- Ruby
- Rack
- Application Server
- HTTP
- Open-Source
---
