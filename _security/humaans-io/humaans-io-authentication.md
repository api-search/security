---
api_key_in: []
api_specs:
- filename: humaans-api-openapi.yml
  format: yaml
  label: Humaans API
  slug: humaans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Humaans Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Humaans secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Humaans
provider_slug: humaans-io
scheme_count: 1
schemes:
- bearerFormat: token
  description: Bearer access token issued by Humaans with OAuth-style scopes
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/humaans-api-openapi.yml
  type: http
slug: humaans-io-authentication
source_filename: humaans-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/humaans-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  description: Bearer access token issued by Humaans with OAuth-style scopes\n  sources:\n  - openapi/humaans-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/authentication/humaans-io-authentication.yml
summary_line: http · 1 scheme
tags:
- HR
- HRIS
- Human Resources
- People Operations
- People Analytics
- Onboarding
- Offboarding
- Performance Management
- Time Off
- Compensation
- Workflow Automation
- AI Companion
- Agentic AI
- UK
- London
---
