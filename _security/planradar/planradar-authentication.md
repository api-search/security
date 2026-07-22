---
api_key_in:
- header
api_specs:
- filename: planradar-openapi-original.json
  format: json
  label: PlanRadar Open API
  slug: planradar-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planradar/refs/heads/main/openapi/planradar-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Planradar Authentication
name_suffix: Authentication
oauth_flows: []
overview: PlanRadar secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PlanRadar
provider_slug: planradar
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-PlanRadar-API-Key
  sources:
  - openapi/planradar-openapi-original.json
  type: apiKey
slug: planradar-authentication
source_filename: planradar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/planradar-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-PlanRadar-API-Key\n  sources:\n  - openapi/planradar-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planradar/refs/heads/main/authentication/planradar-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Construction
- Real Estate
- Project Management
- Documentation
- Defect Management
- Field Service
- Facility Management
- BIM
- SaaS
---
