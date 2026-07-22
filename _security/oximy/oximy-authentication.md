---
api_key_in:
- header
api_specs:
- filename: oximy-public-api-openapi.yml
  format: yaml
  label: Oximy Public API
  slug: oximy-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oximy/refs/heads/main/openapi/oximy-public-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Oximy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oximy secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Oximy
provider_slug: oximy
scheme_count: 2
schemes:
- description: 'Project API key presented as `Authorization: Bearer <apiKey>`. Keys use the `ox_` prefix.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/oximy-public-api-openapi.yml
  type: http
- description: Project identifier (`proj_` prefix). Sent alongside the bearer key on init and event ingestion.
  in: header
  name: projectId
  parameter: X-Project-Id
  sources:
  - openapi/oximy-public-api-openapi.yml
  type: apiKey
slug: oximy-authentication
source_filename: oximy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/oximy-public-api-openapi.yml\ndocs: https://docs.oximy.com/docs/developer/public-api\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Project API key presented as `Authorization: Bearer <apiKey>`. Keys use the\n    `ox_` prefix.'\n  sources:\n  - openapi/oximy-public-api-openapi.yml\n- name: projectId\n  type: apiKey\n  in: header\n  parameter: X-Project-Id\n  description: Project identifier (`proj_` prefix). Sent alongside the bearer key on init and\n    event ingestion.\n  sources:\n  - openapi/oximy-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oximy/refs/heads/main/authentication/oximy-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- AI Governance
- LLM Observability
- AI Adoption
- Telemetry
- Policy Enforcement
- Artificial Intelligence
- Developer Tools
---
