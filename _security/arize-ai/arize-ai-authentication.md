---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Arize Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arize AI secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Arize AI
provider_slug: arize-ai
scheme_count: 2
schemes:
- description: Arize AX API Key (paired with space_id header).
  in: header
  name: ArizeApiKey
  parameter: api_key
  sources:
  - openapi/arize-ai-openapi.yml
  type: apiKey
- description: Arize AX Space ID.
  in: header
  name: ArizeSpaceId
  parameter: space_id
  sources:
  - openapi/arize-ai-openapi.yml
  type: apiKey
slug: arize-ai-authentication
source_filename: arize-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/arize-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ArizeApiKey\n  type: apiKey\n  in: header\n  parameter: api_key\n  description: Arize AX API Key (paired with space_id header).\n  sources:\n  - openapi/arize-ai-openapi.yml\n- name: ArizeSpaceId\n  type: apiKey\n  in: header\n  parameter: space_id\n  description: Arize AX Space ID.\n  sources:\n  - openapi/arize-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arize-ai/refs/heads/main/authentication/arize-ai-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- LLM Observability
- ML Monitoring
- Open Source
- OpenTelemetry
- Phoenix
- Tracing
- Evaluation
---
