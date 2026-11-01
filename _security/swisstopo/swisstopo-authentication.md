---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: swisstopo-layers-api-openapi.yml
  format: yaml
  label: swisstopo Layers API
  slug: swisstopo-layers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swisstopo/openapi/swisstopo-layers-api-openapi.yml
- filename: swisstopo-vocabularies-api-openapi.yml
  format: yaml
  label: swisstopo Vocabularies API
  slug: swisstopo-vocabularies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swisstopo/openapi/swisstopo-vocabularies-api-openapi.yml
- filename: swisstopo-wms-api-openapi.yml
  format: yaml
  label: swisstopo WMS API
  slug: swisstopo-wms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swisstopo/openapi/swisstopo-wms-api-openapi.yml
- filename: swisstopo-wmts-api-openapi.yml
  format: yaml
  label: swisstopo WMTS API
  slug: swisstopo-wmts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swisstopo/openapi/swisstopo-wmts-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Swisstopo Authentication
name_suffix: Authentication
oauth_flows: []
overview: swisstopo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: swisstopo
provider_slug: swisstopo
scheme_count: 1
schemes:
- description: API key required to access all endpoints of the SwissTopo WebMap Semantic Filtering API.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/swissgeol-lexic-webmap-api.yaml
  - openapi/swisstopo-openapi.yml
  type: apiKey
slug: swisstopo-authentication
source_filename: swisstopo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: derived\nsource: openapi/swissgeol-lexic-webmap-api.yaml, openapi/swisstopo-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key required to access all endpoints of the SwissTopo WebMap Semantic Filtering\n    API.\n  sources:\n  - openapi/swissgeol-lexic-webmap-api.yaml\n  - openapi/swisstopo-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/swisstopo/authentication/swisstopo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Geodata
- Government
- Switzerland
- Mapping
- OpenData
---
