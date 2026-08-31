---
api_key_in:
- header
api_specs:
- filename: seam-ai-completions-api-openapi.yml
  format: yaml
  label: Seam AI Completions API
  slug: seam-ai-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seam-ai/refs/heads/main/openapi/seam-ai-completions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Seam Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Seam AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Seam AI
provider_slug: seam-ai
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: Authorization
  sources:
  - openapi/seam-ai-enrichment-openapi.json
  type: apiKey
slug: seam-ai-authentication
source_filename: seam-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/seam-ai-enrichment-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/seam-ai-enrichment-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seam-ai/refs/heads/main/authentication/seam-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai Ml
- Account Based Marketing
- Sales Intelligence
- Marketing
- AI Agents
- CRM
- Data Enrichment
- Intent Data
- Sales Automation
---
