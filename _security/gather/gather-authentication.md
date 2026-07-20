---
api_key_in:
- header
api_specs:
- filename: gather-http-api-openapi.yml
  format: yaml
  label: Gather HTTP API
  slug: gather-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gather/refs/heads/main/openapi/gather-http-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Gather Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gather secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gather
provider_slug: gather
scheme_count: 1
schemes:
- description: API key generated at https://gather.town/apiKeys, sent in the apiKey request header. The associated user must have Admin or Builder permission on the target space.
  in: header
  name: apiKey
  parameter: apiKey
  sources:
  - openapi/gather-http-api-openapi.yml
  type: apiKey
slug: gather-authentication
source_filename: gather-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/gather-http-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: apiKey\n  description: API key generated at https://gather.town/apiKeys, sent in the apiKey request\n    header. The associated user must have Admin or Builder permission on the target space.\n  sources:\n  - openapi/gather-http-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gather/refs/heads/main/authentication/gather-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Future Of Work
- Virtual Office
- Video Conferencing
- Collaboration
- Metaverse
- Remote Work
- Events
---
