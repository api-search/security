---
api_key_in:
- header
api_specs:
- filename: julep-openapi-original.yml
  format: yaml
  label: Julep API
  slug: julep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/julep/refs/heads/main/openapi/julep-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Julep Authentication
name_suffix: Authentication
oauth_flows: []
overview: Julep secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Julep
provider_slug: julep
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/julep-openapi-original.yml
  type: apiKey
- in: header
  name: ApiKeyAuth_
  parameter: X-Auth-Key
  sources:
  - openapi/julep-openapi-original.yml
  type: apiKey
slug: julep-authentication
source_filename: julep-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/julep-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/julep-openapi-original.yml\n- name: ApiKeyAuth_\n  type: apiKey\n  in: header\n  parameter: X-Auth-Key\n  sources:\n  - openapi/julep-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/julep/refs/heads/main/authentication/julep-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- AI Agents
- LLM
- Agents
- Workflows
- RAG
- Memory
- Orchestration
- Developer Tools
- Open Source
---
