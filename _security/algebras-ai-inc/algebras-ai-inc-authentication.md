---
api_key_in:
- header
api_specs:
- filename: algebras-ai-inc-openapi-original.json
  format: json
  label: Algebras API
  slug: algebras-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algebras-ai-inc/refs/heads/main/openapi/algebras-ai-inc-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Algebras Ai Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Algebras AI Inc. secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Algebras AI Inc.
provider_slug: algebras-ai-inc
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/algebras-ai-inc-openapi-original.json
  type: apiKey
slug: algebras-ai-inc-authentication
source_filename: algebras-ai-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/algebras-ai-inc-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/algebras-ai-inc-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/algebras-ai-inc/refs/heads/main/authentication/algebras-ai-inc-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Translation
- Localization
- Internationalization
- Artificial Intelligence
- Machine Translation
- Voice
- Video
- Developer Tools
---
