---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: halo-h5pc-api-openapi.yml
  format: yaml
  label: Halo H5pc API
  slug: halo-h5pc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/halo/openapi/halo-h5pc-api-openapi.yml
- filename: halo-h5-api-openapi.yml
  format: yaml
  label: Halo H5 API
  slug: halo-h5-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/halo/openapi/halo-h5-api-openapi.yml
- filename: halo-hw2-api-openapi.yml
  format: yaml
  label: Halo Hw2 API
  slug: halo-hw2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/halo/openapi/halo-hw2-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Halo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Halo secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Halo
provider_slug: halo
scheme_count: 2
schemes:
- in: header
  name: apiKeyHeader
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/halo-metadata-openapi.yml
  - openapi/halo-profile-openapi.yml
  - openapi/halo-stats-openapi.yml
  - openapi/halo-ugc-openapi.yml
  type: apiKey
- in: query
  name: apiKeyQuery
  parameter: subscription-key
  sources:
  - openapi/halo-metadata-openapi.yml
  - openapi/halo-profile-openapi.yml
  - openapi/halo-stats-openapi.yml
  - openapi/halo-ugc-openapi.yml
  type: apiKey
slug: halo-authentication
source_filename: halo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/halo-metadata-openapi.yml, openapi/halo-profile-openapi.yml, openapi/halo-stats-openapi.yml,\n  openapi/halo-ugc-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  sources:\n  - openapi/halo-metadata-openapi.yml\n  - openapi/halo-profile-openapi.yml\n  - openapi/halo-stats-openapi.yml\n  - openapi/halo-ugc-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  sources:\n  - openapi/halo-metadata-openapi.yml\n  - openapi/halo-profile-openapi.yml\n  - openapi/halo-stats-openapi.yml\n  - openapi/halo-ugc-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/halo/authentication/halo-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Game Data
- Gaming
- Halo
- Microsoft
- Player Statistics
- Public APIs
- Video Games
- Xbox
---
