---
api_key_in:
- header
api_specs:
- filename: iceye-catalog-api-openapi.yml
  format: yaml
  label: ICEYE Catalog API
  slug: iceye-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iceye/refs/heads/main/openapi/iceye-catalog-api-openapi.yml
- filename: iceye-company-api-openapi.yml
  format: yaml
  label: ICEYE Company API
  slug: iceye-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iceye/refs/heads/main/openapi/iceye-company-api-openapi.yml
- filename: iceye-tasking-api-openapi.yml
  format: yaml
  label: ICEYE Tasking API
  slug: iceye-tasking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iceye/refs/heads/main/openapi/iceye-tasking-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Iceye Authentication
name_suffix: Authentication
oauth_flows: []
overview: ICEYE secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ICEYE
provider_slug: iceye
scheme_count: 1
schemes:
- description: API key issued by ICEYE.
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/iceye-openapi.yml
  type: apiKey
slug: iceye-authentication
source_filename: iceye-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/iceye-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key issued by ICEYE.\n  sources:\n  - openapi/iceye-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iceye/refs/heads/main/authentication/iceye-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- SAR
- Satellite Imagery
- Earth Observation
- Tasking
- Catalog
- Flood Monitoring
- Disaster Response
- Defense
- ISR
- Geospatial
- All-Weather
---
