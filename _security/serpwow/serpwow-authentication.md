---
api_key_in:
- query
api_specs:
- filename: serpwow-openapi.yml
  format: yaml
  label: SerpWow
  slug: serpwow
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serpwow/refs/heads/main/openapi/serpwow-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Serpwow Authentication
name_suffix: Authentication
oauth_flows: []
overview: SerpWow secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SerpWow
provider_slug: serpwow
scheme_count: 1
schemes:
- in: query
  name: apiKeyAuth
  parameter: api_key
  sources:
  - openapi/serpwow-openapi.yml
  type: apiKey
slug: serpwow-authentication
source_filename: serpwow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/serpwow-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/serpwow-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serpwow/refs/heads/main/authentication/serpwow-authentication.yml
summary_line: apiKey · 1 scheme
tags: []
---
