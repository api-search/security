---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: flight-mcp-com-flights-api-openapi.yml
  format: yaml
  label: flight-mcp-com Flights API
  slug: flight-mcp-com-flights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flight-mcp-com/openapi/flight-mcp-com-flights-api-openapi.yml
- filename: flight-mcp-com-healthz-api-openapi.yml
  format: yaml
  label: flight-mcp-com Healthz API
  slug: flight-mcp-com-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flight-mcp-com/openapi/flight-mcp-com-healthz-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Flight Mcp Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: flight-mcp-com secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: flight-mcp-com
provider_slug: flight-mcp-com
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/flight-mcp-com-openapi.json
  - openapi/flight-mcp-com-openapi.yml
  type: http
- in: header
  name: apiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/flight-mcp-com-openapi.json
  - openapi/flight-mcp-com-openapi.yml
  type: apiKey
slug: flight-mcp-com-authentication
source_filename: flight-mcp-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/flight-mcp-com-openapi.json, openapi/flight-mcp-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/flight-mcp-com-openapi.json\n  - openapi/flight-mcp-com-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/flight-mcp-com-openapi.json\n  - openapi/flight-mcp-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/flight-mcp-com/authentication/flight-mcp-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Travel
- API
- Flight
- MCP
- Search
---
