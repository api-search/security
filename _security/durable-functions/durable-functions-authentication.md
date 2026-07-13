---
api_key_in:
- query
api_specs:
- filename: durable-functions-http-api-openapi.yml
  format: yaml
  label: Azure Durable Functions HTTP API
  slug: durable-functions-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/durable-functions/refs/heads/main/openapi/durable-functions-http-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Durable Functions Authentication
name_suffix: Authentication
oauth_flows: []
overview: Azure Durable Functions secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Azure Durable Functions
provider_slug: durable-functions
scheme_count: 1
schemes:
- in: query
  name: systemKey
  parameter: code
  sources:
  - openapi/durable-functions-http-api-openapi.yml
  type: apiKey
slug: durable-functions-authentication
source_filename: durable-functions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/durable-functions-http-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: systemKey\n  type: apiKey\n  in: query\n  parameter: code\n  sources:\n  - openapi/durable-functions-http-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/durable-functions/refs/heads/main/authentication/durable-functions-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Composition
- Durable Execution
- Serverless Orchestration
- Workflow
---
