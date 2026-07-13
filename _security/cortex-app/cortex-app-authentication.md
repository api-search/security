---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cortex App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cortex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cortex
provider_slug: cortex-app
scheme_count: 1
schemes:
- bearerFormat: Personal Access Token
  description: 'Provide a Cortex personal access token using `Authorization: Bearer

    <CORTEX_TOKEN>`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/cortex-app-openapi.yml
  type: http
slug: cortex-app-authentication
source_filename: cortex-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cortex-app-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Personal Access Token\n  description: |-\n    Provide a Cortex personal access token using `Authorization: Bearer\n    <CORTEX_TOKEN>`.\n  sources:\n  - openapi/cortex-app-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cortex-app/refs/heads/main/authentication/cortex-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Internal Developer Portal
- Service Catalog
- Scorecards
- Platform Engineering
- Developer Experience
- SRE
---
