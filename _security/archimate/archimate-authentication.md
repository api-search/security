---
api_key_in: []
api_specs:
- filename: archimate-elements-api-openapi.yml
  format: yaml
  label: ArchiMate Elements API
  slug: archimate-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/openapi/archimate-elements-api-openapi.yml
- filename: archimate-models-api-openapi.yml
  format: yaml
  label: ArchiMate Models API
  slug: archimate-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/openapi/archimate-models-api-openapi.yml
- filename: archimate-relationships-api-openapi.yml
  format: yaml
  label: ArchiMate Relationships API
  slug: archimate-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/openapi/archimate-relationships-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Archimate Authentication
name_suffix: Authentication
oauth_flows: []
overview: ArchiMate secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ArchiMate
provider_slug: archimate
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token for ArchiMate repository access
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/archimate-model-exchange-api.yaml
  type: http
slug: archimate-authentication
source_filename: archimate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/archimate-model-exchange-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token for ArchiMate repository access\n  sources:\n  - openapi/archimate-model-exchange-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/authentication/archimate-authentication.yml
summary_line: http · 1 scheme
tags:
- Enterprise Architecture
- Architecture Framework
- Modeling Language
- Business Architecture
- Technology Architecture
- Standard
- Open Group
---
