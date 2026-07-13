---
api_key_in: []
api_specs:
- filename: bubble-data-api-openapi.yml
  format: yaml
  label: Bubble Data API
  slug: bubble-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bubble/refs/heads/main/openapi/bubble-data-api-openapi.yml
- filename: bubble-workflow-api-openapi.yml
  format: yaml
  label: Bubble Workflow API
  slug: bubble-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bubble/refs/heads/main/openapi/bubble-workflow-api-openapi.yml
- filename: bubble-plugin-api-openapi.yml
  format: yaml
  label: Bubble Plugin API
  slug: bubble-plugin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bubble/refs/heads/main/openapi/bubble-plugin-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bubble Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bubble secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bubble
provider_slug: bubble
scheme_count: 1
schemes:
- bearerFormat: API Token
  description: 'Send the API token in the `Authorization` header as `Bearer <token>`.

    Admin tokens bypass privacy rules; user tokens (returned by the

    `Log the User in` workflow action) enforce privacy rules per user.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/bubble-data-api-openapi.yml
  - openapi/bubble-workflow-api-openapi.yml
  type: http
slug: bubble-authentication
source_filename: bubble-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bubble-data-api-openapi.yml, openapi/bubble-workflow-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Token\n  description: |-\n    Send the API token in the `Authorization` header as `Bearer <token>`.\n    Admin tokens bypass privacy rules; user tokens (returned by the\n    `Log the User in` workflow action) enforce privacy rules per user.\n  sources:\n  - openapi/bubble-data-api-openapi.yml\n  - openapi/bubble-workflow-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bubble/refs/heads/main/authentication/bubble-authentication.yml
summary_line: http · 1 scheme
tags:
- No-Code
- Application Platform
- Database
- Workflow Automation
- Plugins
---
