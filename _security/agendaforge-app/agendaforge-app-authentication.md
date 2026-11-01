---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agendaforge-app-connection-api-openapi.yml
  format: yaml
  label: agendaforge-app Connection API
  slug: agendaforge-app-connection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agendaforge-app/openapi/agendaforge-app-connection-api-openapi.yml
- filename: agendaforge-app-jobs-api-openapi.yml
  format: yaml
  label: agendaforge-app Jobs API
  slug: agendaforge-app-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agendaforge-app/openapi/agendaforge-app-jobs-api-openapi.yml
- filename: agendaforge-app-records-api-openapi.yml
  format: yaml
  label: agendaforge-app Records API
  slug: agendaforge-app-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agendaforge-app/openapi/agendaforge-app-records-api-openapi.yml
- filename: agendaforge-app-webhooks-api-openapi.yml
  format: yaml
  label: agendaforge-app Webhooks API
  slug: agendaforge-app-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agendaforge-app/openapi/agendaforge-app-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Agendaforge App Authentication
name_suffix: Authentication
oauth_flows: []
overview: agendaforge-app declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: agendaforge-app
provider_slug: agendaforge-app
scheme_count: 2
schemes:
- description: 'Send the API key as a Bearer token, e.g., Authorization: Bearer afk_live_<key>'
  in: header
  name: Authorization
  type: apiKey
- description: Alternative header for API key.
  in: header
  name: X-API-Key
  type: apiKey
slug: agendaforge-app-authentication
source_filename: agendaforge-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://agendaforge.app/docs/api#authentication\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: \"Send the API key as a Bearer token, e.g., Authorization: Bearer afk_live_<key>\"\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: \"Alternative header for API key.\"\nscopes:\n  - name: public_api\n    description: Grants access to the REST API (default).\n  - name: mcp:read\n    description: Grants read access to the AgendaForge MCP server for AI clients.\n  - name: mcp:write\n    description: Grants write access to the AgendaForge MCP server for AI clients.\n  - name: tickets:import\n    description: Allows importing tickets via POST /imports/tickets.\n"
source_yaml_url: https://artifacts.apis.io/agendaforge-app/authentication/agendaforge-app-authentication.yml
summary_line: 2 schemes
tags:
- Event Management
- SaaS
- AI-native
- Conferences
- Software
---
