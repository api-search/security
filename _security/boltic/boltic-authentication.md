---
api_key_in: []
api_specs:
- filename: boltic-gateway-api-openapi.yml
  format: yaml
  label: Boltic Gateway API
  slug: gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-gateway-api-openapi.yml
- filename: boltic-workflow-api-openapi.yml
  format: yaml
  label: Boltic Workflow API
  slug: workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-workflow-api-openapi.yml
- filename: boltic-tables-api-openapi.yml
  format: yaml
  label: Boltic Tables API
  slug: tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-tables-api-openapi.yml
- filename: boltic-pipes-api-openapi.yml
  format: yaml
  label: Boltic Pipes API
  slug: pipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-pipes-api-openapi.yml
- filename: boltic-streams-api-openapi.yml
  format: yaml
  label: Boltic Streams API
  slug: streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-streams-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Boltic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Boltic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Boltic
provider_slug: boltic
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/boltic-gateway-api-openapi.yml
  - openapi/boltic-pipes-api-openapi.yml
  - openapi/boltic-streams-api-openapi.yml
  - openapi/boltic-tables-api-openapi.yml
  - openapi/boltic-workflow-api-openapi.yml
  type: http
slug: boltic-authentication
source_filename: boltic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/boltic-gateway-api-openapi.yml, openapi/boltic-pipes-api-openapi.yml, openapi/boltic-streams-api-openapi.yml,\n  openapi/boltic-tables-api-openapi.yml, openapi/boltic-workflow-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/boltic-gateway-api-openapi.yml\n  - openapi/boltic-pipes-api-openapi.yml\n  - openapi/boltic-streams-api-openapi.yml\n  - openapi/boltic-tables-api-openapi.yml\n  - openapi/boltic-workflow-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/authentication/boltic-authentication.yml
summary_line: http · 1 scheme
tags:
- Automation
- DataSync
- Gateways
- NoCode
- Streaming
- Workflows
---
