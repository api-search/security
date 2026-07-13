---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Evidently Platform REST API
  slug: evidently-platform-rest-api
  spec_type: OpenAPI
  url: https://docs.evidentlyai.com/api-reference/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Evidently Authentication
name_suffix: Authentication
oauth_flows: []
overview: Evidently AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Evidently AI
provider_slug: evidently
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: Bearer token (API key) obtained from the Evidently platform settings. Set via the Authorization header or the EVIDENTLY_API_KEY environment variable.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/evidently-platform-openapi.yml
  type: http
slug: evidently-authentication
source_filename: evidently-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/evidently-platform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: Bearer token (API key) obtained from the Evidently platform settings. Set via\n    the Authorization header or the EVIDENTLY_API_KEY environment variable.\n  sources:\n  - openapi/evidently-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evidently/refs/heads/main/authentication/evidently-authentication.yml
summary_line: http · 1 scheme
tags:
- ML Monitoring
- LLM Observability
- Data Drift
- Model Performance
- AI Evaluation
- Data Quality
- Open Source
- MLOps
- LLMOps
- Generative AI
---
