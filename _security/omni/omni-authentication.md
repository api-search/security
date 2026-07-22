---
api_key_in: []
api_specs:
- filename: omni-openapi-original.yml
  format: yaml
  label: Omni API
  slug: omni-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omni/refs/heads/main/openapi/omni-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Omni Authentication
name_suffix: Authentication
oauth_flows: []
overview: Omni secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Omni
provider_slug: omni
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Can be either an [Organization API Key](/api/authentication#organization-api-keys) or [Personal Access Token (PAT)](/api/authentication#token-types).


    Include in the `Authorization` header as: `Bearer YOUR_TOKEN`'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/omni-openapi-original.yml
  type: http
slug: omni-authentication
source_filename: omni-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/omni-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Can be either an [Organization API Key](/api/authentication#organization-api-keys) or [Personal Access Token (PAT)](/api/authentication#token-types).\n\n    Include in the `Authorization` header as: `Bearer YOUR_TOKEN`\n  sources:\n  - openapi/omni-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omni/refs/heads/main/authentication/omni-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai
- Analytics
- Business Intelligence
- Data
- Embedded Analytics
- Semantic Layer
- MCP
---
