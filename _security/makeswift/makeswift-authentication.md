---
api_key_in:
- header
api_specs:
- filename: makeswift-openapi.json
  format: json
  label: Makeswift REST API
  slug: makeswift-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/makeswift/refs/heads/main/openapi/makeswift-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Makeswift Authentication
name_suffix: Authentication
oauth_flows: []
overview: Makeswift secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Makeswift
provider_slug: makeswift
scheme_count: 1
schemes:
- description: 'API key authentication. Accepts either:

    - App API key (e.g. sk_eczMHVBY9fV6GYFhvs53qcnxq7yptlXL3ABKOZtn6dQ)

    - Site API key (UUID format, e.g. 550e8400-e29b-41d4-a716-446655440000)'
  in: header
  name: Authentication
  parameter: x-api-key
  sources:
  - openapi/makeswift-openapi.json
  type: apiKey
slug: makeswift-authentication
source_filename: makeswift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/makeswift-openapi.json + docs.makeswift.com/developer/api-reference/authentication\ndocs: https://docs.makeswift.com/developer/api-reference/authentication\nnotes: App API keys (prefix sk_) are created per app under Workspace -> Apps; Site\n  API keys are UUIDs. A Bearer token is also accepted, but only one auth method may\n  be sent per request (requests with both are rejected).\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Authentication\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: |-\n    API key authentication. Accepts either:\n    - App API key (e.g. sk_eczMHVBY9fV6GYFhvs53qcnxq7yptlXL3ABKOZtn6dQ)\n    - Site API key (UUID format, e.g. 550e8400-e29b-41d4-a716-446655440000)\n  sources:\n  - openapi/makeswift-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/makeswift/refs/heads/main/authentication/makeswift-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Visual Page Builder
- Website Builder
- Next.js
- Headless CMS
- Composable
- Content Management
- Web Development
- Developer Tools
---
