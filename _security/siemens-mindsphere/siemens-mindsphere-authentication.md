---
api_key_in: []
api_specs:
- filename: siemens-mindsphere-asset-management-openapi.yml
  format: yaml
  label: Siemens MindSphere Asset Management API
  slug: asset-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siemens-mindsphere/refs/heads/main/openapi/siemens-mindsphere-asset-management-openapi.yml
- filename: siemens-mindsphere-iot-timeseries-openapi.yml
  format: yaml
  label: Siemens MindSphere IoT Time Series API
  slug: iot-timeseries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siemens-mindsphere/refs/heads/main/openapi/siemens-mindsphere-iot-timeseries-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Siemens Mindsphere Authentication
name_suffix: Authentication
oauth_flows: []
overview: Siemens MindSphere secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Siemens MindSphere
provider_slug: siemens-mindsphere
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/siemens-mindsphere-asset-management-openapi.yml
  - openapi/siemens-mindsphere-iot-timeseries-openapi.yml
  type: http
slug: siemens-mindsphere-authentication
source_filename: siemens-mindsphere-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/siemens-mindsphere-asset-management-openapi.yml, openapi/siemens-mindsphere-iot-timeseries-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/siemens-mindsphere-asset-management-openapi.yml\n  - openapi/siemens-mindsphere-iot-timeseries-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/siemens-mindsphere/refs/heads/main/authentication/siemens-mindsphere-authentication.yml
summary_line: http · 1 scheme
tags:
- IoT
- Industrial
- Digital Twin
- Time Series
- Asset Management
- Industrial IoT
- Insights Hub
---
