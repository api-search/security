---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: direct-freight-boards-api-openapi.yml
  format: yaml
  label: Direct Freight Boards API
  slug: direct-freight-boards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/direct-freight/openapi/direct-freight-boards-api-openapi.yml
- filename: direct-freight-end-user-authentications-api-openapi.yml
  format: yaml
  label: Direct Freight End User Authentications API
  slug: direct-freight-end-user-authentications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/direct-freight/openapi/direct-freight-end-user-authentications-api-openapi.yml
- filename: direct-freight-locations-api-openapi.yml
  format: yaml
  label: Direct Freight Locations API
  slug: direct-freight-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/direct-freight/openapi/direct-freight-locations-api-openapi.yml
- filename: direct-freight-postings-api-openapi.yml
  format: yaml
  label: Direct Freight Postings API
  slug: direct-freight-postings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/direct-freight/openapi/direct-freight-postings-api-openapi.yml
- filename: direct-freight-profiles-api-openapi.yml
  format: yaml
  label: Direct Freight Profiles API
  slug: direct-freight-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/direct-freight/openapi/direct-freight-profiles-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Direct Freight Authentication
name_suffix: Authentication
oauth_flows: []
overview: Direct Freight secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Direct Freight
provider_slug: direct-freight
scheme_count: 1
schemes:
- in: header
  name: api-token
  parameter: api-token
  sources:
  - openapi/direct-freight-openapi.json
  type: apiKey
slug: direct-freight-authentication
source_filename: direct-freight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/direct-freight-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api-token\n  type: apiKey\n  in: header\n  parameter: api-token\n  sources:\n  - openapi/direct-freight-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/direct-freight/authentication/direct-freight-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Load Board
- Freight Brokers
- Shippers
- Carrier
- Owner Operators
- Freight Rate Tool
- Mileage Calculator
---
