---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: flightqueue-com-airports-api-openapi.yml
  format: yaml
  label: FlightQueue Airports API
  slug: flightqueue-com-airports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightqueue-com/openapi/flightqueue-com-airports-api-openapi.yml
- filename: flightqueue-com-alerts-api-openapi.yml
  format: yaml
  label: FlightQueue Alerts API
  slug: flightqueue-com-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightqueue-com/openapi/flightqueue-com-alerts-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: FlightQueue Authentication
name_suffix: Authentication
oauth_flows: []
overview: FlightQueue secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FlightQueue
provider_slug: flightqueue-com
scheme_count: 2
schemes:
- description: Agent key (`fqagent_…`) from POST /api/agent/register, or developer key (`fq_live_…`) from https://flightqueue.com/pricing
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/flightqueue-com-openapi.json
  type: http
- description: Same keys as Bearer auth, sent via X-API-Key header
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/flightqueue-com-openapi.json
  type: apiKey
slug: flightqueue-com-authentication
source_filename: flightqueue-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/flightqueue-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Agent key (`fqagent_…`) from POST /api/agent/register, or developer key (`fq_live_…`)\n    from https://flightqueue.com/pricing\n  sources:\n  - openapi/flightqueue-com-openapi.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Same keys as Bearer auth, sent via X-API-Key header\n  sources:\n  - openapi/flightqueue-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/flightqueue-com/authentication/flightqueue-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Airport
- Real-Time Data
- Travel
- Aviation
---
