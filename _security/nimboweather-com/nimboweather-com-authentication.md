---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: nimboweather-com-frames-api-openapi.yml
  format: yaml
  label: Nimbo Weather Frames API
  slug: nimboweather-com-frames-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nimboweather-com/openapi/nimboweather-com-frames-api-openapi.yml
- filename: nimboweather-com-keys-api-openapi.yml
  format: yaml
  label: Nimbo Weather Keys API
  slug: nimboweather-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nimboweather-com/openapi/nimboweather-com-keys-api-openapi.yml
- filename: nimboweather-com-nowcast-api-openapi.yml
  format: yaml
  label: Nimbo Weather Nowcast API
  slug: nimboweather-com-nowcast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nimboweather-com/openapi/nimboweather-com-nowcast-api-openapi.yml
- filename: nimboweather-com-status-api-openapi.yml
  format: yaml
  label: Nimbo Weather Status API
  slug: nimboweather-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nimboweather-com/openapi/nimboweather-com-status-api-openapi.yml
- filename: nimboweather-com-tiles-api-openapi.yml
  format: yaml
  label: Nimbo Weather Tiles API
  slug: nimboweather-com-tiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nimboweather-com/openapi/nimboweather-com-tiles-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Nimbo Weather Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nimbo Weather secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nimbo Weather
provider_slug: nimboweather-com
scheme_count: 3
schemes:
- description: Your key (nimbo_...), recommended.
  in: header
  name: X-API-Key
  parameter: X-API-Key
  sources:
  - openapi/nimboweather-com-openapi.json
  type: apiKey
- description: Your key as ?key= (the only way tiles take it).
  in: query
  name: key
  parameter: key
  sources:
  - openapi/nimboweather-com-openapi.json
  type: apiKey
- description: 'Authorization: Bearer nimbo_...'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/nimboweather-com-openapi.json
  type: http
slug: nimboweather-com-authentication
source_filename: nimboweather-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/nimboweather-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Your key (nimbo_...), recommended.\n  sources:\n  - openapi/nimboweather-com-openapi.json\n- name: key\n  type: apiKey\n  in: query\n  parameter: key\n  description: Your key as ?key= (the only way tiles take it).\n  sources:\n  - openapi/nimboweather-com-openapi.json\n- name: Bearer\n  type: http\n  scheme: bearer\n  description: 'Authorization: Bearer nimbo_...'\n  sources:\n  - openapi/nimboweather-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/nimboweather-com/authentication/nimboweather-com-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Weather
- Rain
- Europe
- Forecast
---
