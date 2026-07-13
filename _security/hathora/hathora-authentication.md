---
api_key_in: []
api_specs:
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Auth API
  slug: hathora-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Apps API
  slug: hathora-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Builds API
  slug: hathora-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Deployments API
  slug: hathora-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Processes API
  slug: hathora-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Rooms API
  slug: hathora-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Discovery API
  slug: hathora-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Logs API
  slug: hathora-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Metrics API
  slug: hathora-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Billing API
  slug: hathora-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Tokens API
  slug: hathora-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hathora Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hathora secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hathora
provider_slug: hathora
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Organization developer/API token used for management endpoints (apps, builds, deployments, processes, rooms, logs, metrics, billing, tokens).
  name: hathoraDevToken
  scheme: bearer
  sources:
  - openapi/hathora-openapi.yml
  type: http
slug: hathora-authentication
source_filename: hathora-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hathora-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: hathoraDevToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Organization developer/API token used for management endpoints (apps, builds,\n    deployments, processes, rooms, logs, metrics, billing, tokens).\n  sources:\n  - openapi/hathora-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/authentication/hathora-authentication.yml
summary_line: http · 1 scheme
tags:
- Game Servers
- Multiplayer
- Compute
- Hosting
- Orchestration
---
