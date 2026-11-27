---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getsliq-com-agents-api-openapi.yml
  format: yaml
  label: Sliq Agents API
  slug: getsliq-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getsliq-com/openapi/getsliq-com-agents-api-openapi.yml
- filename: getsliq-com-people-api-openapi.yml
  format: yaml
  label: Sliq People API
  slug: getsliq-com-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getsliq-com/openapi/getsliq-com-people-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Sliq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sliq secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sliq
provider_slug: getsliq-com
scheme_count: 1
schemes:
- name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/getsliq_com.json
  type: http
slug: getsliq-com-authentication
source_filename: getsliq-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/getsliq_com.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/getsliq_com.json\n"
source_yaml_url: https://artifacts.apis.io/getsliq-com/authentication/getsliq-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Outbound Sales
- Sales Outreach
---
