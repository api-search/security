---
api_key_in:
- query
api_specs:
- filename: nodeping-openapi.yml
  format: yaml
  label: NodePing API
  slug: nodeping
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nodeping/refs/heads/main/openapi/nodeping-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nodeping Authentication
name_suffix: Authentication
oauth_flows: []
overview: NodePing secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NodePing
provider_slug: nodeping
scheme_count: 2
schemes:
- description: API token passed as the `token` query parameter
  in: query
  name: ApiTokenQuery
  parameter: token
  sources:
  - openapi/nodeping-openapi.yml
  type: apiKey
- description: API token used as the username in HTTP Basic Auth
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/nodeping-openapi.yml
  type: http
slug: nodeping-authentication
source_filename: nodeping-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nodeping-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: ApiTokenQuery\n  type: apiKey\n  in: query\n  parameter: token\n  description: API token passed as the `token` query parameter\n  sources:\n  - openapi/nodeping-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: API token used as the username in HTTP Basic Auth\n  sources:\n  - openapi/nodeping-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nodeping/refs/heads/main/authentication/nodeping-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Monitoring
- Uptime
- Notifications
- SaaS
---
