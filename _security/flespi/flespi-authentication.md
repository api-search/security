---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: flespi-assets-api-openapi.yml
  format: yaml
  label: flespi Assets API
  slug: flespi-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flespi/openapi/flespi-assets-api-openapi.yml
- filename: flespi-calculators-api-openapi.yml
  format: yaml
  label: flespi Calculators API
  slug: flespi-calculators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flespi/openapi/flespi-calculators-api-openapi.yml
- filename: flespi-changelog-api-openapi.yml
  format: yaml
  label: flespi Changelog API
  slug: flespi-changelog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flespi/openapi/flespi-changelog-api-openapi.yml
- filename: flespi-channels-api-openapi.yml
  format: yaml
  label: flespi Channels API
  slug: flespi-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flespi/openapi/flespi-channels-api-openapi.yml
- filename: flespi-devices-api-openapi.yml
  format: yaml
  label: flespi Devices API
  slug: flespi-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flespi/openapi/flespi-devices-api-openapi.yml
- filename: flespi-geofences-api-openapi.yml
  format: yaml
  label: flespi Geofences API
  slug: flespi-geofences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flespi/openapi/flespi-geofences-api-openapi.yml
- filename: flespi-groups-api-openapi.yml
  format: yaml
  label: flespi Groups API
  slug: flespi-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flespi/openapi/flespi-groups-api-openapi.yml
- filename: flespi-modems-api-openapi.yml
  format: yaml
  label: flespi Modems API
  slug: flespi-modems-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flespi/openapi/flespi-modems-api-openapi.yml
- filename: flespi-plugins-api-openapi.yml
  format: yaml
  label: flespi Plugins API
  slug: flespi-plugins-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flespi/openapi/flespi-plugins-api-openapi.yml
- filename: flespi-protocols-api-openapi.yml
  format: yaml
  label: flespi Protocols API
  slug: flespi-protocols-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flespi/openapi/flespi-protocols-api-openapi.yml
- filename: flespi-streams-api-openapi.yml
  format: yaml
  label: flespi Streams API
  slug: flespi-streams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flespi/openapi/flespi-streams-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: flespi Authentication
name_suffix: Authentication
oauth_flows: []
overview: flespi secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: flespi
provider_slug: flespi
scheme_count: 1
schemes:
- description: Authorization through FlespiToken
  in: header
  name: FlespiToken
  parameter: Authorization
  sources:
  - openapi/gw-openapi.json
  type: apiKey
slug: flespi-authentication
source_filename: flespi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/gw-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: FlespiToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Authorization through FlespiToken\n  sources:\n  - openapi/gw-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/flespi/authentication/flespi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Telematics
- IoT
- Data Ingestion
- Real-Time Analytics
---
