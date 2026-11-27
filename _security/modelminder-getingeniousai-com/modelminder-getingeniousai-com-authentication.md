---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: modelminder-getingeniousai-com-openapi.yml
  format: yaml
  label: ModelMinder API
  slug: modelminder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelminder-getingeniousai-com/openapi/modelminder-getingeniousai-com-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: ModelMinder Authentication
name_suffix: Authentication
oauth_flows: []
overview: ModelMinder secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ModelMinder
provider_slug: modelminder-getingeniousai-com
scheme_count: 2
schemes:
- in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/modelminder-getingeniousai-com-openapi.json
  - openapi/modelminder-getingeniousai-com-openapi.yml
  type: apiKey
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/modelminder-getingeniousai-com-openapi.json
  - openapi/modelminder-getingeniousai-com-openapi.yml
  type: http
slug: modelminder-getingeniousai-com-authentication
source_filename: modelminder-getingeniousai-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/modelminder-getingeniousai-com-openapi.json, openapi/modelminder-getingeniousai-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/modelminder-getingeniousai-com-openapi.json\n  - openapi/modelminder-getingeniousai-com-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/modelminder-getingeniousai-com-openapi.json\n  - openapi/modelminder-getingeniousai-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/modelminder-getingeniousai-com/authentication/modelminder-getingeniousai-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Artificial Intelligence
- Model Management
- Monitoring
- Alerts
- Deprecation
---
