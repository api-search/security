---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pickedbyagents-research-api-api-openapi.yml
  format: yaml
  label: Picked by Agents Research API
  slug: pickedbyagents-research-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pickedbyagents/refs/heads/main/openapi/pickedbyagents-research-api-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Pickedbyagents Authentication
name_suffix: Authentication
oauth_flows: []
overview: Picked by Agents secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Picked by Agents
provider_slug: pickedbyagents
scheme_count: 1
schemes:
- name: bearer
  scheme: bearer
  sources:
  - openapi/pickedbyagents-openapi.json
  - openapi/research-api-openapi.json
  type: http
slug: pickedbyagents-authentication
source_filename: pickedbyagents-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: derived\nsource: openapi/pickedbyagents-openapi.json, openapi/research-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/pickedbyagents-openapi.json\n  - openapi/research-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pickedbyagents/refs/heads/main/authentication/pickedbyagents-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Monitoring
- Visibility
- Local Business
---
