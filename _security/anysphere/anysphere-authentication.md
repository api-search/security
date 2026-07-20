---
api_key_in: []
api_specs:
- filename: anysphere-cloud-agents-openapi-original.yml
  format: yaml
  label: Cursor Cloud Agents API
  slug: cursor-cloud-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anysphere/refs/heads/main/openapi/anysphere-cloud-agents-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Anysphere Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anysphere secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Anysphere
provider_slug: anysphere
scheme_count: 2
schemes:
- description: 'API key from Cursor Dashboard, supplied as the Basic

    Authentication username with an empty password.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/anysphere-cloud-agents-openapi-original.yml
  type: http
- description: 'API key from Cursor Dashboard, supplied via

    `Authorization: Bearer <key>`. Equivalent to Basic Auth.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/anysphere-cloud-agents-openapi-original.yml
  type: http
slug: anysphere-authentication
source_filename: anysphere-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/anysphere-cloud-agents-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    API key from Cursor Dashboard, supplied as the Basic\n    Authentication username with an empty password.\n  sources:\n  - openapi/anysphere-cloud-agents-openapi-original.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    API key from Cursor Dashboard, supplied via\n    `Authorization: Bearer <key>`. Equivalent to Basic Auth.\n  sources:\n  - openapi/anysphere-cloud-agents-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anysphere/refs/heads/main/authentication/anysphere-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Developer Tools
- Artificial Intelligence
- Code Editor
- Coding Agents
- Cloud Agents
- Developer Productivity
- IDE
---
