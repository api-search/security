---
api_key_in: []
api_specs:
- filename: insomnia-mock-logs-api-openapi.yml
  format: yaml
  label: Insomnia Mock Logs API
  slug: insomnia-mock-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insomnia/refs/heads/main/openapi/insomnia-mock-logs-api-openapi.yml
- filename: insomnia-mock-routes-api-openapi.yml
  format: yaml
  label: Insomnia Mock Routes API
  slug: insomnia-mock-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insomnia/refs/heads/main/openapi/insomnia-mock-routes-api-openapi.yml
- filename: insomnia-mock-servers-api-openapi.yml
  format: yaml
  label: Insomnia Mock Servers API
  slug: insomnia-mock-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insomnia/refs/heads/main/openapi/insomnia-mock-servers-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Insomnia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Insomnia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Insomnia
provider_slug: insomnia
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Insomnia cloud authentication token for accessing mock server management endpoints.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/insomnia-mock-server-openapi.yml
  type: http
slug: insomnia-authentication
source_filename: insomnia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/insomnia-mock-server-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Insomnia cloud authentication token for accessing mock server management endpoints.\n  sources:\n  - openapi/insomnia-mock-server-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insomnia/refs/heads/main/authentication/insomnia-authentication.yml
summary_line: http · 1 scheme
tags:
- API Design
- CLI
- Clients
- Mocking
- Platform
- Testing
---
