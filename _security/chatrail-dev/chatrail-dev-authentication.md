---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chatrail-dev-ai-api-openapi.yml
  format: yaml
  label: chatrail-dev AI API
  slug: chatrail-dev-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-ai-api-openapi.yml
- filename: chatrail-dev-auth-api-openapi.yml
  format: yaml
  label: chatrail-dev Auth API
  slug: chatrail-dev-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-auth-api-openapi.yml
- filename: chatrail-dev-billing-api-openapi.yml
  format: yaml
  label: chatrail-dev Billing API
  slug: chatrail-dev-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-billing-api-openapi.yml
- filename: chatrail-dev-connections-api-openapi.yml
  format: yaml
  label: chatrail-dev Connections API
  slug: chatrail-dev-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-connections-api-openapi.yml
- filename: chatrail-dev-groups-api-openapi.yml
  format: yaml
  label: chatrail-dev Groups API
  slug: chatrail-dev-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-groups-api-openapi.yml
- filename: chatrail-dev-internal-api-openapi.yml
  format: yaml
  label: chatrail-dev Internal API
  slug: chatrail-dev-internal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-internal-api-openapi.yml
- filename: chatrail-dev-mcp-api-openapi.yml
  format: yaml
  label: chatrail-dev MCP API
  slug: chatrail-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-mcp-api-openapi.yml
- filename: chatrail-dev-messages-api-openapi.yml
  format: yaml
  label: chatrail-dev Messages API
  slug: chatrail-dev-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-messages-api-openapi.yml
- filename: chatrail-dev-operational-api-openapi.yml
  format: yaml
  label: chatrail-dev Operational API
  slug: chatrail-dev-operational-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-operational-api-openapi.yml
- filename: chatrail-dev-opt-outs-api-openapi.yml
  format: yaml
  label: chatrail-dev Opt Outs API
  slug: chatrail-dev-opt-outs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-opt-outs-api-openapi.yml
- filename: chatrail-dev-schedules-api-openapi.yml
  format: yaml
  label: chatrail-dev Schedules API
  slug: chatrail-dev-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-schedules-api-openapi.yml
- filename: chatrail-dev-team-api-openapi.yml
  format: yaml
  label: chatrail-dev Team API
  slug: chatrail-dev-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-team-api-openapi.yml
- filename: chatrail-dev-webhooks-api-openapi.yml
  format: yaml
  label: chatrail-dev Webhooks API
  slug: chatrail-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-webhooks-api-openapi.yml
- filename: chatrail-dev-workspace-api-openapi.yml
  format: yaml
  label: chatrail-dev Workspace API
  slug: chatrail-dev-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-workspace-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Chatrail Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: chatrail-dev declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: chatrail-dev
provider_slug: chatrail-dev
scheme_count: 2
schemes:
- description: 'A workspace API key, `cr_live_…`. Server-side only: it carries workspace authority and must never reach a browser.'
  in: header
  name: Authorization
  scheme: bearer
  type: http
- description: Dashboard session cookie. Set by `/v1/auth/verify`.
  in: cookie
  name: chatrail_session
  type: apiKey
slug: chatrail-dev-authentication
source_filename: chatrail-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: \"https://www.chatrail.dev/openapi.json\"\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"A workspace API key, `cr_live_…`. Server-side only: it carries workspace authority and must never reach a browser.\"\n    name: Authorization\n    in: header\n  - type: apiKey\n    in: cookie\n    name: chatrail_session\n    description: \"Dashboard session cookie. Set by `/v1/auth/verify`.\"\n"
source_yaml_url: https://artifacts.apis.io/chatrail-dev/authentication/chatrail-dev-authentication.yml
summary_line: 2 schemes
tags:
- WhatsApp
- API
- Messaging
- AI
- Developers
---
