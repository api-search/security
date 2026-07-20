---
api_key_in:
- header
api_specs:
- filename: bem-openapi-original.yml
  format: yaml
  label: Bem API v3
  slug: bem-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bem/refs/heads/main/openapi/bem-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bem Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bem secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bem
provider_slug: bem
scheme_count: 1
schemes:
- description: Authenticate using API Key in request header
  in: header
  name: API Key
  parameter: x-api-key
  sources:
  - openapi/bem-openapi-original.yml
  type: apiKey
slug: bem-authentication
source_filename: bem-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/bem-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: API Key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Authenticate using API Key in request header\n  sources:\n  - openapi/bem-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bem/refs/heads/main/authentication/bem-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Document Processing
- Unstructured Data
- Data Extraction
- Artificial Intelligence
- LLM
- ETL
- Schema Inference
- Webhooks
---
