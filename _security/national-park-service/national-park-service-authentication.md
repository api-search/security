---
api_key_in:
- header
api_specs:
- filename: national-park-service-openapi.yml
  format: yaml
  label: National Park Service API
  slug: national-park-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: National Park Service Authentication
name_suffix: Authentication
oauth_flows: []
overview: National Park Service secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: National Park Service
provider_slug: national-park-service
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/national-park-service-openapi.yml
  type: apiKey
slug: national-park-service-authentication
source_filename: national-park-service-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/national-park-service-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/national-park-service-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/authentication/national-park-service-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Conservation
- Federal Government
- Parks
---
