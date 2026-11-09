---
anonymous_access: false
api_key_in: []
api_specs:
- filename: anjal-app-addresses-api-openapi.yml
  format: yaml
  label: Anjal Addresses API
  slug: anjal-app-addresses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-addresses-api-openapi.yml
- filename: anjal-app-cadences-api-openapi.yml
  format: yaml
  label: Anjal Cadences API
  slug: anjal-app-cadences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-cadences-api-openapi.yml
- filename: anjal-app-domains-api-openapi.yml
  format: yaml
  label: Anjal Domains API
  slug: anjal-app-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-domains-api-openapi.yml
- filename: anjal-app-drafts-api-openapi.yml
  format: yaml
  label: Anjal Drafts API
  slug: anjal-app-drafts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-drafts-api-openapi.yml
- filename: anjal-app-inboxes-api-openapi.yml
  format: yaml
  label: Anjal Inboxes API
  slug: anjal-app-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-inboxes-api-openapi.yml
- filename: anjal-app-linkedin-outreach-api-openapi.yml
  format: yaml
  label: Anjal LinkedIn — Outreach API
  slug: anjal-app-linkedin-outreach-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-linkedin-outreach-api-openapi.yml
- filename: anjal-app-linkedin-posts-api-openapi.yml
  format: yaml
  label: Anjal LinkedIn — Posts API
  slug: anjal-app-linkedin-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-linkedin-posts-api-openapi.yml
- filename: anjal-app-linkedin-searches-api-openapi.yml
  format: yaml
  label: Anjal LinkedIn — Searches API
  slug: anjal-app-linkedin-searches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-linkedin-searches-api-openapi.yml
- filename: anjal-app-linkedin-sessions-api-openapi.yml
  format: yaml
  label: Anjal LinkedIn — Sessions API
  slug: anjal-app-linkedin-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-linkedin-sessions-api-openapi.yml
- filename: anjal-app-linkedin-signals-api-openapi.yml
  format: yaml
  label: Anjal LinkedIn — Signals API
  slug: anjal-app-linkedin-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-linkedin-signals-api-openapi.yml
- filename: anjal-app-lists-api-openapi.yml
  format: yaml
  label: Anjal Lists API
  slug: anjal-app-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-lists-api-openapi.yml
- filename: anjal-app-messages-api-openapi.yml
  format: yaml
  label: Anjal Messages API
  slug: anjal-app-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-messages-api-openapi.yml
- filename: anjal-app-metrics-api-openapi.yml
  format: yaml
  label: Anjal Metrics API
  slug: anjal-app-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-metrics-api-openapi.yml
- filename: anjal-app-tenants-api-openapi.yml
  format: yaml
  label: Anjal Tenants API
  slug: anjal-app-tenants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-tenants-api-openapi.yml
- filename: anjal-app-webhooks-api-openapi.yml
  format: yaml
  label: Anjal Webhooks API
  slug: anjal-app-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-webhooks-api-openapi.yml
- filename: anjal-app-websocket-api-openapi.yml
  format: yaml
  label: Anjal WebSocket API
  slug: anjal-app-websocket-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-websocket-api-openapi.yml
- filename: anjal-app-workspaces-api-openapi.yml
  format: yaml
  label: Anjal Workspaces API
  slug: anjal-app-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anjal-app/openapi/anjal-app-workspaces-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Anjal App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anjal declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Anjal
provider_slug: anjal-app
scheme_count: 2
schemes:
- description: API key header for authentication
  in: header
  name: X-API-Key
  type: apiKey
- bearerFormat: JWT
  description: Bearer token alternative
  scheme: bearer
  type: http
slug: anjal-app-authentication
source_filename: anjal-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: \"https://anjal.app/docs\"\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: API key header for authentication\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Bearer token alternative\n"
source_yaml_url: https://artifacts.apis.io/anjal-app/authentication/anjal-app-authentication.yml
summary_line: 2 schemes
tags:
- Email
- Artificial Intelligence
- Agents
- Software-as-a-Service
- Email API
---
