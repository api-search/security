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
name: Ingenious AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ingenious AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ingenious AI
provider_slug: admt-getingeniousai-com
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/admt-getingeniousai-com-openapi.json
  type: apiKey
slug: admt-getingeniousai-com-authentication
source_filename: admt-getingeniousai-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/admt-getingeniousai-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/admt-getingeniousai-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/admt-getingeniousai-com/authentication/admt-getingeniousai-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Compliance
- Automation
- Small Business
---
