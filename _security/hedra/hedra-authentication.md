---
api_key_in:
- header
api_specs:
- filename: hedra-web-api-openapi-original.json
  format: json
  label: Hedra Web API
  slug: hedra-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hedra/refs/heads/main/openapi/hedra-web-api-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hedra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hedra secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hedra
provider_slug: hedra
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/hedra-web-api-openapi-original.json
  type: apiKey
slug: hedra-authentication
source_filename: hedra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/hedra-web-api-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/hedra-web-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hedra/refs/heads/main/authentication/hedra-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Generative AI
- Video Generation
- Image Generation
- Audio Generation
- Text to Speech
- Avatars
- Media
- Machine Learning
---
