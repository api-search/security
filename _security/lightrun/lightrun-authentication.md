---
api_key_in: []
api_specs:
- filename: lightrun-openapi-original.json
  format: json
  label: Lightrun Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightrun/refs/heads/main/openapi/lightrun-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lightrun Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lightrun secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lightrun
provider_slug: lightrun
scheme_count: 1
schemes:
- name: API Token
  scheme: bearer
  sources:
  - openapi/lightrun-openapi-original.json
  type: http
slug: lightrun-authentication
source_filename: lightrun-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/lightrun-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: API Token\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/lightrun-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightrun/refs/heads/main/authentication/lightrun-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Developer Tools
- Observability
- Debugging
- Monitoring
- Logging
- Application Performance
- Agent Skills
- Model Context Protocol
- DevOps
---
