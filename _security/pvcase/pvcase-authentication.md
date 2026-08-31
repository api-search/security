---
api_key_in: []
api_specs:
- filename: pvcase-asset-api-openapi.yml
  format: yaml
  label: PVcase Asset API
  slug: pvcase-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pvcase/refs/heads/main/openapi/pvcase-asset-api-openapi.yml
- filename: pvcase-company-api-openapi.yml
  format: yaml
  label: PVcase Company API
  slug: pvcase-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pvcase/refs/heads/main/openapi/pvcase-company-api-openapi.yml
- filename: pvcase-project-api-openapi.yml
  format: yaml
  label: PVcase Project API
  slug: pvcase-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pvcase/refs/heads/main/openapi/pvcase-project-api-openapi.yml
- filename: pvcase-team-api-openapi.yml
  format: yaml
  label: PVcase Team API
  slug: pvcase-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pvcase/refs/heads/main/openapi/pvcase-team-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pvcase Authentication
name_suffix: Authentication
oauth_flows: []
overview: PVcase secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PVcase
provider_slug: pvcase
scheme_count: 1
schemes:
- description: AO Username and API Token Authentication
  name: basicAuth
  scheme: basic
  sources:
  - openapi/pvcase-anderson-optimization-openapi.json
  type: http
slug: pvcase-authentication
source_filename: pvcase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/pvcase-anderson-optimization-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: AO Username and API Token Authentication\n  sources:\n  - openapi/pvcase-anderson-optimization-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pvcase/refs/heads/main/authentication/pvcase-authentication.yml
summary_line: http · 1 scheme
tags:
- Solar
- Energy
- Renewable Energy
- Photovoltaic
- Geospatial
- Site Selection
- Engineering Design
- Simulation
- Project Development
- CAD
---
