---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: gatiflow-openapi.yml
  format: yaml
  label: GatiFlow Intelligence API
  slug: gatiflow-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gatiflow/refs/heads/main/openapi/gatiflow-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Gatiflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: GatiFlow secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GatiFlow
provider_slug: gatiflow
scheme_count: 2
schemes:
- description: API key (prefix gf_) created in Dashboard → API Keys.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/gatiflow-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: Web session token issued to the browser at sign-in. It is not part of the public API and cannot be created from an API key; an API key sent to an operation that requires it receives 401.
  name: SessionBearer
  scheme: bearer
  sources:
  - openapi/gatiflow-openapi.yml
  type: http
slug: gatiflow-authentication
source_filename: gatiflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: derived\nsource: openapi/gatiflow-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key (prefix gf_) created in Dashboard → API Keys.\n  sources:\n  - openapi/gatiflow-openapi.yml\n- name: SessionBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Web session token issued to the browser at sign-in. It is not part of the public\n    API and cannot be created from an API key; an API key sent to an operation that requires\n    it receives 401.\n  sources:\n  - openapi/gatiflow-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gatiflow/refs/heads/main/authentication/gatiflow-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Market Intelligence
- Developer Signals
- Trends
- Hiring
- Open Source
- Research
- B2B SaaS
- Artificial Intelligence
---
