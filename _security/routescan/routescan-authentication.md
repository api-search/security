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
name: Routescan Authentication
name_suffix: Authentication
oauth_flows: []
overview: Routescan secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Routescan
provider_slug: routescan
scheme_count: 1
schemes:
- description: Api Key
  in: header
  name: apiKey
  parameter: apikey
  sources:
  - openapi/routescan-openapi.json
  type: apiKey
slug: routescan-authentication
source_filename: routescan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: derived\nsource: openapi/routescan-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: Api Key\n  sources:\n  - openapi/routescan-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/routescan/authentication/routescan-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
---
