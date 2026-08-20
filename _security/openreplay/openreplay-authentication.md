---
api_key_in: []
api_specs:
- filename: openreplay-assist-api-openapi.yml
  format: yaml
  label: OpenReplay Assist API
  slug: openreplay-assist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openreplay/refs/heads/main/openapi/openreplay-assist-api-openapi.yml
- filename: openreplay-events-api-openapi.yml
  format: yaml
  label: OpenReplay Events API
  slug: openreplay-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openreplay/refs/heads/main/openapi/openreplay-events-api-openapi.yml
- filename: openreplay-jobs-api-openapi.yml
  format: yaml
  label: OpenReplay Jobs API
  slug: openreplay-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openreplay/refs/heads/main/openapi/openreplay-jobs-api-openapi.yml
- filename: openreplay-projects-api-openapi.yml
  format: yaml
  label: OpenReplay Projects API
  slug: openreplay-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openreplay/refs/heads/main/openapi/openreplay-projects-api-openapi.yml
- filename: openreplay-sessions-api-openapi.yml
  format: yaml
  label: OpenReplay Sessions API
  slug: openreplay-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openreplay/refs/heads/main/openapi/openreplay-sessions-api-openapi.yml
- filename: openreplay-users-api-openapi.yml
  format: yaml
  label: OpenReplay Users API
  slug: openreplay-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openreplay/refs/heads/main/openapi/openreplay-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openreplay Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenReplay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenReplay
provider_slug: openreplay
scheme_count: 1
schemes:
- description: Organization API key from Preferences > Account > Organization API Key.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openreplay-openapi.yml
  type: http
slug: openreplay-authentication
source_filename: openreplay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openreplay-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Organization API key from Preferences > Account > Organization API Key.\n  sources:\n  - openapi/openreplay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openreplay/refs/heads/main/authentication/openreplay-authentication.yml
summary_line: http · 1 scheme
tags:
- Debugging
- Error Tracking
- Open-Source
- Performance Monitoring
- Session Replay
- User Behavior
---
