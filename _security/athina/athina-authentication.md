---
api_key_in:
- header
api_specs:
- filename: athina-datasets-api-openapi.yml
  format: yaml
  label: Athina AI Datasets API
  slug: athina-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athina/refs/heads/main/openapi/athina-datasets-api-openapi.yml
- filename: athina-evaluations-api-openapi.yml
  format: yaml
  label: Athina AI Evaluations API
  slug: athina-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athina/refs/heads/main/openapi/athina-evaluations-api-openapi.yml
- filename: athina-logging-api-openapi.yml
  format: yaml
  label: Athina AI Logging API
  slug: athina-logging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athina/refs/heads/main/openapi/athina-logging-api-openapi.yml
- filename: athina-prompts-api-openapi.yml
  format: yaml
  label: Athina AI Prompts API
  slug: athina-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athina/refs/heads/main/openapi/athina-prompts-api-openapi.yml
- filename: athina-tracing-api-openapi.yml
  format: yaml
  label: Athina AI Tracing API
  slug: athina-tracing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athina/refs/heads/main/openapi/athina-tracing-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Athina Authentication
name_suffix: Authentication
oauth_flows: []
overview: Athina AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Athina AI
provider_slug: athina
scheme_count: 1
schemes:
- description: Athina API key created in the Athina platform settings.
  in: header
  name: athinaApiKey
  parameter: athina-api-key
  sources:
  - openapi/athina-openapi.yml
  type: apiKey
slug: athina-authentication
source_filename: athina-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/athina-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: athinaApiKey\n  type: apiKey\n  in: header\n  parameter: athina-api-key\n  description: Athina API key created in the Athina platform settings.\n  sources:\n  - openapi/athina-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/athina/refs/heads/main/authentication/athina-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- LLM
- Observability
- Evaluation
- Monitoring
---
