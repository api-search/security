---
api_key_in: []
api_specs:
- filename: snaplogic-public-apis-openapi.yml
  format: yaml
  label: SnapLogic Public APIs
  slug: snaplogic-public-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snaplogic/refs/heads/main/openapi/snaplogic-public-apis-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Snaplogic Authentication
name_suffix: Authentication
oauth_flows: []
overview: SnapLogic secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SnapLogic
provider_slug: snaplogic
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: JWT token obtained from the SnapLogic authentication endpoint
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/snaplogic-public-apis-openapi.yml
  type: http
- description: Basic authentication with SnapLogic username and password
  name: basicAuth
  scheme: basic
  sources:
  - openapi/snaplogic-public-apis-openapi.yml
  type: http
slug: snaplogic-authentication
source_filename: snaplogic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/snaplogic-public-apis-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token obtained from the SnapLogic authentication endpoint\n  sources:\n  - openapi/snaplogic-public-apis-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication with SnapLogic username and password\n  sources:\n  - openapi/snaplogic-public-apis-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snaplogic/refs/heads/main/authentication/snaplogic-authentication.yml
summary_line: http · 2 schemes
tags:
- AI
- API Management
- Automation
- Data Integration
- Integrations
- iPaaS
- Management
---
