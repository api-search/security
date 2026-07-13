---
api_key_in:
- header
api_specs:
- filename: log10-logging-openapi.yml
  format: yaml
  label: Log10 LLM Logging API
  slug: log10-llm-logging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/log10/refs/heads/main/openapi/log10-logging-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Log10 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Log10 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Log10
provider_slug: log10
scheme_count: 1
schemes:
- in: header
  name: Log10Token
  parameter: X-Log10-Token
  sources:
  - openapi/log10-logging-openapi.yml
  type: apiKey
slug: log10-authentication
source_filename: log10-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/log10-logging-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Log10Token\n  type: apiKey\n  in: header\n  parameter: X-Log10-Token\n  sources:\n  - openapi/log10-logging-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/log10/refs/heads/main/authentication/log10-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- LLM
- Logging
- Observability
- Evaluation
- Feedback
- Debugging
- LLMOps
- Artificial Intelligence
- Machine Learning
---
