---
api_key_in: []
api_specs:
- filename: smartcar-vehicles-openapi.yml
  format: yaml
  label: Smartcar Vehicles API
  slug: vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartcar/refs/heads/main/openapi/smartcar-vehicles-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Smartcar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Smartcar secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Smartcar
provider_slug: smartcar
scheme_count: 1
schemes:
- description: OAuth 2.0 access token obtained via Authorization Code or Client Credentials flow
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/smartcar-vehicles-openapi.yml
  type: http
slug: smartcar-authentication
source_filename: smartcar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smartcar-vehicles-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token obtained via Authorization Code or Client Credentials\n    flow\n  sources:\n  - openapi/smartcar-vehicles-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartcar/refs/heads/main/authentication/smartcar-authentication.yml
summary_line: http · 1 scheme
tags:
- Automotive
- Connected Vehicles
- IoT
- Mobility
- Fleet Management
- EV Management
- Telematics
---
