---
api_key_in: []
api_specs:
- filename: rossum-annotations-api-openapi.yml
  format: yaml
  label: Rossum Annotations API
  slug: rossum-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rossum/refs/heads/main/openapi/rossum-annotations-api-openapi.yml
- filename: rossum-authentication-api-openapi.yml
  format: yaml
  label: Rossum Authentication API
  slug: rossum-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rossum/refs/heads/main/openapi/rossum-authentication-api-openapi.yml
- filename: rossum-queues-api-openapi.yml
  format: yaml
  label: Rossum Queues API
  slug: rossum-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rossum/refs/heads/main/openapi/rossum-queues-api-openapi.yml
- filename: rossum-schemas-api-openapi.yml
  format: yaml
  label: Rossum Schemas API
  slug: rossum-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rossum/refs/heads/main/openapi/rossum-schemas-api-openapi.yml
- filename: rossum-uploads-api-openapi.yml
  format: yaml
  label: Rossum Uploads API
  slug: rossum-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rossum/refs/heads/main/openapi/rossum-uploads-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rossum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rossum secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rossum
provider_slug: rossum
scheme_count: 1
schemes:
- description: 'Token obtained from POST /auth/login. Pass as

    `Authorization: Bearer <token>`. The legacy `Token <token>` scheme is

    also accepted.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/rossum-openapi.yml
  type: http
slug: rossum-authentication
source_filename: rossum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rossum-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Token obtained from POST /auth/login. Pass as\n    `Authorization: Bearer <token>`. The legacy `Token <token>` scheme is\n    also accepted.\n  sources:\n  - openapi/rossum-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rossum/refs/heads/main/authentication/rossum-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Document AI
- IDP
- Invoices
- OCR
- Workflow
- AP Automation
---
