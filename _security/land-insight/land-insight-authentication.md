---
api_key_in:
- header
api_specs:
- filename: land-insight-api-openapi.yml
  format: yaml
  label: LandTech API
  slug: land-insight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/land-insight/refs/heads/main/openapi/land-insight-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Land Insight Authentication
name_suffix: Authentication
oauth_flows: []
overview: Land Insight secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Land Insight
provider_slug: land-insight
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/land-insight-api-openapi.yml
  type: apiKey
slug: land-insight-authentication
source_filename: land-insight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/land-insight-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/land-insight-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/land-insight/refs/heads/main/authentication/land-insight-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Real Estate
- Property
- Land
- Planning
- Geospatial
- Data
- United Kingdom
- PropTech
- Construction
---
