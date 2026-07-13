---
api_key_in:
- query
api_specs:
- filename: 123formbuilder-rest-api-v2-openapi.yml
  format: yaml
  label: 123FormBuilder REST API v2
  slug: rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/123formbuilder/refs/heads/main/openapi/123formbuilder-rest-api-v2-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: 123Formbuilder Authentication
name_suffix: Authentication
oauth_flows: []
overview: 123FormBuilder secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 123FormBuilder
provider_slug: 123formbuilder
scheme_count: 1
schemes:
- description: JWT token obtained from POST /token, supplied as the JWT query parameter.
  in: query
  name: JWTQuery
  parameter: JWT
  sources:
  - openapi/123formbuilder-rest-api-v2-openapi.yml
  type: apiKey
slug: 123formbuilder-authentication
source_filename: 123formbuilder-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/123formbuilder-rest-api-v2-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: JWTQuery\n  type: apiKey\n  in: query\n  parameter: JWT\n  description: JWT token obtained from POST /token, supplied as the JWT query parameter.\n  sources:\n  - openapi/123formbuilder-rest-api-v2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/123formbuilder/refs/heads/main/authentication/123formbuilder-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Online Forms
- Form Builder
- Surveys
- Workflow
- Data Collection
- Submissions
- Webhooks
- HIPAA
- GDPR
- Payments
---
