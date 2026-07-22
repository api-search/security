---
api_key_in: []
api_specs:
- filename: screenpipe-openapi-original.yml
  format: yaml
  label: Screenpipe Local REST API
  slug: screenpipe-local-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenpipe/refs/heads/main/openapi/screenpipe-openapi-original.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Screenpipe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Screenpipe declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Screenpipe
provider_slug: screenpipe
scheme_count: 0
schemes: []
slug: screenpipe-authentication
source_filename: screenpipe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/screenpipe-openapi-original.yml\ndocs: https://docs.screenpipe.com/connection-reference\nsummary:\n  types: []\n  model: local-loopback\n  note: >-\n    The OpenAPI declares NO securitySchemes. The screenpipe REST API is served\n    locally at http://localhost:3030 and is unauthenticated by default, relying\n    on loopback binding and OS-level process isolation rather than API-layer\n    auth. An OPTIONAL bearer token can be retrieved via the CLI command\n    `screenpipe auth token` and supplied by clients (e.g. the MCP server) when\n    the local server is configured to require it. Pipes are additionally scoped\n    by an endpoint allowlist (see docs pipe-permissions).\nschemes: []\noptional_token:\n  mechanism: bearer\n  retrieval: screenpipe auth token\n  docs: https://docs.screenpipe.com/getting-started\npipe_permissions:\n  docs: https://docs.screenpipe.com/pipe-permissions\n  note: >-\n    Per-pipe API access\
  \ is controlled by allowlisting endpoints and restricting\n    writes, scoping permissions per automation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/screenpipe/refs/heads/main/authentication/screenpipe-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Screen Recording
- Screen Memory
- Audio Transcription
- Meeting Intelligence
- Local First
- Privacy
- AI Agents
- MCP
- Developer Tools
- Productivity
- Open Source
---
