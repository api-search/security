---
api_key_in:
- header
api_specs:
- filename: blaxel-agents-api-openapi.yml
  format: yaml
  label: Blaxel Agents API
  slug: blaxel-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-agents-api-openapi.yml
- filename: blaxel-compute-api-openapi.yml
  format: yaml
  label: Blaxel Compute API
  slug: blaxel-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-compute-api-openapi.yml
- filename: blaxel-functions-api-openapi.yml
  format: yaml
  label: Blaxel Functions API
  slug: blaxel-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-functions-api-openapi.yml
- filename: blaxel-integrations-api-openapi.yml
  format: yaml
  label: Blaxel Integrations API
  slug: blaxel-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-integrations-api-openapi.yml
- filename: blaxel-jobs-api-openapi.yml
  format: yaml
  label: Blaxel Jobs API
  slug: blaxel-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-jobs-api-openapi.yml
- filename: blaxel-locations-api-openapi.yml
  format: yaml
  label: Blaxel Locations API
  slug: blaxel-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-locations-api-openapi.yml
- filename: blaxel-models-api-openapi.yml
  format: yaml
  label: Blaxel Models API
  slug: blaxel-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-models-api-openapi.yml
- filename: blaxel-policies-api-openapi.yml
  format: yaml
  label: Blaxel Policies API
  slug: blaxel-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-policies-api-openapi.yml
- filename: blaxel-service-accounts-api-openapi.yml
  format: yaml
  label: Blaxel Service Accounts API
  slug: blaxel-service-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-service-accounts-api-openapi.yml
- filename: blaxel-volumes-api-openapi.yml
  format: yaml
  label: Blaxel Volumes API
  slug: blaxel-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-volumes-api-openapi.yml
- filename: blaxel-workspaces-api-openapi.yml
  format: yaml
  label: Blaxel Workspaces API
  slug: blaxel-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-workspaces-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Blaxel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blaxel secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Blaxel
provider_slug: blaxel
scheme_count: 2
schemes:
- description: API key supplied as "Bearer [example key]".
  in: header
  name: apiKey
  parameter: X-Blaxel-Authorization
  sources:
  - openapi/blaxel-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: OAuth 2.0 short-lived JWT access token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/blaxel-openapi.yml
  type: http
slug: blaxel-authentication
source_filename: blaxel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blaxel-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Blaxel-Authorization\n  description: API key supplied as \"Bearer [example key]\".\n  sources:\n  - openapi/blaxel-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 short-lived JWT access token.\n  sources:\n  - openapi/blaxel-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/authentication/blaxel-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Artificial Intelligence
- Agents
- Infrastructure
- Sandboxes
- MCP
- Compute
- Serverless
---
