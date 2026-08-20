---
api_key_in:
- header
api_specs:
- filename: eraser-ai-requests-api-openapi.yml
  format: yaml
  label: Eraser AI Requests API
  slug: eraser-ai-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eraser/refs/heads/main/openapi/eraser-ai-requests-api-openapi.yml
- filename: eraser-audit-logs-api-openapi.yml
  format: yaml
  label: Eraser Audit Logs API
  slug: eraser-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eraser/refs/heads/main/openapi/eraser-audit-logs-api-openapi.yml
- filename: eraser-diagram-elements-api-openapi.yml
  format: yaml
  label: Eraser Diagram Elements API
  slug: eraser-diagram-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eraser/refs/heads/main/openapi/eraser-diagram-elements-api-openapi.yml
- filename: eraser-diagrams-ai-api-openapi.yml
  format: yaml
  label: Eraser Diagrams (AI) API
  slug: eraser-diagrams-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eraser/refs/heads/main/openapi/eraser-diagrams-ai-api-openapi.yml
- filename: eraser-files-api-openapi.yml
  format: yaml
  label: Eraser Files API
  slug: eraser-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eraser/refs/heads/main/openapi/eraser-files-api-openapi.yml
- filename: eraser-folders-api-openapi.yml
  format: yaml
  label: Eraser Folders API
  slug: eraser-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eraser/refs/heads/main/openapi/eraser-folders-api-openapi.yml
- filename: eraser-usage-metrics-api-openapi.yml
  format: yaml
  label: Eraser Usage Metrics API
  slug: eraser-usage-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eraser/refs/heads/main/openapi/eraser-usage-metrics-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Eraser Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eraser secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Eraser
provider_slug: eraser
scheme_count: 2
schemes:
- description: Team-specific API bearer token from Eraser settings
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/eraser-eraser-api-openapi.yml
  type: http
- description: Audit-specific API key for accessing audit log endpoints
  in: header
  name: auditApiKey
  parameter: Authorization
  sources:
  - openapi/eraser-eraser-api-openapi.yml
  type: apiKey
slug: eraser-authentication
source_filename: eraser-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/eraser-eraser-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Team-specific API bearer token from Eraser settings\n  sources:\n  - openapi/eraser-eraser-api-openapi.yml\n- name: auditApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Audit-specific API key for accessing audit log endpoints\n  sources:\n  - openapi/eraser-eraser-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eraser/refs/heads/main/authentication/eraser-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Diagrams
- Documentation
- Artificial Intelligence
- Technical Documentation
- Diagramming
- Architecture
- Developer Tools
---
