---
api_key_in:
- header
api_specs:
- filename: swagger.json
  format: json
  label: iNaturalist API v1
  slug: inaturalist-api-v1
  spec_type: OpenAPI
  url: https://api.inaturalist.org/v1/docs/swagger.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Inaturalist Authentication
name_suffix: Authentication
oauth_flows: []
overview: iNaturalist secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: iNaturalist
provider_slug: inaturalist
scheme_count: 1
schemes:
- in: header
  name: api_token
  parameter: Authorization
  sources:
  - openapi/openapi.json
  type: apiKey
slug: inaturalist-authentication
source_filename: inaturalist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/authentication/inaturalist-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Biodiversity
- Nature
- Citizen Science
- Wildlife
- Observations
- Taxa
- Ecology
---
