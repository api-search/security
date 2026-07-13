---
api_key_in: []
api_specs:
- filename: siemens-building-operations-openapi.yml
  format: yaml
  label: Siemens Building Operations API
  slug: building-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siemens/refs/heads/main/openapi/siemens-building-operations-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Siemens Authentication
name_suffix: Authentication
oauth_flows: []
overview: Siemens secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Siemens
provider_slug: siemens
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token from Siemens Building X identity service
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/siemens-building-operations-openapi.yml
  type: http
slug: siemens-authentication
source_filename: siemens-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/siemens-building-operations-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token from Siemens Building X identity service\n  sources:\n  - openapi/siemens-building-operations-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/siemens/refs/heads/main/authentication/siemens-authentication.yml
summary_line: http · 1 scheme
tags:
- Automation
- Electrification
- Industry
- Manufacturing
- Building Automation
- Industrial IoT
- Smart Buildings
- Digital Twin
---
