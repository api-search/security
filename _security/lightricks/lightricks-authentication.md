---
api_key_in: []
api_specs:
- filename: lightricks-ltx-openapi.yml
  format: yaml
  label: LTX API
  slug: ltx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightricks/refs/heads/main/openapi/lightricks-ltx-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lightricks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lightricks secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lightricks
provider_slug: lightricks
scheme_count: 1
schemes:
- description: API key authentication
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lightricks-ltx-openapi-original.json
  - openapi/lightricks-ltx-openapi.yml
  type: http
slug: lightricks-authentication
source_filename: lightricks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/lightricks-ltx-openapi-original.json, openapi/lightricks-ltx-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key authentication\n  sources:\n  - openapi/lightricks-ltx-openapi-original.json\n  - openapi/lightricks-ltx-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightricks/refs/heads/main/authentication/lightricks-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Consumer
- Artificial Intelligence
- Generative AI
- Video
- Video Generation
- Media
- Machine Learning
- Creative Tools
---
