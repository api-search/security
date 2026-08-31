---
api_key_in:
- header
api_specs:
- filename: nexar-citystream-live-feed-api-v4-api-openapi.yml
  format: yaml
  label: Nexar CityStream™ Live Feed API V4 API
  slug: nexar-citystream-live-feed-api-v4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-citystream-live-feed-api-v4-api-openapi.yml
- filename: nexar-get-a-collection-of-road-signs-api-openapi.yml
  format: yaml
  label: Nexar Get a collection of road signs API
  slug: nexar-get-a-collection-of-road-signs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-get-a-collection-of-road-signs-api-openapi.yml
- filename: nexar-get-a-collection-of-work-zones-api-openapi.yml
  format: yaml
  label: Nexar Get a collection of work zones API
  slug: nexar-get-a-collection-of-work-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-get-a-collection-of-work-zones-api-openapi.yml
- filename: nexar-get-a-specific-work-zone-api-openapi.yml
  format: yaml
  label: Nexar Get a specific work zone API
  slug: nexar-get-a-specific-work-zone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-get-a-specific-work-zone-api-openapi.yml
- filename: nexar-get-the-details-of-a-specific-road-sign-api-openapi.yml
  format: yaml
  label: Nexar Get the details of a specific road sign API
  slug: nexar-get-the-details-of-a-specific-road-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-get-the-details-of-a-specific-road-sign-api-openapi.yml
- filename: nexar-virtualcam-api-api-openapi.yml
  format: yaml
  label: Nexar VirtualCam API
  slug: nexar-virtualcam-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-virtualcam-api-api-openapi.yml
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
