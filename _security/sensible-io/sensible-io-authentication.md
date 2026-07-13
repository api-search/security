---
api_key_in: []
api_specs:
- filename: sensible-io-openapi.yml
  format: yaml
  label: Sensible REST API
  slug: rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-io/refs/heads/main/openapi/sensible-io-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sensible Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sensible secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sensible
provider_slug: sensible-io
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sensible-io-openapi.yml
  type: http
slug: sensible-io-authentication
source_filename: sensible-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sensible-io-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/sensible-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensible-io/refs/heads/main/authentication/sensible-io-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Document AI
- IDP
- Extraction
- LLM
- SenseML
- PDF
---
