---
api_key_in:
- header
- query
api_specs:
- filename: workwave-openapi.yml
  format: yaml
  label: WorkWave Route Manager - Orders, Routes & Territories
  slug: route-manager-orders-routes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-openapi.yml
- filename: workwave-openapi.yml
  format: yaml
  label: WorkWave Route Manager - Drivers & Vehicles
  slug: route-manager-drivers-vehicles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-openapi.yml
- filename: workwave-openapi.yml
  format: yaml
  label: WorkWave Route Manager - GPS Tracking
  slug: route-manager-gps-tracking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-openapi.yml
- filename: workwave-openapi.yml
  format: yaml
  label: WorkWave Route Manager - Webhooks
  slug: route-manager-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Workwave Authentication
name_suffix: Authentication
oauth_flows: []
overview: WorkWave secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: WorkWave
provider_slug: workwave
scheme_count: 2
schemes:
- description: API key (UUID) supplied via the X-WorkWave-Key HTTP header.
  in: header
  name: ApiKeyHeader
  parameter: X-WorkWave-Key
  sources:
  - openapi/workwave-openapi.yml
  type: apiKey
- description: API key (UUID) supplied via the `key` query-string parameter. Takes precedence over the header if both are present.
  in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/workwave-openapi.yml
  type: apiKey
slug: workwave-authentication
source_filename: workwave-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workwave-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-WorkWave-Key\n  description: API key (UUID) supplied via the X-WorkWave-Key HTTP header.\n  sources:\n  - openapi/workwave-openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key (UUID) supplied via the `key` query-string parameter. Takes precedence\n    over the header if both are present.\n  sources:\n  - openapi/workwave-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/authentication/workwave-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Field Service
- Route Optimization
- Last Mile Delivery
- Fleet
- GPS Tracking
- Logistics
---
