---
api_key_in: []
api_specs:
- filename: screenpipe-activity-api-openapi.yml
  format: yaml
  label: Screenpipe Activity API
  slug: screenpipe-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenpipe/refs/heads/main/openapi/screenpipe-activity-api-openapi.yml
- filename: screenpipe-audio-api-openapi.yml
  format: yaml
  label: Screenpipe Audio API
  slug: screenpipe-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenpipe/refs/heads/main/openapi/screenpipe-audio-api-openapi.yml
- filename: screenpipe-cloud-archive-api-openapi.yml
  format: yaml
  label: Screenpipe Cloud Archive API
  slug: screenpipe-cloud-archive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenpipe/refs/heads/main/openapi/screenpipe-cloud-archive-api-openapi.yml
- filename: screenpipe-cloud-sync-api-openapi.yml
  format: yaml
  label: Screenpipe Cloud Sync API
  slug: screenpipe-cloud-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenpipe/refs/heads/main/openapi/screenpipe-cloud-sync-api-openapi.yml
- filename: screenpipe-data-management-api-openapi.yml
  format: yaml
  label: Screenpipe Data Management API
  slug: screenpipe-data-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenpipe/refs/heads/main/openapi/screenpipe-data-management-api-openapi.yml
- filename: screenpipe-data-retention-api-openapi.yml
  format: yaml
  label: Screenpipe Data Retention API
  slug: screenpipe-data-retention-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenpipe/refs/heads/main/openapi/screenpipe-data-retention-api-openapi.yml
- filename: screenpipe-database-api-openapi.yml
  format: yaml
  label: Screenpipe Database API
  slug: screenpipe-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenpipe/refs/heads/main/openapi/screenpipe-database-api-openapi.yml
- filename: screenpipe-elements-api-openapi.yml
  format: yaml
  label: Screenpipe Elements API
  slug: screenpipe-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenpipe/refs/heads/main/openapi/screenpipe-elements-api-openapi.yml
- filename: screenpipe-experimental-api-openapi.yml
  format: yaml
  label: Screenpipe Experimental API
  slug: screenpipe-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenpipe/refs/heads/main/openapi/screenpipe-experimental-api-openapi.yml
- filename: screenpipe-frames-api-openapi.yml
  format: yaml
  label: Screenpipe Frames API
  slug: screenpipe-frames-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenpipe/refs/heads/main/openapi/screenpipe-frames-api-openapi.yml
- filename: screenpipe-meetings-api-openapi.yml
  format: yaml
  label: Screenpipe Meetings API
  slug: screenpipe-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenpipe/refs/heads/main/openapi/screenpipe-meetings-api-openapi.yml
- filename: screenpipe-memories-api-openapi.yml
  format: yaml
  label: Screenpipe Memories API
  slug: screenpipe-memories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenpipe/refs/heads/main/openapi/screenpipe-memories-api-openapi.yml
- filename: screenpipe-search-api-openapi.yml
  format: yaml
  label: Screenpipe Search API
  slug: screenpipe-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenpipe/refs/heads/main/openapi/screenpipe-search-api-openapi.yml
- filename: screenpipe-speakers-api-openapi.yml
  format: yaml
  label: Screenpipe Speakers API
  slug: screenpipe-speakers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenpipe/refs/heads/main/openapi/screenpipe-speakers-api-openapi.yml
- filename: screenpipe-system-api-openapi.yml
  format: yaml
  label: Screenpipe System API
  slug: screenpipe-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenpipe/refs/heads/main/openapi/screenpipe-system-api-openapi.yml
- filename: screenpipe-tags-api-openapi.yml
  format: yaml
  label: Screenpipe Tags API
  slug: screenpipe-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenpipe/refs/heads/main/openapi/screenpipe-tags-api-openapi.yml
- filename: screenpipe-vault-api-openapi.yml
  format: yaml
  label: Screenpipe Vault API
  slug: screenpipe-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenpipe/refs/heads/main/openapi/screenpipe-vault-api-openapi.yml
- filename: screenpipe-vision-api-openapi.yml
  format: yaml
  label: Screenpipe Vision API
  slug: screenpipe-vision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenpipe/refs/heads/main/openapi/screenpipe-vision-api-openapi.yml
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
- Local-First
- Privacy
- AI Agents
- MCP
- Developer Tools
- Productivity
- Open-Source
---
