---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: ZoomEye Authentication
name_suffix: Authentication
oauth_flows: []
overview: ZoomEye secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ZoomEye
provider_slug: zoomeye
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: API-KEY
  sources:
  - openapi/zoomeye-openapi.json
  type: apiKey
slug: zoomeye-authentication
source_filename: zoomeye-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/zoomeye-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: API-KEY\n  sources:\n  - openapi/zoomeye-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/zoomeye/authentication/zoomeye-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cybersecurity
- Search Engines
- Asset Discovery
---
