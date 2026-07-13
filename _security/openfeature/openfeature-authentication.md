---
api_key_in:
- header
api_specs:
- filename: openfeature-openapi.yaml
  format: yaml
  label: OpenFeature Evaluation API
  slug: openfeature-spec
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfeature/refs/heads/main/openapi/openfeature-openapi.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openfeature Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenFeature secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OpenFeature
provider_slug: openfeature
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: "Optional Bearer token authentication. If supported by the flag management system, \nclients can authenticate using a Bearer token in the `Authorization` header following \nthe format: `Authorization: Bearer <token>`."
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/openfeature-openapi.yaml
  type: http
- description: "Optional API key authentication. If supported by the flag management system, clients \ncan authenticate by providing an API key in the `X-API-Key` header."
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/openfeature-openapi.yaml
  type: apiKey
slug: openfeature-authentication
source_filename: openfeature-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openfeature-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: \"Optional Bearer token authentication. If supported by the flag management system,\\\n    \\ \\nclients can authenticate using a Bearer token in the `Authorization` header following\\\n    \\ \\nthe format: `Authorization: Bearer <token>`.\"\n  sources:\n  - openapi/openfeature-openapi.yaml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: \"Optional API key authentication. If supported by the flag management system,\\\n    \\ clients \\ncan authenticate by providing an API key in the `X-API-Key` header.\"\n  sources:\n  - openapi/openfeature-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openfeature/refs/heads/main/authentication/openfeature-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Cloud Native
- Feature Flags
- Feature Management
- Incubating
- SDKs
- Specification
---
