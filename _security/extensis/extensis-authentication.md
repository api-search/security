---
api_key_in:
- header
api_specs:
- filename: extensis-assets-api-openapi.yml
  format: yaml
  label: Extensis Assets API
  slug: extensis-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensis/refs/heads/main/openapi/extensis-assets-api-openapi.yml
- filename: extensis-catalogs-api-openapi.yml
  format: yaml
  label: Extensis Catalogs API
  slug: extensis-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensis/refs/heads/main/openapi/extensis-catalogs-api-openapi.yml
- filename: extensis-search-api-openapi.yml
  format: yaml
  label: Extensis Search API
  slug: extensis-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensis/refs/heads/main/openapi/extensis-search-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Extensis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Extensis secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Extensis
provider_slug: extensis
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/extensis-portfolio-openapi.json
  type: apiKey
slug: extensis-authentication
source_filename: extensis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/extensis-portfolio-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/extensis-portfolio-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/extensis/refs/heads/main/authentication/extensis-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Digital Asset Management
- Font Management
- Creative Assets
- Font Licensing
- Design Workflows
- DAM
---
