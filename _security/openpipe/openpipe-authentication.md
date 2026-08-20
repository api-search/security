---
api_key_in: []
api_specs:
- filename: openpipe-chat-api-openapi.yml
  format: yaml
  label: OpenPipe Chat API
  slug: openpipe-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/openapi/openpipe-chat-api-openapi.yml
- filename: openpipe-check-cache-api-openapi.yml
  format: yaml
  label: OpenPipe Check Cache API
  slug: openpipe-check-cache-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/openapi/openpipe-check-cache-api-openapi.yml
- filename: openpipe-criteria-api-openapi.yml
  format: yaml
  label: OpenPipe Criteria API
  slug: openpipe-criteria-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/openapi/openpipe-criteria-api-openapi.yml
- filename: openpipe-datasets-api-openapi.yml
  format: yaml
  label: OpenPipe Datasets API
  slug: openpipe-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/openapi/openpipe-datasets-api-openapi.yml
- filename: openpipe-local-testing-only-get-latest-logged-call-api-openapi.yml
  format: yaml
  label: OpenPipe Local Testing Only Get Latest Logged Call API
  slug: openpipe-local-testing-only-get-latest-logged-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/openapi/openpipe-local-testing-only-get-latest-logged-call-api-openapi.yml
- filename: openpipe-logs-api-openapi.yml
  format: yaml
  label: OpenPipe Logs API
  slug: openpipe-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/openapi/openpipe-logs-api-openapi.yml
- filename: openpipe-models-api-openapi.yml
  format: yaml
  label: OpenPipe Models API
  slug: openpipe-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/openapi/openpipe-models-api-openapi.yml
- filename: openpipe-report-anthropic-api-openapi.yml
  format: yaml
  label: OpenPipe Report Anthropic API
  slug: openpipe-report-anthropic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/openapi/openpipe-report-anthropic-api-openapi.yml
- filename: openpipe-report-api-openapi.yml
  format: yaml
  label: OpenPipe Report API
  slug: openpipe-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/openapi/openpipe-report-api-openapi.yml
- filename: openpipe-unstable-api-openapi.yml
  format: yaml
  label: OpenPipe Unstable API
  slug: openpipe-unstable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/openapi/openpipe-unstable-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openpipe Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenPipe secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenPipe
provider_slug: openpipe
scheme_count: 1
schemes:
- name: Authorization
  scheme: bearer
  sources:
  - openapi/openpipe-openapi.json
  type: http
slug: openpipe-authentication
source_filename: openpipe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openpipe-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: Authorization\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/openpipe-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/authentication/openpipe-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- LLM
- Fine-Tuning
- Distillation
- Inference
- OpenAI-Compatible
- Anthropic Compatible
- Caching
---
