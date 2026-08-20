---
api_key_in:
- header
api_specs:
- filename: langtrace-projects-api-openapi.yml
  format: yaml
  label: Langtrace AI Projects API
  slug: langtrace-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langtrace/refs/heads/main/openapi/langtrace-projects-api-openapi.yml
- filename: langtrace-prompt-registry-api-openapi.yml
  format: yaml
  label: Langtrace AI Prompt Registry API
  slug: langtrace-prompt-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langtrace/refs/heads/main/openapi/langtrace-prompt-registry-api-openapi.yml
- filename: langtrace-traces-api-openapi.yml
  format: yaml
  label: Langtrace AI Traces API
  slug: langtrace-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langtrace/refs/heads/main/openapi/langtrace-traces-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Langtrace Authentication
name_suffix: Authentication
oauth_flows: []
overview: Langtrace AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Langtrace AI
provider_slug: langtrace
scheme_count: 1
schemes:
- description: Project-level (or team-level for project creation) API key.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/langtrace-openapi.yml
  type: apiKey
slug: langtrace-authentication
source_filename: langtrace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/langtrace-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Project-level (or team-level for project creation) API key.\n  sources:\n  - openapi/langtrace-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langtrace/refs/heads/main/authentication/langtrace-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- LLM
- Observability
- OpenTelemetry
- Tracing
- Open-Source
---
