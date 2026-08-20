---
api_key_in: []
api_specs:
- filename: caspio-applications-api-openapi.yml
  format: yaml
  label: Caspio Applications API
  slug: caspio-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caspio/refs/heads/main/openapi/caspio-applications-api-openapi.yml
- filename: caspio-authentication-api-openapi.yml
  format: yaml
  label: Caspio Authentication API
  slug: caspio-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caspio/refs/heads/main/openapi/caspio-authentication-api-openapi.yml
- filename: caspio-files-api-openapi.yml
  format: yaml
  label: Caspio Files API
  slug: caspio-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caspio/refs/heads/main/openapi/caspio-files-api-openapi.yml
- filename: caspio-tables-api-openapi.yml
  format: yaml
  label: Caspio Tables API
  slug: caspio-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caspio/refs/heads/main/openapi/caspio-tables-api-openapi.yml
- filename: caspio-tasks-api-openapi.yml
  format: yaml
  label: Caspio Tasks API
  slug: caspio-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caspio/refs/heads/main/openapi/caspio-tasks-api-openapi.yml
- filename: caspio-users-api-openapi.yml
  format: yaml
  label: Caspio Users API
  slug: caspio-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caspio/refs/heads/main/openapi/caspio-users-api-openapi.yml
- filename: caspio-views-api-openapi.yml
  format: yaml
  label: Caspio Views API
  slug: caspio-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caspio/refs/heads/main/openapi/caspio-views-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Caspio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Caspio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Caspio
provider_slug: caspio
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/caspio-openapi.yml
  type: http
slug: caspio-authentication
source_filename: caspio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/caspio-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/caspio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caspio/refs/heads/main/authentication/caspio-authentication.yml
summary_line: http · 1 scheme
tags:
- Low-Code
- No-Code
- Database
- Application Platform
- Cloud Database
- Online Forms
- Workflow-Automation
---
