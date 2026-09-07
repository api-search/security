---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: RoxyAPI REST API v2
  slug: roxyapi-rest-api-v2
  spec_type: OpenAPI
  url: https://roxyapi.com/api/v2/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Roxyapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: RoxyAPI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RoxyAPI
provider_slug: roxyapi
scheme_count: 1
schemes:
- description: Your API key for accessing RoxyAPI. Alternatively, you can pass the API key as a query parameter "api_key".
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/roxyapi-openapi-original.json
  type: apiKey
slug: roxyapi-authentication
source_filename: roxyapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: derived\nsource: openapi/roxyapi-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Your API key for accessing RoxyAPI. Alternatively, you can pass the API key as\n    a query parameter \"api_key\".\n  sources:\n  - openapi/roxyapi-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roxyapi/refs/heads/main/authentication/roxyapi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Astrology
- Vedic Astrology
- numerology
- tarot
- human-design
- Forecast
- biorhythm
- iching
- crystals
- Dreams
- angel-numbers
- Location
- spiritual
- Wellness
- MCP Server
- OpenAPI
- llms-txt
- agent-native
---
