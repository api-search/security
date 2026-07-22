---
api_key_in:
- header
api_specs:
- filename: nobueno-openapi-original.json
  format: json
  label: Jungle API
  slug: jungle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nobueno/refs/heads/main/openapi/nobueno-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nobueno Authentication
name_suffix: Authentication
oauth_flows: []
overview: NoBueno secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NoBueno
provider_slug: nobueno
scheme_count: 4
schemes:
- in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/nobueno-openapi-original.json
  type: apiKey
- in: header
  name: Device-type
  parameter: Device-Type
  sources:
  - openapi/nobueno-openapi-original.json
  type: apiKey
- in: header
  name: x-scheme
  parameter: x-scheme
  sources:
  - openapi/nobueno-openapi-original.json
  type: apiKey
- in: header
  name: x-app-id
  parameter: x-app-id
  sources:
  - openapi/nobueno-openapi-original.json
  type: apiKey
slug: nobueno-authentication
source_filename: nobueno-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/nobueno-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/nobueno-openapi-original.json\n- name: Device-type\n  type: apiKey\n  in: header\n  parameter: Device-Type\n  sources:\n  - openapi/nobueno-openapi-original.json\n- name: x-scheme\n  type: apiKey\n  in: header\n  parameter: x-scheme\n  sources:\n  - openapi/nobueno-openapi-original.json\n- name: x-app-id\n  type: apiKey\n  in: header\n  parameter: x-app-id\n  sources:\n  - openapi/nobueno-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nobueno/refs/heads/main/authentication/nobueno-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Company
- Jobs
- Recruiting
- Hiring
- Talent
- Matching
- Human Resources
- Candidates
---
