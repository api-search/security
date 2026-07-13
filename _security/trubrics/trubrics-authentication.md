---
api_key_in:
- header
api_specs:
- filename: trubrics-openapi.yml
  format: yaml
  label: Trubrics Event Ingestion API
  slug: trubrics-event-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trubrics/refs/heads/main/openapi/trubrics-openapi.yml
- filename: trubrics-openapi.yml
  format: yaml
  label: Trubrics LLM Event Ingestion API
  slug: trubrics-llm-event-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trubrics/refs/heads/main/openapi/trubrics-openapi.yml
- filename: trubrics-openapi.yml
  format: yaml
  label: Trubrics Experiences and Feedback API
  slug: trubrics-experiences-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trubrics/refs/heads/main/openapi/trubrics-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Trubrics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trubrics secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Trubrics
provider_slug: trubrics
scheme_count: 1
schemes:
- description: Project-scoped write-only API key, copied from the project settings page in the Trubrics application.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/trubrics-openapi.yml
  type: apiKey
slug: trubrics-authentication
source_filename: trubrics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trubrics-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Project-scoped write-only API key, copied from the project settings page in the\n    Trubrics application.\n  sources:\n  - openapi/trubrics-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trubrics/refs/heads/main/authentication/trubrics-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- LLM
- Product Analytics
- Event Tracking
- Feedback
---
