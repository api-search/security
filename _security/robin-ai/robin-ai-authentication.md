---
api_key_in:
- header
api_specs:
- filename: robin-ai-documents-api-openapi.yml
  format: yaml
  label: Robin AI Documents API
  slug: robin-ai-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robin-ai/refs/heads/main/openapi/robin-ai-documents-api-openapi.yml
- filename: robin-ai-groups-api-openapi.yml
  format: yaml
  label: Robin AI Groups API
  slug: robin-ai-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robin-ai/refs/heads/main/openapi/robin-ai-groups-api-openapi.yml
- filename: robin-ai-properties-api-openapi.yml
  format: yaml
  label: Robin AI Properties API
  slug: robin-ai-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robin-ai/refs/heads/main/openapi/robin-ai-properties-api-openapi.yml
- filename: robin-ai-tables-api-openapi.yml
  format: yaml
  label: Robin AI Tables API
  slug: robin-ai-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robin-ai/refs/heads/main/openapi/robin-ai-tables-api-openapi.yml
- filename: robin-ai-templates-api-openapi.yml
  format: yaml
  label: Robin AI Templates API
  slug: robin-ai-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robin-ai/refs/heads/main/openapi/robin-ai-templates-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Robin Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Robin AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Robin AI
provider_slug: robin-ai
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/robin-ai-openapi.yml
  type: apiKey
slug: robin-ai-authentication
source_filename: robin-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/robin-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/robin-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/robin-ai/refs/heads/main/authentication/robin-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Legal
- LegalTech
- Contract Review
- Contract Analysis
- Contract Lifecycle Management
- CLM
- Document Extraction
- Structured Data
- Legal AI
- Artificial Intelligence
- Word Add-In
- Playbook
- Redlining
- Obligation Tracking
- Anthropic
- Claude
---
