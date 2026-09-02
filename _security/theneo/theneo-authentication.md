---
api_key_in:
- header
api_specs:
- filename: theneo-import-api-openapi.yml
  format: yaml
  label: Theneo Import API
  slug: theneo-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theneo/refs/heads/main/openapi/theneo-import-api-openapi.yml
- filename: theneo-projects-api-openapi.yml
  format: yaml
  label: Theneo Projects API
  slug: theneo-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theneo/refs/heads/main/openapi/theneo-projects-api-openapi.yml
- filename: theneo-publishing-api-openapi.yml
  format: yaml
  label: Theneo Publishing API
  slug: theneo-publishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theneo/refs/heads/main/openapi/theneo-publishing-api-openapi.yml
- filename: theneo-users-api-openapi.yml
  format: yaml
  label: Theneo Users API
  slug: theneo-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theneo/refs/heads/main/openapi/theneo-users-api-openapi.yml
- filename: theneo-workspaces-api-openapi.yml
  format: yaml
  label: Theneo Workspaces API
  slug: theneo-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theneo/refs/heads/main/openapi/theneo-workspaces-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Theneo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Theneo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Theneo
provider_slug: theneo
scheme_count: 1
schemes:
- description: API key for authentication. Generate from the Theneo dashboard. Can also be set via the THENEO_API_KEY environment variable when using the CLI or SDK.
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/theneo-api-openapi.yml
  type: apiKey
slug: theneo-authentication
source_filename: theneo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/theneo-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key for authentication. Generate from the Theneo dashboard. Can also be set\n    via the THENEO_API_KEY environment variable when using the CLI or SDK.\n  sources:\n  - openapi/theneo-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/theneo/refs/heads/main/authentication/theneo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Documentation
- Developer Portal
- Developer Tools
- Documentation Platform
- Artificial Intelligence
- AI Copilot
- MCP
- Platform
---
