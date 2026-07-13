---
api_key_in:
- header
api_specs:
- filename: travelcenters-of-america-openapi.yml
  format: yaml
  label: TravelCenters of America API
  slug: travelcenters-of-america
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelcenters-of-america/refs/heads/main/openapi/travelcenters-of-america-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Travelcenters Of America Authentication
name_suffix: Authentication
oauth_flows: []
overview: TravelCenters of America secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TravelCenters of America
provider_slug: travelcenters-of-america
scheme_count: 1
schemes:
- description: API access token obtained via developer.accessta.com
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/travelcenters-of-america-openapi.yml
  type: apiKey
slug: travelcenters-of-america-authentication
source_filename: travelcenters-of-america-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/travelcenters-of-america-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API access token obtained via developer.accessta.com\n  sources:\n  - openapi/travelcenters-of-america-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travelcenters-of-america/refs/heads/main/authentication/travelcenters-of-america-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Travel Centers
- Truck Service
- Retail
- Fuel
- Locations
- Trucking
- Fleet Management
- Fortune 500
---
