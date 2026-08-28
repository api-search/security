---
api_key_in:
- header
api_specs:
- filename: nexar-virtualcam-openapi.yml
  format: yaml
  label: CityStream VirtualCam API
  slug: virtualcam
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-virtualcam-openapi.yml
- filename: nexar-livefeed-openapi.yml
  format: yaml
  label: CityStream Live Feed API
  slug: livefeed
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-livefeed-openapi.yml
- filename: nexar-workzones-openapi.yml
  format: yaml
  label: CityStream Work Zones API
  slug: workzones
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-workzones-openapi.yml
- filename: nexar-roadinventory-openapi.yml
  format: yaml
  label: CityStream Road Inventory API
  slug: roadinventory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-roadinventory-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nexar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nexar secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nexar
provider_slug: nexar
scheme_count: 1
schemes:
- in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/nexar-livefeed-openapi.yml
  - openapi/nexar-roadinventory-openapi.yml
  - openapi/nexar-virtualcam-openapi.yml
  - openapi/nexar-workzones-openapi.yml
  type: apiKey
slug: nexar-authentication
source_filename: nexar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/nexar-livefeed-openapi.yml, openapi/nexar-roadinventory-openapi.yml, openapi/nexar-virtualcam-openapi.yml,\n  openapi/nexar-workzones-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/nexar-livefeed-openapi.yml\n  - openapi/nexar-roadinventory-openapi.yml\n  - openapi/nexar-virtualcam-openapi.yml\n  - openapi/nexar-workzones-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/authentication/nexar-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Mapping
- Geospatial
- Transportation
- Computer Vision
- Autonomous Vehicles
- Smart Cities
- Imagery
- Road Data
- Machine Learning
---
