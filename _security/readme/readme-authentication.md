---
api_key_in: []
api_specs:
- filename: readme-openapi.yml
  format: yaml
  label: ReadMe API
  slug: readme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-openapi.yml
- filename: readme-developer-metrics-openapi.yml
  format: yaml
  label: ReadMe Developer Metrics API
  slug: developer-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-developer-metrics-openapi.yml
- filename: readme-personalized-docs-webhook-asyncapi.yml
  format: yaml
  label: ReadMe Personalized Docs Webhook
  slug: personalized-docs-webhook
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/asyncapi/readme-personalized-docs-webhook-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Readme Authentication
name_suffix: Authentication
oauth_flows: []
overview: ReadMe secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ReadMe
provider_slug: readme
scheme_count: 2
schemes:
- description: HTTP Basic auth using your ReadMe API key as the username (password blank).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/readme-developer-metrics-openapi.yml
  type: http
- description: Use your ReadMe API key as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/readme-openapi.yml
  type: http
slug: readme-authentication
source_filename: readme-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/readme-developer-metrics-openapi.yml, openapi/readme-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth using your ReadMe API key as the username (password blank).\n  sources:\n  - openapi/readme-developer-metrics-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Use your ReadMe API key as a Bearer token in the Authorization header.\n  sources:\n  - openapi/readme-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/authentication/readme-authentication.yml
summary_line: http · 2 schemes
tags:
- Documentation
- Developer Hub
- API Reference
- Portals
- Analytics
- AI
- MCP
- Bi-Directional Sync
---
