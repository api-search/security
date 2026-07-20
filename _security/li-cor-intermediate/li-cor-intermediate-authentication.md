---
api_key_in: []
api_specs:
- filename: li-cor-intermediate-hobolink-openapi.json
  format: json
  label: HOBOLINK External API
  slug: hobolink-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/li-cor-intermediate/refs/heads/main/openapi/li-cor-intermediate-hobolink-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Li Cor Intermediate Authentication
name_suffix: Authentication
oauth_flows: []
overview: LI-COR Intermediate secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LI-COR Intermediate
provider_slug: li-cor-intermediate
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/li-cor-intermediate-hobolink-openapi.json
  type: http
slug: li-cor-intermediate-authentication
source_filename: li-cor-intermediate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/li-cor-intermediate-hobolink-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/li-cor-intermediate-hobolink-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/li-cor-intermediate/refs/heads/main/authentication/li-cor-intermediate-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Environmental Monitoring
- Greenhouse Gas
- Climate
- Agriculture
- Sensors
- Data Loggers
- IoT
- Scientific Instruments
- Life Sciences
- Time Series Data
---
