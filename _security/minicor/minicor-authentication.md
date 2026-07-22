---
api_key_in:
- header
- query
api_specs:
- filename: minicor-openapi.json
  format: json
  label: Laminar API
  slug: laminar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/minicor/refs/heads/main/openapi/minicor-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Minicor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Minicor secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Minicor
provider_slug: minicor
scheme_count: 2
schemes:
- description: API key authentication via query parameter
  in: query
  name: api-key-query
  parameter: api_key
  sources:
  - openapi/minicor-openapi.json
  type: apiKey
- description: API key authentication via header
  in: header
  name: api-key
  parameter: X-API-KEY
  sources:
  - openapi/minicor-openapi.json
  type: apiKey
slug: minicor-authentication
source_filename: minicor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/minicor-openapi.json\ndocs: https://docs.laminar.run/running-an-integration/api-key\nnotes: >-\n  The Laminar external API authenticates with an API key, supplied either as the\n  api_key query parameter (documented primary method) or the X-API-KEY request\n  header. Keys are created and managed in workspace settings. Separately, the\n  Laminar workflow engine can store downstream target-API credentials\n  (AuthCredentials) supporting OAuth client-credentials, OAuth password grant,\n  API key, bearer token, basic and custom auth for the protected endpoints a\n  workflow calls; those are per-workflow secrets, not the Laminar API auth.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: api-key-query\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key authentication via query parameter\n  sources:\n  - openapi/minicor-openapi.json\n- name: api-key\n  type: apiKey\n\
  \  in: header\n  parameter: X-API-KEY\n  description: API key authentication via header\n  sources:\n  - openapi/minicor-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/minicor/refs/heads/main/authentication/minicor-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Desktop Automation
- RPA
- Computer Use Agents
- Workflow Automation
- Healthcare
- Legacy Systems
- AI Agents
- Integration
---
