---
api_key_in: []
api_specs:
- filename: codesphere-openapi-original.json
  format: json
  label: Codesphere Public API
  slug: codesphere-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codesphere/refs/heads/main/openapi/codesphere-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Codesphere Authentication
name_suffix: Authentication
oauth_flows: []
overview: Codesphere secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Codesphere
provider_slug: codesphere
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/codesphere-openapi-original.json
  type: http
slug: codesphere-authentication
source_filename: codesphere-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/codesphere-openapi-original.json\ndocs: https://docs.codesphere.com/user-settings/api-keys\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  token_model: Personal Access Token (PAT)\n  header: 'Authorization: Bearer <token>'\n  token_source: https://docs.codesphere.com/user-settings/api-keys\n  notes: >-\n    Tokens are generated in User Settings > API Keys and shown once; the `cs`\n    CLI reads the same token from the CS_TOKEN environment variable.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/codesphere-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codesphere/refs/heads/main/authentication/codesphere-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Saas
- Cloud
- Deployment
- Developer Tools
- Platform as a Service
- Infrastructure
- Sovereign Cloud
- CI/CD
- Managed Services
---
