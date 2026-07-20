---
api_key_in: []
api_specs:
- filename: corestory-openapi-original.json
  format: json
  label: CoreStory API
  slug: corestory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corestory/refs/heads/main/openapi/corestory-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Corestory Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoreStory secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CoreStory
provider_slug: corestory
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Enter the Bearer token from Clerk authentication
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/corestory-openapi-original.json
  type: http
slug: corestory-authentication
source_filename: corestory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/corestory-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Enter the Bearer token from Clerk authentication\n  sources:\n  - openapi/corestory-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corestory/refs/heads/main/authentication/corestory-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai
- Code Intelligence
- Legacy Modernization
- Developer Tools
- Code Analysis
- Documentation
- MCP
- Agentic
---
