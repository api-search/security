---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: capslane-com-transcript-api-openapi.yml
  format: yaml
  label: capslane-com Transcript API
  slug: capslane-com-transcript-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capslane-com/openapi/capslane-com-transcript-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Capslane Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: capslane-com secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: capslane-com
provider_slug: capslane-com
scheme_count: 1
schemes:
- description: Capslane workspace API key. Keep this value on the server.
  in: header
  name: capslaneApiKey
  parameter: x-api-key
  sources:
  - openapi/capslane-com-openapi.json
  type: apiKey
slug: capslane-com-authentication
source_filename: capslane-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/capslane-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: capslaneApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Capslane workspace API key. Keep this value on the server.\n  sources:\n  - openapi/capslane-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/capslane-com/authentication/capslane-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- API
- YouTube
- Transcript
- AI
---
