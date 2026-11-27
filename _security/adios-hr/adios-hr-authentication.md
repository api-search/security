---
anonymous_access: false
api_key_in: []
api_specs:
- filename: adios-hr-radar-api-api-openapi.yml
  format: yaml
  label: adios-hr Radar API
  slug: adios-hr-radar-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adios-hr/openapi/adios-hr-radar-api-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: adios-hr Authentication
name_suffix: Authentication
oauth_flows: []
overview: adios-hr declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: adios-hr
provider_slug: adios-hr
scheme_count: 2
schemes:
- description: 'Authorization: Bearer adios_radar_… (a Radar key: /api/v1/radar only)'
  scheme: bearer
  type: http
- description: 'A Radar key (adios_radar_…): /api/v1/radar only'
  in: header
  name: X-Api-Key
  type: apiKey
slug: adios-hr-authentication
source_filename: adios-hr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://adios.hr/developers/radar/docs\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"Authorization: Bearer adios_radar_… (a Radar key: /api/v1/radar only)\"\n  - type: apiKey\n    in: header\n    name: X-Api-Key\n    description: \"A Radar key (adios_radar_…): /api/v1/radar only\"\n"
source_yaml_url: https://artifacts.apis.io/adios-hr/authentication/adios-hr-authentication.yml
summary_line: 2 schemes
tags:
- Company
---
