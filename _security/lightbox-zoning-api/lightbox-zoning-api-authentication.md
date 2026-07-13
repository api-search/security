---
api_key_in:
- header
api_specs:
- filename: lightbox-zoning-api-openapi.yml
  format: yaml
  label: LightBox Zoning API
  slug: lightbox-zoning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightbox-zoning-api/refs/heads/main/openapi/lightbox-zoning-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lightbox Zoning Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: LightBox Zoning API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LightBox Zoning API
provider_slug: lightbox-zoning-api
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/lightbox-zoning-api-openapi.yml
  type: apiKey
slug: lightbox-zoning-api-authentication
source_filename: lightbox-zoning-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lightbox-zoning-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/lightbox-zoning-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightbox-zoning-api/refs/heads/main/authentication/lightbox-zoning-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Zoning
- Real Estate
- CRE
- Property
- Parcels
- Geospatial
- Land Use
---
