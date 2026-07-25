---
api_key_in:
- query
api_specs:
- filename: aviation-edge-real-time-api-openapi.yml
  format: yaml
  label: Aviation Edge Real-Time API
  slug: aviation-edge-real-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aviation-edge/refs/heads/main/openapi/aviation-edge-real-time-api-openapi.yml
- filename: aviation-edge-reference-api-openapi.yml
  format: yaml
  label: Aviation Edge Reference API
  slug: aviation-edge-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aviation-edge/refs/heads/main/openapi/aviation-edge-reference-api-openapi.yml
- filename: aviation-edge-satellites-api-openapi.yml
  format: yaml
  label: Aviation Edge Satellites API
  slug: aviation-edge-satellites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aviation-edge/refs/heads/main/openapi/aviation-edge-satellites-api-openapi.yml
- filename: aviation-edge-schedules-api-openapi.yml
  format: yaml
  label: Aviation Edge Schedules API
  slug: aviation-edge-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aviation-edge/refs/heads/main/openapi/aviation-edge-schedules-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aviation Edge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aviation Edge secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aviation Edge
provider_slug: aviation-edge
scheme_count: 1
schemes:
- in: query
  name: ApiKeyAuth
  parameter: key
  sources:
  - openapi/aviation-edge-openapi.yml
  type: apiKey
slug: aviation-edge-authentication
source_filename: aviation-edge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aviation-edge-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/aviation-edge-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aviation-edge/refs/heads/main/authentication/aviation-edge-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Airlines
- Airports
- Aviation
- Flight Data
- Real-Time
---
