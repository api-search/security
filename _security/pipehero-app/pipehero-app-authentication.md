---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pipehero-app-mcp-api-openapi.yml
  format: yaml
  label: pipehero-app MCP API
  slug: pipehero-app-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pipehero-app/openapi/pipehero-app-mcp-api-openapi.yml
- filename: pipehero-app-slack-api-openapi.yml
  format: yaml
  label: pipehero-app Slack API
  slug: pipehero-app-slack-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pipehero-app/openapi/pipehero-app-slack-api-openapi.yml
- filename: pipehero-app-webhooks-api-openapi.yml
  format: yaml
  label: pipehero-app Webhooks API
  slug: pipehero-app-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pipehero-app/openapi/pipehero-app-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Pipehero App Authentication
name_suffix: Authentication
oauth_flows: []
overview: pipehero-app declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: pipehero-app
provider_slug: pipehero-app
scheme_count: 1
schemes:
- description: Bearer token used in Authorization header
  scheme: bearer
  type: http
slug: pipehero-app-authentication
source_filename: pipehero-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: \"https://pipehero.app/docs/tokens\"\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"Bearer token used in Authorization header\"\n"
source_yaml_url: https://artifacts.apis.io/pipehero-app/authentication/pipehero-app-authentication.yml
summary_line: 1 scheme
tags:
- Webhook
- API Workspace
- Developer Tools
- MCP
- Integration
---
