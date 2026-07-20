---
api_key_in:
- header
api_specs:
- filename: groundwork-open-source-tcg-openapi-original.yml
  format: yaml
  label: GroundWork TCG Controller API
  slug: groundwork-tcg-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groundwork-open-source/refs/heads/main/openapi/groundwork-open-source-tcg-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Groundwork Open Source Authentication
name_suffix: Authentication
oauth_flows: []
overview: Groundwork Open Source secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Groundwork Open Source
provider_slug: groundwork-open-source
scheme_count: 2
schemes:
- description: Application name registered with the GroundWork Monitor / Foundation server (e.g. the connector's appName). Sent on every protected request.
  in: header
  name: GWOS-APP-NAME
  parameter: GWOS-APP-NAME
  required: true
  sources:
  - openapi/groundwork-open-source-tcg-openapi-original.yml
  type: apiKey
- description: API token issued by the GroundWork Foundation server, obtained by the agent/connector at startup. Presented alongside GWOS-APP-NAME to authorize config, inventory, metrics, events and downtime operations.
  in: header
  name: GWOS-API-TOKEN
  parameter: GWOS-API-TOKEN
  required: true
  sources:
  - openapi/groundwork-open-source-tcg-openapi-original.yml
  type: apiKey
slug: groundwork-open-source-authentication
source_filename: groundwork-open-source-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/groundwork-open-source-tcg-openapi-original.yml\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    The TCG Controller REST API authenticates every protected operation with a\n    pair of required request headers rather than a declared OpenAPI\n    securityScheme. The Swagger 2.0 document models them as required header\n    parameters (GWOS-APP-NAME + GWOS-API-TOKEN); the effective auth model is an\n    apiKey-in-header scheme.\nschemes:\n  - name: GWOS-APP-NAME\n    type: apiKey\n    in: header\n    parameter: GWOS-APP-NAME\n    description: >-\n      Application name registered with the GroundWork Monitor / Foundation\n      server (e.g. the connector's appName). Sent on every protected request.\n    required: true\n    sources: [openapi/groundwork-open-source-tcg-openapi-original.yml]\n  - name: GWOS-API-TOKEN\n    type: apiKey\n    in: header\n    parameter: GWOS-API-TOKEN\n\
  \    description: >-\n      API token issued by the GroundWork Foundation server, obtained by the\n      agent/connector at startup. Presented alongside GWOS-APP-NAME to authorize\n      config, inventory, metrics, events and downtime operations.\n    required: true\n    sources: [openapi/groundwork-open-source-tcg-openapi-original.yml]\nunauthenticated_operations:\n  - path: /identity\n    method: GET\n    note: /identity returns only a 200 (no 401) in the spec.\nnotes: >-\n  Absent a live public host (GroundWork Monitor is self-hosted per customer) the\n  auth model is derived from the published Swagger 2.0 spec and the TCG SDK\n  README, not from a hosted docs auth page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groundwork-open-source/refs/heads/main/authentication/groundwork-open-source-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Monitoring
- Network Monitoring
- IT Infrastructure
- Observability
- Metrics
- Events
- Open Source
- Nagios
---
