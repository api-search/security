---
api_key_in:
- query
api_specs:
- filename: apicontext-platform-openapi.yaml
  format: yaml
  label: APIContext Synthetic API Testing
  slug: synthetic-api-testing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-platform-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Apicontext Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIContext secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: APIContext
provider_slug: apicontext
scheme_count: 1
schemes:
- in: query
  name: ApiTokenAuth
  parameter: _token
  sources:
  - openapi/apicontext-platform-openapi.yaml
  type: apiKey
slug: apicontext-authentication
source_filename: apicontext-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apicontext-platform-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiTokenAuth\n  type: apiKey\n  in: query\n  parameter: _token\n  sources:\n  - openapi/apicontext-platform-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/authentication/apicontext-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Directory
- API Monitoring
- Conformance
- Performance
- Platform
- SLO
- Synthetic Testing
- Testing
---
