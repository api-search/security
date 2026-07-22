---
api_key_in: []
api_specs:
- filename: traversal-sessions-openapi.yaml
  format: yaml
  label: Traversal Sessions API
  slug: traversal-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traversal/refs/heads/main/openapi/traversal-sessions-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Traversal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Traversal secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Traversal
provider_slug: traversal
scheme_count: 1
schemes:
- description: 'Bearer token in the `Authorization` header — for example,

    `Authorization: Bearer trv_ak_your_api_key_here`. Each key is bound to a

    specific user and organization.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/traversal-sessions-openapi.yaml
  type: http
slug: traversal-authentication
source_filename: traversal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/traversal-sessions-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Bearer token in the `Authorization` header — for example,\n    `Authorization: Bearer trv_ak_your_api_key_here`. Each key is bound to a\n    specific user and organization.\n  sources:\n  - openapi/traversal-sessions-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/traversal/refs/heads/main/authentication/traversal-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- AI SRE
- Site Reliability Engineering
- Observability
- Incident Management
- Root Cause Analysis
- DevOps
- MCP
---
