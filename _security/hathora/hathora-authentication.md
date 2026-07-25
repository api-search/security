---
api_key_in: []
api_specs:
- filename: hathora-appsv2-api-openapi.yml
  format: yaml
  label: Hathora AppsV2 API
  slug: hathora-appsv2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-appsv2-api-openapi.yml
- filename: hathora-authv1-api-openapi.yml
  format: yaml
  label: Hathora AuthV1 API
  slug: hathora-authv1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-authv1-api-openapi.yml
- filename: hathora-billingv1-api-openapi.yml
  format: yaml
  label: Hathora BillingV1 API
  slug: hathora-billingv1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-billingv1-api-openapi.yml
- filename: hathora-buildsv3-api-openapi.yml
  format: yaml
  label: Hathora BuildsV3 API
  slug: hathora-buildsv3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-buildsv3-api-openapi.yml
- filename: hathora-deploymentsv3-api-openapi.yml
  format: yaml
  label: Hathora DeploymentsV3 API
  slug: hathora-deploymentsv3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-deploymentsv3-api-openapi.yml
- filename: hathora-discoveryv2-api-openapi.yml
  format: yaml
  label: Hathora DiscoveryV2 API
  slug: hathora-discoveryv2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-discoveryv2-api-openapi.yml
- filename: hathora-logsv1-api-openapi.yml
  format: yaml
  label: Hathora LogsV1 API
  slug: hathora-logsv1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-logsv1-api-openapi.yml
- filename: hathora-metricsv1-api-openapi.yml
  format: yaml
  label: Hathora MetricsV1 API
  slug: hathora-metricsv1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-metricsv1-api-openapi.yml
- filename: hathora-processesv3-api-openapi.yml
  format: yaml
  label: Hathora ProcessesV3 API
  slug: hathora-processesv3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-processesv3-api-openapi.yml
- filename: hathora-roomsv2-api-openapi.yml
  format: yaml
  label: Hathora RoomsV2 API
  slug: hathora-roomsv2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-roomsv2-api-openapi.yml
- filename: hathora-tokensv1-api-openapi.yml
  format: yaml
  label: Hathora TokensV1 API
  slug: hathora-tokensv1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-tokensv1-api-openapi.yml
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
