---
api_key_in:
- header
api_specs:
- filename: exa-openapi.yml
  format: yaml
  label: Exa Search API
  slug: search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa/refs/heads/main/openapi/exa-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Exa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Exa secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Exa
provider_slug: exa
scheme_count: 2
schemes:
- in: header
  name: apiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/exa-openapi.yml
  type: apiKey
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/exa-openapi.yml
  type: http
slug: exa-authentication
source_filename: exa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/exa-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/exa-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/exa-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exa/refs/heads/main/authentication/exa-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Search
- Neural Search
- AI Agents
- LLMs
- Web Index
- Retrieval
- Answer
- Contents
- Find Similar
- Research
- SOC 2
- MCP
---
