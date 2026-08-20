---
api_key_in: []
api_specs:
- filename: boltic-tables-api-openapi.yml
  format: yaml
  label: Boltic Tables API
  slug: tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-tables-api-openapi.yml
- filename: boltic-pipes-api-openapi.yml
  format: yaml
  label: Boltic Pipes API
  slug: pipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-pipes-api-openapi.yml
- filename: boltic-certificates-api-openapi.yml
  format: yaml
  label: Boltic Certificates API
  slug: boltic-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-certificates-api-openapi.yml
- filename: boltic-consumers-api-openapi.yml
  format: yaml
  label: Boltic Consumers API
  slug: boltic-consumers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-consumers-api-openapi.yml
- filename: boltic-destinations-api-openapi.yml
  format: yaml
  label: Boltic Destinations API
  slug: boltic-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-destinations-api-openapi.yml
- filename: boltic-events-api-openapi.yml
  format: yaml
  label: Boltic Events API
  slug: boltic-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-events-api-openapi.yml
- filename: boltic-executions-api-openapi.yml
  format: yaml
  label: Boltic Executions API
  slug: boltic-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-executions-api-openapi.yml
- filename: boltic-plugins-api-openapi.yml
  format: yaml
  label: Boltic Plugins API
  slug: boltic-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-plugins-api-openapi.yml
- filename: boltic-queries-api-openapi.yml
  format: yaml
  label: Boltic Queries API
  slug: boltic-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-queries-api-openapi.yml
- filename: boltic-routes-api-openapi.yml
  format: yaml
  label: Boltic Routes API
  slug: boltic-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-routes-api-openapi.yml
- filename: boltic-rows-api-openapi.yml
  format: yaml
  label: Boltic Rows API
  slug: boltic-rows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-rows-api-openapi.yml
- filename: boltic-services-api-openapi.yml
  format: yaml
  label: Boltic Services API
  slug: boltic-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-services-api-openapi.yml
- filename: boltic-sources-api-openapi.yml
  format: yaml
  label: Boltic Sources API
  slug: boltic-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-sources-api-openapi.yml
- filename: boltic-stream-sources-api-openapi.yml
  format: yaml
  label: Boltic Stream Sources API
  slug: boltic-stream-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-stream-sources-api-openapi.yml
- filename: boltic-sync-runs-api-openapi.yml
  format: yaml
  label: Boltic Sync Runs API
  slug: boltic-sync-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-sync-runs-api-openapi.yml
- filename: boltic-triggers-api-openapi.yml
  format: yaml
  label: Boltic Triggers API
  slug: boltic-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-triggers-api-openapi.yml
- filename: boltic-workflows-api-openapi.yml
  format: yaml
  label: Boltic Workflows API
  slug: boltic-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Boltic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Boltic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Boltic
provider_slug: boltic
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/boltic-gateway-api-openapi.yml
  - openapi/boltic-pipes-api-openapi.yml
  - openapi/boltic-streams-api-openapi.yml
  - openapi/boltic-tables-api-openapi.yml
  - openapi/boltic-workflow-api-openapi.yml
  type: http
slug: boltic-authentication
source_filename: boltic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/boltic-gateway-api-openapi.yml, openapi/boltic-pipes-api-openapi.yml, openapi/boltic-streams-api-openapi.yml,\n  openapi/boltic-tables-api-openapi.yml, openapi/boltic-workflow-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/boltic-gateway-api-openapi.yml\n  - openapi/boltic-pipes-api-openapi.yml\n  - openapi/boltic-streams-api-openapi.yml\n  - openapi/boltic-tables-api-openapi.yml\n  - openapi/boltic-workflow-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/authentication/boltic-authentication.yml
summary_line: http · 1 scheme
tags:
- Automation
- Data Sync
- Gateways
- No-Code
- Streaming
- Workflows
---
