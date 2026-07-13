---
api_key_in:
- header
api_specs:
- filename: ambee-openapi.yml
  format: yaml
  label: Ambee Air Quality API
  slug: air-quality
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambee/refs/heads/main/openapi/ambee-openapi.yml
- filename: ambee-openapi.yml
  format: yaml
  label: Ambee Pollen API
  slug: pollen
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambee/refs/heads/main/openapi/ambee-openapi.yml
- filename: ambee-openapi.yml
  format: yaml
  label: Ambee Weather API
  slug: weather
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambee/refs/heads/main/openapi/ambee-openapi.yml
- filename: ambee-openapi.yml
  format: yaml
  label: Ambee Fire API
  slug: fire
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambee/refs/heads/main/openapi/ambee-openapi.yml
- filename: ambee-openapi.yml
  format: yaml
  label: Ambee Soil API
  slug: soil
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambee/refs/heads/main/openapi/ambee-openapi.yml
- filename: ambee-openapi.yml
  format: yaml
  label: Ambee NDVI / Vegetation API
  slug: ndvi-vegetation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambee/refs/heads/main/openapi/ambee-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ambee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ambee secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ambee
provider_slug: ambee
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/ambee-openapi.yml
  type: apiKey
slug: ambee-authentication
source_filename: ambee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ambee-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/ambee-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambee/refs/heads/main/authentication/ambee-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Environmental Intelligence
- Air Quality
- Weather
- Pollen
- Geospatial
---
